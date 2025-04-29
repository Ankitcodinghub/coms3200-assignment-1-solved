# coms3200-assignment-1-solved
**TO GET THIS SOLUTION VISIT:** [COMS3200 Assignment 1 Solved](https://www.ankitcodinghub.com/product/coms3200-assignment-1-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;116301&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMS3200 Assignment 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (1 vote)    </div>
    </div>
A client requests a webpage from a remote server on a remote island via a slow satellite link above the earth in geostationary orbit.

The goal of this exercise is to use the following information to calculate the time for the request to be completed. The scenario is in no way intended to be realistic.

There is a client (C), a server (V), and a DNS server (D). These are connected by three switches (S1, S2, S3) and five transmission links (L1 to L5). L2 is the satellite link. The following tables provide further information about the network (bps == bits per second, 1 kbps == 103 bps, 1 Mbps == 106 bps).

Transmission Links

Link Name Connected to Connected to Transmission Rate Length Propogation Speed

L1 C S1 100Mbps 150m 2 × 108 m/s

L2 S1 S2 5kbps 36,000km 3 × 108 m/s

L3 S2 V 100Mbps 150m 2 × 108 m/s

L4 S1 S3 100Mbps 6,000km 2 × 108 m/s

L5 S3 D 100Mbps 150m 2 × 108 m/s

Switches

Switch Links on Ports Processing Delay

S1 L1, L2, L4 500µs

S2 L2, L3 1ms

S3 L4, L5 500µs

Assumptions

• The network is packet-switched

• The network starts with no other packets in queues – only packets that are a part of this question

• Each link is bidirectional and can concurrently handle bits travelling in opposite directions

• All required records are stored in the DNS server

• C, D, and V have no processing delays (while this is unrealistic, this simplifies calculations)

• DNS packets and TCP SYN, ACK, FIN, SYN/ACK, and FIN/ACK packets are 100 bytes long, including all headers, preamble, etc

• HTTP GET and HTTP response packets are 1000 bytes long, including all headers, preamble, etc

Scenario

At time t = 0, a program on the client (C), starts the process of retrieving a webpage from the server (V). The following events happen sequentially:

1. C sends a DNS request to D

2. D sends a response with V’s IP address to C

3. C sends a TCP request (SYN) to open a connection to V

4. V acknowledges (SYN/ACK) the TCP request and opens the connections

5. C sends a HTTP GET request to V (which includes the ACK back to V for its SYN)

6. V sends the web page to C, which requires 5 packets, which includes the HTTP response plus the HTML file.

7. After receiving each data packet, C sends an ACK message back to V. Note that V does not need to wait foran ACK before sending the next data packet.

8. After receiving the last data packet acknowledgement, V sends a TCP FIN packet to close the connection.

9. After receiving FIN, C sends one FIN/ACK packet back to V.

10. After receiving FIN/ACK, V sends a final ACK packet back to C.

11. When this final ACK packet is received at C, the connection is finally closed.

Questions

Answer each of the following questions in the associated quiz on blackboard, following the specified instructions. All answers should be in milliseconds (ms) rounded to at least four decimal places.

HINT: Make sure you correctly convert between units

This question requires you to analyse the Wireshark file Assignment1.pcapng. This packet capture shows a client connecting to an email server from their home PC.

You will need to read the relevant IETF RFCs for the application level protocols used in this trace to answer some of these questions.

The first six questions relate to the message being sent:

1. What application layer protocol is used to send the email message?

2. What is the IP address and port number of the mail client?

3. What is the IP address and port number of the mail server?

4. What mail client is the sender using?

5. What is the first line of the body of the message? Omit any ASCII characters with a decimal value less than32 or greater than 126.

6. What is the maximum message size (in bytes) that the mail server will accept?

The following questions relate to the message being received:

7. What application layer protocol is used to read the email message from the server?

8. What is the username and password that is used to login to the server?

9. How many packets are used to transmit the body of the message that is being received?

10. What is the size (in bytes) of the first email in the in the maildrop? (i.e. the message with ID 1)

Your task for this part is to write a program to retrieve a file on a webserver via HTTP. Your program should make use of sockets to send and receive HTTP requests/responses and must be written in Python, Java, C, or C++. It is recommended that you use Python as more support will be available for it in this course.

Description

Your program should take a HTTP URL as a command line input, leading to a file on a webserver. This URL could just be a domain name (eg. http://www.my.server.com) or include the resource location

(eg. http://www.my.server.com/about or http://www.my.server.com/file.json). The exact method of program invocation is described later.

Your program should open a TCP connection to the webserver and print the following information to stdout:

URL Requested: [url]

Client: [client-ip-addr] [client-port-num]

Server: [server-ip-addr] [server-port-num]

You do not need to handle invalid domains. Upon successful connection, your program should make a HTTP request to the server. After receiving the associated response, the following information should then be printed:

Retrieval Successful

Last Modified: [dd/mm/yyyy] [hh:mm:ss] AEST

The contents of the file retrieved from the webserver should be written to a file named “output.[extension]”. [extension] should be replaced with an appropriate extension based on the MIME type of the retrieved file. You only have to support the MIME types given in the table below. You can read more about MIME types at https://tools.ietf.org/html/rfc6838. Note that the extension of the URL is not always indicative of a file’s MIME type, you will need to retrieve this from the HTTP response.

Supported MIME Types

MIME Type File Extension

text/plain .txt

text/html .html

text/css .css

text/javascript or application/javascript .js

application/json .json

application/octet-stream No extension

Your program does not need to work for HTTPS URLs. If a HTTPS URL is requested your program should print the following and terminate:

URL Requested: [url]

HTTPS Not Supported

If the status code of a HTTP response is in the range of 400-599, your program should notify the user of this and terminate, as follows:

URL Requested: [url]

Client: [client-ip-addr] [client-port-num]

Server: [server-ip-addr] [server-port-num]

Retrieval Failed ([code])

The final feature your program should support is handling of 301 and 302 status codes. If a resource has been moved, you should repeat the above process until either the resource is found, or an invalid/unsupported URL is given. For example:

URL Requested: [url]

Client: [client-ip-addr] [client-port-num]

Server: [server-ip-addr] [server-port-num]

Resource [temporarily/permanently] moved to [url]

Client: [client-ip-addr] [client-port-num]

Server: [server-ip-addr] [server-port-num]

Retrieval Successful

Last Modified: [dd/mm/yyyy] [hh:mm:ss] AEST

Program Invocation

Your program should be able to be invoked from a UNIX command line as follows. url is the URL of the webpage to request.

Python python3 assign1.py url

C/C++

make

./assign1 url

Java

make java Assign1 url

Example Output

The following is an example output for a request to http://uq.edu.au/:

URL Requested: http://uq.edu.au/

Client: 192.168.12.15 54321

Server: 10.187.2.85 80

Retrieval Successful

In this case, the user should be able to view the contents of this webpage in a file named “output.html”.

An example for a request to http://uq.edu.au/missing is below:

URL Requested: http://uq.edu.au/missing

Client: 192.168.12.15 54321

Server: 10.187.2.85 80

Retrieval Failed (404)

An example for a request to http://abc.net.au/ is below:

URL Requested: http://abc.net.au/

Client: 192.168.12.15 54321

Server: 10.187.2.85 80

Resource permanently moved to http://www.abc.net.au/

Client: 192.168.12.15 54321

Server: 10.187.2.85 80

Resource temporarily moved to https://www.abc.net.au/

HTTPS Not Supported

Library Restrictions

• You should use standard socket libraries to open the TCP connection and communicate between the client and server

• You should NOT use higher level libraries, packages, or programs which retrieve data from HTTP servers, such as the python requests and urllib libraries.

Submission

Submit all files necessary to run your program. At a minimum, you should submit a file named assign1.py, assign1.c, assign1.cpp or Assign1.java. If you submit a C or Java program, you should also submit a makefile to compile your code into a binary named assign1 or a .class file named Assign1.class.

Marking

Academic Misconduct

Version History

v1.0

• Released assignment

v1.1 (11/03/19)

Fixes:

• Added missing port to S1 in part A

• Added missing “Retrieval Successful” to redirection example

Clarifications:

• Reworded part B Q9

• Clarified spacing between words in part C output Additions:

• Added C++ as one of the allowed languages for part C v1.2 (14/03/19)

Additions:

• Changed the URL for the abc example to include a trailing slash

• Redirection now requires the client/server info to be re-printed

v1.3 (21/03/19)

Fixes:

• Fixed inconsistency between redirection outputs
