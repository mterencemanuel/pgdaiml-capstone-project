# Data Dictionary: RT-IoT2022 Dataset Features

This data dictionary provides an overview of the features used in the analysis, including original features from the RT-IoT2022 dataset and new features engineered during preprocessing.

## Original Features

| Feature Name | Type        | Description                                       |
|:-------------|:------------|:--------------------------------------------------|
| `id.orig_p`      | Integer     | Originator port number.                           |
| `id.resp_p`      | Integer     | Responder port number.                            |
| `proto`          | Categorical | Transport layer protocol (e.g., TCP, UDP, ICMP).   |
| `service`        | Categorical | Application layer protocol (e.g., HTTP, DNS, SSH).|
| `flow_duration`  | Continuous  | Duration of the network flow.                     |
| `fwd_pkts_tot`   | Integer     | Total number of forward packets.                  |
| `bwd_pkts_tot`   | Integer     | Total number of backward packets.                 |
| `fwd_data_pkts_tot` | Integer  | Total number of forward data packets.             |
| `bwd_data_pkts_tot` | Integer  | Total number of backward data packets.            |
| `fwd_pkts_per_sec` | Float    | Forward packets per second.                       |
| `bwd_pkts_per_sec` | Float    | Backward packets per second.                      |
| `flow_pkts_per_sec`| Float    | Total packets per second.                         |
| `down_up_ratio`  | Float       | Ratio of downstream to upstream bytes.            |

| `fwd_header_size_tot` | Integer | Total size of forward headers.                    |
| `fwd_header_size_min` | Integer | Minimum size of forward headers.                  |
| `fwd_header_size_max` | Integer | Maximum size of forward headers.                  |
| `bwd_header_size_tot` | Integer | Total size of backward headers.                   |
| `bwd_header_size_min` | Integer | Minimum size of backward headers.                 |
| `bwd_header_size_max` | Integer | Maximum size of backward headers.                 |
| `flow_FIN_flag_count`| Integer | Count of FIN flags in the flow.                   |
| `flow_SYN_flag_count`| Integer | Count of SYN flags in the flow.                   |
| `flow_RST_flag_count`| Integer | Count of RST flags in the flow.                   |
| `fwd_PSH_flag_count` | Integer | Count of PSH flags in forward packets.            |
| `bwd_PSH_flag_count` | Integer | Count of PSH flags in backward packets.           |
| `flow_ACK_flag_count`| Integer | Count of ACK flags in the flow.                   |
| `fwd_URG_flag_count` | Integer | Count of URG flags in forward packets.            |
| `bwd_URG_flag_count` | Integer | Count of URG flags in backward packets.           |
| `flow_CWR_flag_count`| Integer | Count of CWR flags in the flow.                   |
| `flow_ECE_flag_count`| Integer | Count of ECE flags in the flow.                   |
| `fwd_pkts_payload.min`| Integer | Minimum payload size in forward packets.        |
| `fwd_pkts_payload.max`| Integer | Maximum payload size in forward packets.        |
| `fwd_pkts_payload.tot`| Integer | Total payload size in forward packets.          |
| `fwd_pkts_payload.avg`| Float   | Average payload size in forward packets.        |
| `fwd_pkts_payload.std`| Float   | Standard deviation of payload size in forward packets.|
| `bwd_pkts_payload.min`| Integer | Minimum payload size in backward packets.       |
| `bwd_pkts_payload.max`| Integer | Maximum payload size in backward packets.       |
| `bwd_pkts_payload.tot`| Integer | Total payload size in backward packets.         |
| `bwd_pkts_payload.avg`| Float   | Average payload size in backward packets.       |
| `bwd_pkts_payload.std`| Float   | Standard deviation of payload size in backward packets.|
| `flow_pkts_payload.min`| Integer | Minimum payload size in flow packets.           |
| `flow_pkts_payload.max`| Integer | Maximum payload size in flow packets.           |
| `flow_pkts_payload.tot`| Integer | Total payload size in flow packets.             |
| `flow_pkts_payload.avg`| Float   | Average payload size in flow packets.           |
| `flow_pkts_payload.std`| Float   | Standard deviation of payload size in flow packets.|
| `fwd_iat.min`        | Float     | Minimum inter-arrival time in forward direction. |
| `fwd_iat.max`        | Float     | Maximum inter-arrival time in forward direction. |
| `fwd_iat.tot`        | Float     | Total inter-arrival time in forward direction.   |
| `fwd_iat.avg`        | Float     | Average inter-arrival time in forward direction. |
| `fwd_iat.std`        | Float     | Standard deviation of inter-arrival time in forward direction.|
| `bwd_iat.min`        | Float     | Minimum inter-arrival time in backward direction. |
| `bwd_iat.max`        | Float     | Maximum inter-arrival time in backward direction. |
| `bwd_iat.tot`        | Float     | Total inter-arrival time in backward direction.   |
| `bwd_iat.avg`        | Float     | Average inter-arrival time in backward direction. |
| `bwd_iat.std`        | Float     | Standard deviation of inter-arrival time in backward direction.|
| `flow_iat.min`       | Float     | Minimum inter-arrival time in the flow.          |
| `flow_iat.max`       | Float     | Maximum inter-arrival time in the flow.          |
| `flow_iat.tot`       | Float     | Total inter-arrival time in the flow.            |
| `flow_iat.avg`       | Float     | Average inter-arrival time in the flow.          |
| `flow_iat.std`       | Float     | Standard deviation of inter-arrival time in the flow.|
| `payload_bytes_per_second`| Float | Payload bytes transferred per second.           |
| `fwd_subflow_pkts`   | Float     | Number of packets in forward subflow.             |
| `bwd_subflow_pkts`   | Float     | Number of packets in backward subflow.            |
| `fwd_subflow_bytes`  | Float     | Number of bytes in forward subflow.               |
| `bwd_subflow_bytes`  | Float     | Number of bytes in backward subflow.              |
| `fwd_bulk_bytes`     | Float     | Number of bulk bytes in forward direction.        |
| `bwd_bulk_bytes`     | Float     | Number of bulk bytes in backward direction.       |
| `fwd_bulk_packets`   | Float     | Number of bulk packets in forward direction.      |
| `bwd_bulk_packets`   | Float     | Number of bulk packets in backward direction.     |
| `fwd_bulk_rate`      | Float     | Rate of bulk data in forward direction.           |
| `bwd_bulk_rate`      | Float     | Rate of bulk data in backward direction.          |
| `active.min`         | Float     | Minimum duration of active time in flow.          |
| `active.max`         | Float     | Maximum duration of active time in flow.          |
| `active.tot`         | Float     | Total duration of active time in flow.            |
| `active.avg`         | Float     | Average duration of active time in flow.          |
| `active.std`         | Float     | Standard deviation of active time in flow.        |
| `idle.min`           | Float     | Minimum duration of idle time in flow.            |
| `idle.max`           | Float     | Maximum duration of idle time in flow.            |
| `idle.tot`           | Float     | Total duration of idle time in flow.              |
| `idle.avg`           | Float     | Average duration of idle time in flow.            |
| `idle.std`           | Float     | Standard deviation of idle time in flow.          |

