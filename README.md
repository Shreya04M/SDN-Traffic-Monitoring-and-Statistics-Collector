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
Objectives
        To understand SDN architecture and controller-based networking
        To implement flow rule-based forwarding using OpenFlow
        To monitor network traffic using flow statistics
        To analyze performance using latency and throughput
Tools :
        Mininet (Network Emulator)
        Ryu Controller (SDN Controller)
        Python
        Ubuntu Virtual Machine
        iperf (for throughput testing)
        ping (for latency testing)   

Network Topology :
        Open flow switch -1 
        3 hosts (h1, h2 , h3 )

Working of the project:

The Mininet environment creates a virtual network with hosts and switches.
The Ryu controller acts as the central control unit.
When a packet arrives at the switch, it sends a packet_in message to the controller.
The controller processes the packet and installs appropriate flow rules in the switch.
The controller periodically requests flow statistics from the switch.
Flow statistics such as packet count and byte count are collected and displayed.

Expected Output :
        Successful communication between hosts
        Throughput values displayed using iperf
        Controller logs showing:
            Packet count
            Byte count
        

Results :
        Packet count increases as traffic increases
        Byte count increases significantly during iperf testing
        Latency remains stable during normal traffic conditions
        The controller successfully monitors and logs network activity


Conclusion :
        This project demonstrates the use of SDN for centralized 
This project demonstrates the use of SDN for centralized network monitoring. By using Mininet and the Ryu controller, we were able to implement a system that dynamically manages flow rules and collects traffic statistics. The results show that SDN provides better visibility and control over network behavior.