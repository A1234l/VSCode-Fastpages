---
toc: true
comments: true
layout: post
title: Computers and Networks (Unit 4)
description: Add Definitions from Unit 4 Computer Systems and Networks
image: /images/Scammer.png
categories: [week29]
type: ap
week: 29
---

## Requirements
> Work through College Board Unit 4... blog, add definitions, and pictures.  Be creative, for instance make a story of Computing and Networks that is related to your PBL experiences this year.


### How a Computer Works
> As we have learned, a computer needs aa program to do something smart.  The sequence of a program initiates a series of actions with the computers Central Processing Unit (CPU). This component is essentially a binary machine focussing on program instructions provided. The CPU retrieves and stores the data it acts upon in Random Access Memory (RAM). Between the CPU, RAM, and Storage Devices a computer can work with many programs and large amounts of data.

List specification of your Computer, or Computers if working as Pair/Trio
- Processor GHz: 
    - Tirth - i7-12700H, 2.30 Ghz Base, 4.7 Boost 
    - Yuri - Ryzen 5900 3.7 Ghz Base, 4.8 Boost 
    - Alan - i7-1065G7, 1.3 Ghz Base, 1.5 Boost  
    - Jishnu - i5-11320H, 2.5 GHz Base, 3.2 Boost
    - Haoxion - i5-8365U, 1.6 GHz Base, 1.90 Boost
- Memory in GB:
    - Tirth - 16 GB 
    - Yuri - 64 GB
    - Alan - 16 GB
    - Jishnu - 16 Gb
    - Haoxion - 16 GB
- Storage in GB:
    - Tirth - 1024 TB SSD
    - Yuri - 2048 TB SSD, 128 Gb SSD
    - Alan - 512 GB SSD
    - Jishnu - 512 GB SSD
    - Haoxion - 475 GB SSD
- OS:
    - Tirth - Windows 11
    - Yuri - Windows 10
    - Alan - Windows 10
    - Jishnu - Windows 11

Define or describe usage of Computer using Computer Programs. Pictures are preferred over a lot of text.  Use your experience.
- Input devices
- Output devices
- Program File
- Program Code
- Processes
- Ports
- Data File
- Inspect Running Code
- Inspect Variables


