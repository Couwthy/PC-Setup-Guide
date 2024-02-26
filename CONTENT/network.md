# Network Configuration

### Cable connections:

- The most common types of cables include UTP, FTP, STP, S/FTP, S/STP, as well as cat5, cat5e, cat6, cat6a, cat7 and cat8 standards. The ideal and most expensive choice is to use a cat8 shielded cable (STP) with a length of up to 50 cm or less. In case of a limited budget (and low Internet speed), it is recommended to pay attention to cat5e or cat6 shielded cables (STP or S/STP). This will provide a more stable connection to the network and image No. 1

### Important facts (which few people know about):

- It costs about $5 to manufacture all network adapters in China. Changing your traffic provider from a cyclic one to a more delay-sensitive one can lead to an increase in connection speed up to ± 500 times. Many providers use package aggregation, which allows them to increase download speeds by combining multiple packages into one. Some network cards, such as Solarflare, have a delay time.

### Choose a network adapter:

- If you have a Realtek adapter installed, you may encounter problems, while Intel adapters usually provide reliable performance. The preferred option is to use built-in network adapters from Intel or external adapters of the same brand. Remember to periodically update the drivers for your network adapter (LAN/WI-FI) by downloading them from the motherboard manufacturer's official website.

### A bit of theory:

- Internet speed is defined as the number of bits of information transmitted per second, measured in kilobits per second (Kbps), megabits per second (Mbps), or gigabits per second (Gbps). You can perform an [Internet speed test](http://www.dslreports.com/speedtest).

- Packet loss occurs when one or more packets do not reach their destination address during data transmission. You can perform a [packet loss test](https://packetlosstest.com).

- Excessive network buffering can result in increased latency and jitter, as well as reduced throughput. You can perform a test for excessive [network buffering](https://www.waveform.com/tools/bufferbloat).

### Network Adapter Settings


- Offloading features in network cards delegate specific packet handling functions, reducing CPU consumption. This ideally allocates more CPU time for other tasks and gaming activities.

### Settings for Intel Recommendations:

- **Adaptive Inter-Frame Spacing: Recommended to be disabled.**

- **Flow Control: Recommended to be disabled, but enabling it may benefit if link partners support flow control frames.**

- **Interrupt Moderation and Moderation Rate: Personal recommendation is to set it to Medium or leave it on Adaptive (default). Medium values provide acceptable latency during various network scenarios.**

- **IPv4 Checksum Offload: Recommended to be enabled for both RX and TX.**

- **Jumbo Packet: Recommended to be disabled.**

- **Large Send Offload V2 (IPv4 and IPv6): Recommended to be disabled.**

- **Receive Side Scaling: Recommended to be enabled.**

- **Maximum Number of RSS Queues: Use 2 or more queues when available.**

- **Packet Priority & VLAN: Both recommended to be enabled.**

- **Receive Buffers: Increase if extra memory is available, with a recommended value of 1024 or higher.**

- **Transmit Buffers: Similar to receive buffers, increase if extra memory is available, with a recommended value of 1024 or higher.**

- **TCP Checksum Offload (IPv4 and IPv6): Both recommended to be enabled.**

- **UDP Checksum Offload (IPv4 and IPv6): Both recommended to be enabled.**

- **Power Saving Options: Disable all power-saving options in drivers and for the adapter.**

- **These recommendations aim to optimize network performance and reduce latency. For further details and explanations, refer to Intel's and Microsoft's network subsystem performance tuning support guides, available in the Technical References section.**

### Settings for Realtek Recommendations:

- **Large Send Offload V2 (IPv6): Recommended to be disabled.**

- **Large Send Offload V2 (IPv4): Recommended to be disabled.**

- **Jumbo Packet: Recommended to be disabled.**

- **Flow Control: Recommended to be disabled.**

- **Adaptive Inter-Frame Spacing: Recommended to be disabled.**

- **Power Saving Options: Disable all power-saving options in drivers and for the adapter.**

### Operating System Specific Configuration

- Make sure the Network Throttling Index feature is enabled. Recommendation: Set the value between 10 and 20 decimal places, for example, 15 Mbps to 30 Mbps.
```HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Multimedia\SystemProfile\NetworkThrottlingIndex``` 
For more information about Network Throttling Index and its effect on NDIS DPC processing latency, see the study on [Network Throttling Index](../../RESEARCH/NETWORK/README.md#networkthrottlingindex).

### Tips

- Optimize the performance of your system using the best available CPU, RAM and GPU components. Perform a quality overclocking of these components, taking into account the speed of the CPU and RAM, as well as RAM timings and CPU cache size. These parameters directly affect system latency, which can impact hit-reg performance in game scenarios.

- If possible, consider removing the router from the network chain. Connect the network cable directly, bypassing the router. This may result in a slight decrease in ping by 1-3 milliseconds.
