# pgdaiml-capstone-project
First complete AI and ML Project

PROJECT OBJECTIVE
The central objective of this project is to effectively detect anomalies within the collected event data. The approach focuses on distinguishing between normal and anomalous activities by thoroughly analyzing extensive log records. Through this process, the project aims to identify atypical patterns or behaviors that could signal potential security threats or operational concerns within the network environment.
Additionally, the project seeks to enhance the capabilities of Intrusion Detection Systems (IDS). By leveraging the insights gained from anomaly detection, the goal is to contribute to the development of robust and adaptive security solutions tailored for real-time IoT networks. This advancement is intended to support proactive defense mechanisms, enabling timely detection and mitigation of emerging threats.

EVALUATION METRICS
To assess the effectiveness of the classification models in anomaly detection, several key performance metrics will be used: Precision, Recall, F1 Score, and Area Under the ROC Curve (AUC). These metrics are essential for evaluating the balance between correctly identifying anomalies and minimizing false detections.

MACHINE LEARNING ALGORITHMS
The project will explore a range of machine learning algorithms to determine the most suitable approach for anomaly detection. Specifically, Neural Networks, Random Forest, XGBoost, and Logistic Regression will be considered. The comparative analysis of these algorithms will help establish which model offers the best performance for the given dataset and objectives.

DATA SOURCE AND CHARACTERISTICS
The primary dataset utilized in this project is RT-IoT2022, a proprietary resource curated from a real-time IoT infrastructure. This comprehensive dataset integrates a wide variety of IoT devices and incorporates advanced network attack methodologies to emulate real-world environments. RT-IoT2022 captures both normal and adversarial network behaviors, ensuring a balanced and realistic depiction of IoT network traffic patterns.
Within RT-IoT2022, data is collected from devices such as ThingSpeak-LED, Wipro-Bulb, and MQTT-Temp, reflecting a broad spectrum of typical IoT deployments. Additionally, the dataset includes simulated attack scenarios that cover Brute-Force SSH attacks, DDoS attacks executed through tools like Hping and Slowloris, as well as reconnaissance and exploitation patterns using Nmap. This diversity in attack vectors and device types provides an invaluable resource for studying the nuanced behaviors present in real-time IoT networks.
To ensure the fidelity and granularity of the captured traffic, the dataset employs the Zeek network monitoring tool alongside the Flowmeter plugin. This setup allows for meticulous recording of bidirectional network attributes, offering detailed insights into both inbound and outbound traffic characteristics. As a result, RT-IoT2022 stands as a vital asset for researchers aiming to enhance Intrusion Detection Systems (IDS), promoting the advancement of robust and adaptive security solutions tailored for the dynamic landscape of real-time IoT environments.
