- Data Proc 
    * Hadoop as service 
- VPC 
    * uses routing table to forward traffic from instance to other 
    * VPC routing tables are built in
    * VPC belongs to Project (meaning VPC cannot extend to different projects)
    * VPC provides global distributed firewall
        *  VPC Peering - Helps to exchange traffic between two different projects 
        * Shared VPCs - Controlling the who and what can be ve be accessed between the projects 
        * ***Layer 4 load balancing*** operates at the intermediate transport layer, which deals with delivery of messages with no regard to the content of the messages. Transmission Control Protocol (TCP) is the Layer 4 protocol for Hypertext Transfer Protocol (HTTP) traffic on the Internet. Layer 4 load balancers simply forward network packets to and from the upstream server without inspecting the content of the packets. They can make limited routing decisions by inspecting the first few packets in the TCP stream.

        * ***Layer 7 load balancing*** operates at the high-level application layer, which deals with the actual content of each message. HTTP is the predominant Layer 7 protocol for website traffic on the Internet. Layer 7 load balancers route network traffic in a much more sophisticated way than Layer 4 load balancers, particularly applicable to TCP-based traffic such as HTTP. A Layer 7 load balancer terminates the network traffic and reads the message within. It can make a load-balancing decision based on the content of the message (the URL or cookie, for example). It then makes a new TCP connection to the selected upstream server (or reuses an existing one, by means of HTTP keepalives) and writes the request to the server
   *https://freeloadbalancer.com/wp-content/uploads/2015/02/FreeLoadBalancerLayer4Layer7.jpg
