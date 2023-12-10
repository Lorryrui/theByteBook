# Linux 网络虚拟化

虚拟化容器是以 Linux 名称空间的隔离性为基础来实现的，那解决隔离的容器之间、容器与宿主机之间、乃至跨物理网络的不同容器间通信问题的责任，很自然也落在了 Linux 网络虚拟化技术的肩上。

Linux 网络虚拟化的主要技术是 Network Namespace，以及各类虚拟设备，例如 Veth、Linux Bridge、tap/tun 等，虚拟化的本质是现实世界的映射，这些虚拟设备像现实世界中的物理设备一样彼此协作，将各个独立的 namespace 连接起来，构建出不受物理环境局限的各类网络拓扑架构。
