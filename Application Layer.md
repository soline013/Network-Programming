# Application Layer

---

## Some Network Apps

- e-mail
- web
- text messaging
- remote login
- P2P file sharing
- multi-user network games
- streaming stored video(YouTube, Netflix)
- voice over IP (e.g. Skype)
- real-time video conferencing

## Application Architectures

1. client-server
    1. server
        - always-on host
        - permanent IP address
        
    2. clinets
        - communicate with server
        - may be intermittently connected
        - may have dynamic IP addresses
        - do not communicate directly with each other
    
2. peer-to-peer(P2P)
    1. No always-on server
    2. Peers request service from other peers, provide service in return to other peers
    3. Peers are intermittently connected and change IP addresses

## Processes Communicating

Process: program running within a host

- within same host, two processes communicate using inter-process communication(IPC)(defined by OS)
- 살아있는 프로그램 → Process

## Sockets

- Process sends/receives messages to/from its socket
- Socket analogous to door
- Socket → 함수
- operating system 부분에 대한 이해가 깊지 않아도 Socket 프로그래밍으로 내부 프로그램끼리 통신이 가능하다.

## Addressing processes

- Identifier includes both IP address and port number
- example port numbers
    - HTTP server: 80
    - mail server: 25

## App-layer protocal defines

1. Types of messages exchanged
    - e.g. request, response

1. Message syntax
    - What fields in messages, how fields are delineated

1. Message semantics
    - Meaning of information in fields

1. Rules for when and how processes send & respond to messages

1. open protocol
    - defined in RFCs
    - e.g. HTTP, SMTP

## What transport service does an app need?

1. Reliable data transfer
    - some apps(e.g. file transfer, web transactions) require 100% reliabel data transfer
    - other apps(e.g. audio) can tolerate some loss
    
2. Timing
    - some apps(e.g. Internet telephony, interactive games) require low delay to be "effective"
    
3. Throughput
    - some apps(e.g., multimedia) require minimum amount of throughput to be “effective” → bandwidth-sensitive applications
    - other apps(“elastic apps”) make use of whatever throughput they get → Electronic mail, file transfer, and Web transfers are all elastic applications.

1. Security
    - Encryption(암호화), Integrity(무결성), Availability(가용성)

## Transport service requirements: common apps

![스크린샷 2021-10-01 20.16.37.png](Application%20Layer%20cc45bf5a161e407b8dbcb963401fce2c/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA_2021-10-01_20.16.37.png)

## Internet transport protocols services

1. TCP
2. UDP