| `fwd_init_window_size`| Integer  | Initial window size in forward direction.       |
| `bwd_init_window_size`| Integer  | Initial window size in backward direction.      |
| `fwd_last_window_size`| Integer  | Last window size in forward direction.          |
| `Attack_type`        | Categorical | Type of network attack (Target variable).         |
| `id`                 | Integer     | Unique identifier for the flow (ID column).       |

## Engineered Features

| Feature Name                 | Type      | Description                                                 |
|:-----------------------------|:----------|:------------------------------------------------------------|
| `Total_Packets`              | Float     | Sum of `fwd_pkts_tot` and `bwd_pkts_tot`.                   |
| `Total_Bytes_Payload`        | Float     | Sum of `fwd_pkts_payload.tot` and `bwd_pkts_payload.tot`.   |
| `Fwd_Bwd_Packet_Ratio`       | Float     | Ratio of `fwd_pkts_tot` to `bwd_pkts_tot`.                  |
| `Fwd_Bwd_Data_Packet_Ratio`  | Float     | Ratio of `fwd_data_pkts_tot` to `bwd_data_pkts_tot`.        |
| `Avg_Fwd_Packet_Size`        | Float     | Average payload size of forward packets (`fwd_pkts_payload.tot` / `fwd_pkts_tot`). |
| `Avg_Bwd_Packet_Size`        | Float     | Average payload size of backward packets (`bwd_pkts_payload.tot` / `bwd_pkts_tot`). |
| `SYN_Flag_Rate`              | Float     | Rate of SYN flags relative to `Total_Packets`.              |
| `FIN_Flag_Rate`              | Float     | Rate of FIN flags relative to `Total_Packets`.              |
| `RST_Flag_Rate`              | Float     | Rate of RST flags relative to `Total_Packets`.              |
| `flow_duration_binned`       | Integer   | `flow_duration` binned into 5 equal-frequency categories.   |
| `proto_<protocol_name>`      | Binary    | One-hot encoded features for `proto` (e.g., `proto_tcp`).  |
| `service_<service_name>`     | Binary    | One-hot encoded features for `service` (e.g., `service_http`).|

| `flow_duration_binned_<bin_idx>`| Binary | One-hot encoded features for `flow_duration_binned`.      |