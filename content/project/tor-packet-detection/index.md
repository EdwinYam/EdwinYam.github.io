---
title: Tor Packet Detection
summary: A website that provides an intuitive interface for users to track dark web flow and identify potential security threats
tags:
  - Deep Learning
date: '2018-07-04T00:00:00Z'
PublishDate: '2018-07-04T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    name: Follow
    url: https://github.com/EdwinYam
url_code: 'https://github.com/codingbaobao/React-TorDetection'
url_pdf: ''
url_slides: 'https://docs.google.com/presentation/d/13cGDGfIx3MJfcqmQrKtfhkCgjsWMqCVYby1CBdaUT3s/edit?usp=sharing'
url_video: 'https://www.youtube.com/watch?v=1YCn4naV0_M'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

# Network Packet Classification for Dark Web Flow Detection

The project aims to develop a web service for detecting Dark Web flows by performing network packet classification using machine learning algorithms. The project leverages selected features and applies machine learning methods such as K-Nearest Neighbors (KNN), Decision Tree, and Random Forest. The system operates in both real-time and offline modes, allowing for continuous flow analysis and retrospective analysis of pcap files.

## Network Packet and Selected Features
A network packet is a formatted unit of data carried by a packet-switched network. Each packet consists of control information, including a header and payload. In this project, specific features are selected for packet classification based on two tasks:

- **Task A:** Flow IAT Min, Bwd IAT Std, Bwd IAT Mean, Bwd IAT Max
- **Task B:** Flow Duration, Flow Bytes/s, Flow IAT Mean, Flow IAT Max, Flow IAT Min, Fwd IAT Mean, Fwd IAT Max, Fwd IAT Min, Bwd IAT Min

## Packet Classification using Machine Learning
The project employs three popular machine learning methods for packet classification:

- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest

## Source Code Structure
The source code structure for the project can be divided into two scenarios: real-time flow analysis and offline flow analysis.

### Real-time Flow Analysis
In real-time flow analysis, the system captures network packets using a network adapter. The captured packets are then processed using the CICFLOWMETER tool, which converts the pcap files to CSV format. The CSV files are further processed by the classifier, which applies the selected machine learning method. The output of the classifier is a JSON file containing the predictions.

The flow of the real-time analysis can be summarized as follows:

```
network adapter (listen) -> pcap file -> CICFLOWMETER -> pcap2csv -> csv file -> classifier -> json output
```

### Offline Flow Analysis
In offline flow analysis, pcap files are directly processed using the pcap2csv tool, which converts the pcap files to CSV format. The CSV files are then passed to the classifier, which applies the selected machine learning method. Similar to real-time analysis, the output of the classifier is a JSON file containing the predictions.

The flow of the offline analysis can be summarized as follows:

```
pcap file -> pcap2csv -> csv file -> classifier -> json output
```

## Framework and Flow Analysis
The project utilizes a responsive web design (RWD) framework to provide an intuitive interface for users. The flow analysis process involves the following steps:

1. The EXPRESS framework calls Python to initiate the flow analysis.
2. Python processes the network packets or pcap files and generates predictions.
3. Python saves the predictions in JSON format files.
4. EXPRESS reads the JSON files and passes them to REACT, which is responsible for building the user interface.

## Online Flow Analysis
To enable continuous flow analysis, the project utilizes the tcpdump tool to periodically capture and dump pcap files. The dumped pcap files are then processed using the same flow analysis steps as described in the real-time flow analysis section.

The online flow analysis allows for the continuous monitoring and detection of Dark Web activities.

## Contribution and Conclusion
The primary contribution of this project is the development of a web service for Dark Web flow detection. The system provides an intuitive interface for users through responsive web design. It offers both online and offline flow analysis modes, allowing for real-time tracking as well as retrospective analysis of pcap files.

By leveraging machine learning algorithms and selected packet features, the project enhances the accuracy and efficiency of Dark Web flow detection. The seamless integration of tcpdump, CICFLOWMETER, pcap2csv, Python, EXPRESS, and REACT enables a comprehensive and user-friendly solution for network packet classification and Dark Web flow analysis.

The project's contribution lies in providing a web-based service for Dark Web flow detection, offering an intuitive interface for users, and facilitating on-line tracking capabilities.