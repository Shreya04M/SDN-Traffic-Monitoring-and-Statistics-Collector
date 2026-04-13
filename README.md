# SDN-Traffic-Monitoring-and-Statistics-Collector
This project implements an SDN-based traffic monitoring system using Mininet and Ryu controller. The controller collects flow-level statistics such as packet count and byte count, performs periodic monitoring, and displays traffic behavior.

SDN-Traffic-Monitoring/
│
├── traffic_monitor.py
├── README.md
├── screenshots/
│   ├── ping.png
│   ├── iperf.png
│   ├── flow_table.png
│   └── controller_logs.png
└── requirements.txt (optional)
Packets from hosts are sent to the controller. The controller installs flow rules and periodically collects statistics such as packet count and byte count.