![Computer Hardware](https://github.com/Tirth-Thakkar/APCSP-Blog/blob/master/images/Computing1.png?raw=true)
![Computer Hardware](https://github.com/Tirth-Thakkar/APCSP-Blog/blob/master/images/Computing2.png?raw=true)
![Computer Hardware](https://github.com/Tirth-Thakkar/APCSP-Blog/blob/master/images/Computing3.png?raw=true)

### The Internet
> Watch/review College Board Daily Video for 4.1.1

- Essential Knowledge
    - A computing device is a physical artifact that can run a program. Some examples include computers, tablets, servers, routers, and smart sensors.
    - A computing system is a group of computing devices and programs working together for a common purpose.
    - A computer network is a group of interconnected computing devices capable of sending or receiving data.
    - A computer network is a type of computing system. 
    - A path between two computing devices on a computer network (a sender and a receiver) is a sequence of directly connected computing devices that begins at the sender and ends at the receiver.
    - Routing is the process of finding a path from sender to receiver.
    - The bandwidth of a computer network is the maximum amount of data that can be sent in a fixed amount of time.
    - Bandwidth is usually measured in bits per second

- Complete Vocabulary Matching Activity.  Incorporate this into your learnings from year.  To analyze measure path and latency use `traceroute` and `ping` commands from Linux Terminal.  
    - Path - a
    - Route - e
    - Computer System - b
    - Computer Device - c
    - Bandwidth - d
    - Computer Network - f

> Watch/review College Board Daily Video 4.1.2

- Complete True of False Questions
    1. True, open protocols allow for more unrestricted sharing to the rest of the internet.
    2. False, IETF sets up the rules of the internet but does not keep manufacturers out from the internet. The internet is a thing where all people can access it.
    3. False, different routes can be undertaken depending on if a MAC is available for transfer or not. While the file is being transferred it determines which MACs are available or not.
    4. True, things like Internet Protocol and other protocols are agreed upon rules that set up specific behaviors in the system.
    5. False, UDP guarantees faster transfers but does not guarantee consistent transfer success.
    6. False, the World Wide Web is not the internet. WWW links pages instead.
    7. True, HTTP is used by World Wide Web to display website pages.



- Essential Knowledge
    - The internet is a computer network consisting of interconnected networks that use standardized, open (nonproprietary) communication protocols.
    - Access to the internet depends on the ability to connect a computing device to an internet connected device.
    - A protocol is an agreed-upon set of rules that specify the behavior of a system.
    - The protocols used in the internet are open, which allows users to easily connect additional computing devices to the internet.
    - Routing on the internet is usually dynamic; it is not specified in advance
    - The scalability of a system is the capacity for the system to change in size and scale to meet new demands.
    - The internet was designed to be scalable
    - Information is passed through the internet as a data stream. Data streams contain chunks of data, which are encapsulated in packets. 
    - Packets contain a chunk of data and metadata used for routing the packet between the origin and the destination on the internet, as well as for data reassembly.
    - Packets may arrive at the destination in order, out of order, or not at all
    - IP, TCP and UDP are common protocols used on the internet.
    - The world wide web is a system of linked pages, programs, and files.
    - HTTP is a protocol used by the world wide web
    - The world wide web uses the internet

- Go over AP videos, vocabulary, and essential knowledge.  Draw a diagram showing the internet and its many levels. A preferred diagram would using your knowledge of frontend, backend, deployment, etc.  Picture would highlight vocabulary by illustration. The below illustration have some ideas


![Full Stack](https://github.com/Tirth-Thakkar/APCSP-Blog/blob/master/images/FullStack.png?raw=true)


- Often we draw pictures of machines communicating over the Internet with arrows.  However, the real communication goes through protocol layers and the machine and then is transported of the network.   For College Board and future Computer Knowledge you should become familiar with the following ...

```
     User Machine  <---> Frontend Server <---> Backend Server
    +-----------+         +-----------+         +-----------+
    |  Browser  |         |  GH Page  |         |   Flask   |
    +-----------+    ^    +-----------+    ^    +-----------+
    |    HTTP   |    |    |    HTTP   |    |    |    HTTP   |
    +-----------+    |    +-----------+    |    +-----------+
    |    TCP    |    |    |    TCP    |    |    |    TCP    |   
    +-----------+    |    +-----------+    |    +-----------+
    |     IP    |    V    |     IP    |    V    |     IP    |
    +-----------+         +-----------+         +-----------+
    |  Network  |  <--->  |  Network  |  <--->  |  Network  |
    +-----------+         +-----------+         +-----------+
```

The "http" layer is an application layer protocol in the TCP/IP stack, used for ***communication between web browsers and web servers***. It is the protocol used for transmitting data over the World Wide Web.

The "transport" layer (TCP) is responsible for providing reliable data transfer between applications running on different hosts.  The TCP protocol segments the data into smaller ***chunks called "segments"***. Each segment contains a sequence number that identifies its position in the original stream of data, as well as other control information such as source and destination port numbers, and checksums for error detection.

The "ip" layer is responsible for packeting data received from the TCP layer of the protocol stack, and then ***encapsulating the data into IP packets***. The IP packets are then sent to the lower layers of the protocol stack for transmission over the network.

The "network" layer is responsible for ***routing data packets between networks*** using the Internet Protocol (IP). This layer handles tasks such as packet addressing and routing, fragmentation and reassembly, and ***network congestion*** control.


### Fault Tolerance
> Watch both Daily videos for 4.2

- Complete the network activity, summarize your understanding of fault tolerance.
    - i. Yes the network is fault tolerant, as if any link or any points is broken the information can still be distributed to other points in the system.
    - ii. No the network is not fault tolerant, as if node C goes down, then information can’t be sent to F and thus it is not fault tolerant.
    - iii. No the network is not fault tolerant, as if node G comes down, then information can’t be sent to A and thus the system cannot be described as fault tolerant.
    1. Option C
    2. Option A  
    3. The importance of fault tolerance is that there is redundancy in your system and one faulty link doesn't compromise the entire system and information can still be transmitted throughout the entire system. The internet is an example of such a system as if one link is broken, the information can still be sent through other links while the broken link is being repaired. Thus it is vital to create fault tolerant systems with at least one backup link or node per connection in case of a failure.   

### Parallel and Distributed Computing
> Review previous lecture on Parallel Computing and watch Daily video 4.3.  Think of ways to make something in you team project to utilize Cores more effectively.  Here are some thoughts to add to your story of Computers and Networks...

- What is naturally Distributed in Frontend/Backend architecture?  
    - In a frontend/backend architecture, the frontend and backend are naturally distributed components. The frontend typically consists of the user interface and presentation layer, while the backend contains the business logic and data storage. The frontend is distributed across multiple devices or clients, such as web browsers, mobile devices, or desktop applications. Each client has its own instance of the frontend code, which communicates with the backend over a network connection. The backend is typically deployed on one or more servers or cloud platforms. The servers may be physically distributed across multiple locations, and the backend may be composed of multiple services or microservices that work together to provide the required functionality. The distributed nature of the frontend/backend architecture allows for scalability, fault tolerance, and performance optimization. The frontend can be scaled by adding more clients or instances, while the backend can be scaled by adding more servers or services. Fault tolerance can be achieved by replicating the backend across multiple servers or locations, and load balancing can be used to optimize performance by distributing the load across multiple servers. Overall, the frontend/backend architecture is a popular and effective way of building modern web applications that can handle large volumes of users and data.

- Analyze this command in Docker: ```ENV GUNICORN_CMD_ARGS="--workers=1 --bind=0.0.0.0:8086"```.   Determine if there is options are options in this command for parallel computing within the server that runs python/gunicorn.  Here is an [article](https://medium.com/building-the-system/gunicorn-3-means-of-concurrency-efbb547674b7)
    - ```The GUNICORN_CMD_ARGS environment variable is used to set command-line arguments for the Gunicorn web server when it starts up. In the provided command, --workers=1 and --bind=0.0.0.0:8086 are specified as arguments. To run the Gunicorn server in parallel, you can increase the number of worker processes to handle multiple requests simultaneously. To do this, simply set the --workers argument to a higher number. For example, if you want to run four worker processes, you can set the argument to --workers=4. It's important to note that the number of workers you can run at once will depend on the resources available on your system and the workload your application is handling. Be careful not to increase the number of workers beyond what your system can handle, as this can cause performance issues or even crashes. To make sure everything is running smoothly, it's a good idea to monitor the resource usage of the worker processes while the server is running with multiple workers. You can use tools like htop, top, or systemd to keep an eye on things. In summary, to run the Gunicorn server in parallel, set the --workers argument to a number that your system can handle, and keep an eye on the resource usage of the worker processes to ensure everything stays stable.``` 

> Last week we discussed parallel computing on local machine.  There are many options.  Here is something to get parallel computing work with a tool called Ray.
- Review this [article](https://www.anyscale.com/blog/writing-your-first-distributed-python-application-with-ray)...  Can you get parallel code on images to work more effectively?  I have not tried Ray.

- Code example from ChatGPT using squares.  This might be more interesting if nums we generated to be a lot bigger.

```python
import ray

# define a simple function that takes a number and returns its square
def square(x):
    return x * x

# initialize Ray
ray.init()

# create a remote function that squares a list of numbers in parallel
@ray.remote
def square_list(nums):
    return [square(num) for num in nums]

# define a list of numbers to square
nums = [1, 2, 3, 4, 5]

# split the list into two parts
split_idx = len(nums) // 2
part1, part2 = nums[:split_idx], nums[split_idx:]

# call the remote function in parallel on the two parts
part1_result = square_list.remote(part1)
part2_result = square_list.remote(part2)

# get the results and combine them
result = ray.get(part1_result) + ray.get(part2_result)

# print the result
print(result)

```
