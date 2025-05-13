# cse310-program-2-analyzing-packet-traces-pcap-solved
**TO GET THIS SOLUTION VISIT:** [CSE310 Program 2-Analyzing packet traces (PCAP Solved](https://www.ankitcodinghub.com/product/cse310-program-2-analyzing-packet-traces-pcap-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;93852&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE310 Program 2-Analyzing packet traces (PCAP Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
&nbsp;

The goal of this assignment is to dissect TCP packets. To do this, you should be familiar with the packet formats (PCAP files).

Specifically, your goal is to parse a PCAP file. PCAP is the file format used to store packets captured on the wire. PCAP files are in binary format and cannot be read directly. A PCAP library is used to parse the binary packet. Your goal is to write a parser that analyzes the packet with the help of the PCAP library.

TCPdump is the command-line tool that also analyzes the packets captured on the wire. Wireshark is the graphical version of TCPDump. You can check out these tools to see some examples of packet analysis if you want.

Part A PCAP Programming Task and flow-level information (70 points)

Your task is to write a program analysis_pcap_tcp that analyzes a PCAP file to characterize the TCP flows in the trace. A TCP flow starts with a TCP “SYN” and ends at a TCP “FIN” between two hosts. A TCP flow is uniquely identified by the tuple: (source port, source IP address, destination port, destination IP address). There can be multiple TCP flows at the same time between the two hosts, on different ports.

You can use a PCAP library to analyze this file. Example PCAP libraries are provided in the end of this assignment. A PCAP library helps convert a PCAP packet from binary to byte format. You need to then write code to analyze the bytes to get the information about the packet.

[Important: You can create your own packet structures and read the bytes into the structure. This will let you easily parse the bytes rather than doing byte operations. You can also use the ethernet and TCP modules in the PCAP library to get these packets. However, you cannot convert the PCAP file into text for analysis.]

Specifically, we have captured packets that are going on the wire—both packets from the computer and to the computer. This packet capture is in PCAP format and called assignment2.pcap in the resource section. In this file, we have captured packets sent between 130.245.145.12 and 128.208.2.198. Node 130.245.145.12 establishes the connection (let’s call it sender) with 128.208.2.198 (let’s call is receiver) and then sends data. The trace was captured at the sender.

Your “ analysis_pcap_tcp” code should take as input any pcap file (but specifically should work with assignment2.pcap). You can hardcode the sender and receiver IP addresses in your code. Your code should output the answers to these questions (Ignore non-TCP traffic):

• The number of TCP flows initiated from the sender. A TCP flow starts with a SYN and ends with a FIN, and a TCP flow is identified by a (source port, source IP address, destination port, destination IP address). A sender can initiate multiple TCP flows at the same time.

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
• For each TCP flow

(a) Write down the (source port, source IP address, destination port, destination IP address)

(b) For the first two transaction after the TCP connection is set up (from sender to receiver), the values of the Sequence number, Ack number, and Receive Window size. In the figure below, the first two transactions are marked in orange. If there is a packet loss, this illustration should still work. If the last ACK in the three-way handshake is piggy-backed with the first packet (in orange), then you should still start with this piggy-backed packet.

(c) The sender throughput. The throughput is the total amount of data sent by the sender. The period is the time between sending the first byte to receiving the last acknowledgement. For throughput, only consider the packets at the TCP level (including the header). You can ignore all other headers and acks.

This is only an example, your flow may look different

</div>
</div>
<div class="layoutArea">
<div class="column">
Sender Node 130.245.145.12

</div>
<div class="column">
Receiver Node 128.208.2.198

</div>
</div>
<div class="layoutArea">
<div class="column">
SYN

SYN/AC K

ACK

</div>
</div>
<div class="layoutArea">
<div class="column">
cwnd=icwnd

</div>
</div>
<div class="layoutArea">
<div class="column">
Part B Congestion control (30 points)

</div>
</div>
<div class="layoutArea">
<div class="column">
Now extend your program so that it will output the following answer to the questions. For each TCP flow:

(1) Print the first 3 congestion window sizes (or till the end of the flow, if there are less than 3 congestion windows). The congestion window is estimated at the sender. You need to estimate the congestion window size empirically since the information is not available in the packet. Comment on how the congestion window size grows. Remember that your estimation may not be perfect, but that is ok. Congestion window sizes at roughly RTT-intervals.

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
(2) The number of times a retransmission occurred due to triple duplicate ack and the number of time a retransmission occurred due to timeout.

</div>
</div>
</div>
