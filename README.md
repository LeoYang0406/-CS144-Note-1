# TCP/IP

### 4 layers of Internet:
    Application Layer, Transport Layer, Internet Layer and Network Access Layer
    Transport layer: TCP - Transmission control protocol
    Network layer:  to deliver packets from end to end acrossing the Internet from the sources to the destination
    Link layer: to carry data one link at a time (Ethernet & WiFi)
    
    the network layer hands in the datagram
    the link layer helps it to transmit the datagram over one link (可以理解为link层为network层提供service)
    
### TCP/IP的关系:
    TCP是transport layer的transmission control protocol
    IP是Internet protocol
    因为Internet protocol不保证datagram以及传输的完整性
    所以要用到TCP above the head of IP，来保证得到correct and in-order data
    TCP: make sure the data sent by one appliation to another is correctly delivered in right order.
    
    对于不需要保证数据完整性和顺序的应用，可以用UDP(user datagram protocol) instead of TCP
    
### How they collaborate:
    
    总的来说 application layer所代表的一系列应用，比如Skype，communicate directly to its peer layer on the other end of the Internet
    transport layer负责把data reliably(or not) deliver到另一端
    Network layer负责把data分成packets，并带上correct destination address
    Link layer负责把packets从一个hop deliver 到下一个along its path
    
    
### Reuse:
