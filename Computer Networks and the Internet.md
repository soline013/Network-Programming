# Computer Networks and the Internet.

## A closer look at network structure

1. Network Edge(종단 시스템)
    
    Hosts: Clients and Servers
    
    `호스트, 서버와 클라이언트`
    
    `Edge Computing: 유효 통신 인프라를 활용하는 서비스`
    
2. Access Networks
    
    Home, Enterprise, Mobile, ...
    
    `인터넷을 제공할 수 있는 포인트`
    
3. Physical Media
    
    Wired, Wireless Communication Links
    

## Home Access

1. DSL(Digital Subscriber Line)
    
    ![스크린샷 2021-10-21 00.57.45.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/10c1b28e-87c8-4f0f-b12f-9198909ac9b0/스크린샷_2021-10-21_00.57.45.png)
    
2. Cable Internet Access, HFC(Hybrid Fiber Coax)
    
    `광섬유와 구리 케이블을 같이 사용한다.`
    
    ![스크린샷 2021-10-21 00.58.02.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/42f28d9b-2adf-4b1e-8bfd-aa81d09f97a6/스크린샷_2021-10-21_00.58.02.png)
    
3. FTTH(Fiber to the home)
    
    `광섬유를 사용한다. 중계기가 필요하다.`
    
    ![스크린샷 2021-10-21 00.58.28.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/df83bf58-8f0c-442a-a287-8de91fbae784/스크린샷_2021-10-21_00.58.28.png)
    
4. A typical home network
    
    ![스크린샷 2021-10-21 01.01.34.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/80d7b7ee-a26e-43c0-956f-903bda0514c8/스크린샷_2021-10-21_01.01.34.png)
    
5. Ethernet
    
    ![스크린샷 2021-10-21 01.01.55.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9368d3af-baff-45e5-9aaa-cbaeb2e87b8b/스크린샷_2021-10-21_01.01.55.png)
    

## Physical media

`물리적인 신호로 보낼 수 있는 선(유도매체)이나, 라디오와 다른 무선(비유도매체)`

1. Twisted-Pair Copper Wire
    
    ![스크린샷 2021-10-21 01.08.32.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/40702a3b-3568-4dc7-8959-d80af9c12d2a/스크린샷_2021-10-21_01.08.32.png)
    
    - UTP(Unshielded twisted pair) → `일반적으로 보는 랜선`
    - 카테고리 5, 카테고리 6 등으로 나뉘어져 있다.
    
2. Appendix: UTP vs. STP
    
    ![스크린샷 2021-10-21 01.08.53.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8a5fce6d-e67c-4dd6-b33d-27eaa5bef502/스크린샷_2021-10-21_01.08.53.png)
    
    - UTP → `보호되지 않음.`
    - STP → `알루미늄으로 보호됨. 더 신뢰가 필요한 곳에 사용함.`
    
3. coax, fiber
    - Coaxial cable
        
        ![스크린샷 2021-10-21 01.09.21.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/3e56249e-3eaa-41ce-89ab-0bf279fdeeb4/스크린샷_2021-10-21_01.09.21.png)
        
    - Fiber Optics
        
        ![스크린샷 2021-10-21 01.09.37.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2853672b-93be-4647-9a3e-abddce3728c2/스크린샷_2021-10-21_01.09.37.png)
        
    
4. Radio

## The network core

![스크린샷 2021-10-21 01.09.56.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a15b7ffc-c758-4478-b18d-aa0a49812ad7/스크린샷_2021-10-21_01.09.56.png)

## Packet-switching

1. Each packet travels through communication links and packet switches (i.e., routers and link-layer switches)
2. Packet Transmission Delay
    1. sending a packet of L bits
    2. transmission rate R bits/sec
    3. Packet Transmission Delay = $\frac{L(bits)}{R(bits/sec)}$
    
3. Store-and-Forward
    
    ![스크린샷 2021-10-21 01.21.53.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a4cc6446-3d75-4d23-b872-d8787afd90ac/스크린샷_2021-10-21_01.21.53.png)
    
    ![스크린샷 2021-10-21 01.22.29.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/581e2160-2295-469d-9d41-2db4dbbe7d29/스크린샷_2021-10-21_01.22.29.png)
    
4. Queuing Delays and Packet Loss
    
    ![스크린샷 2021-10-21 01.23.24.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/27a95324-b982-4526-8101-c98471120dd6/스크린샷_2021-10-21_01.23.24.png)
    
    - packets can be dropped(lost) if memory(buffer) fills up.
    
5. Forwarding and Routing
    - Forwarding: `A에서 B로 움직이는 것.`
    - Routing: `라우팅 알고리즘에 따라 어디로 갈지 방향을 정해주는 것.`

## Circuit switching

- In circuit switched networks, the resources are reserved...
    - In packet-switched networks, these resources are not reserved.

1. FDM(frequency-division multiplexing)
    
    ![스크린샷 2021-10-21 01.33.55.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2f167ad0-1986-4ba2-825f-6e4a006d5754/스크린샷_2021-10-21_01.33.55.png)
    
    ![스크린샷 2021-10-21 01.35.27.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/75f5aa25-a56b-4dfd-b41a-c57db9a6f027/스크린샷_2021-10-21_01.35.27.png)
    
2. TDM(time-division multiplexing)
    
    ![스크린샷 2021-10-21 01.34.13.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/537bf250-c3ec-46c9-81eb-bd876458c978/스크린샷_2021-10-21_01.34.13.png)
    
3. Silent Period가 네트워크의 자원 낭비로 이어진다.

## Packet Switching vs. Circuit Switching

![스크린샷 2021-10-21 01.37.31.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/deb8eb46-6d7b-4014-93ef-85bd3ed59a51/스크린샷_2021-10-21_01.37.31.png)

- Excessive Congestion Possible: Packet Delay and Loss.

## Network of networks

- End systems connect to Internet via access ISPs(Internet Service Providers)
- Access ISPs in turn must be interconnected.

![스크린샷 2021-10-21 01.40.35.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b73c951a-fd3d-4019-a847-542f7d2cf8eb/스크린샷_2021-10-21_01.40.35.png)

![스크린샷 2021-10-21 01.40.50.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c4fe6648-cd76-48cd-b95d-ba37f432c1c7/스크린샷_2021-10-21_01.40.50.png)

![스크린샷 2021-10-21 01.41.03.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/01c6bb0e-011b-4927-b2a5-05f919307050/스크린샷_2021-10-21_01.41.03.png)

![스크린샷 2021-10-21 01.41.19.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/83cf91e4-9ed2-4113-b2ff-989e03a3132b/스크린샷_2021-10-21_01.41.19.png)

![스크린샷 2021-10-21 01.41.43.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4aedea5b-e5d9-4027-85e4-531e845eef45/스크린샷_2021-10-21_01.41.43.png)

![스크린샷 2021-10-21 01.41.55.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a5a72a8e-df44-4d7d-866f-e0ba52c6956d/스크린샷_2021-10-21_01.41.55.png)

![스크린샷 2021-10-21 01.42.13.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/68e92b98-6381-4d1b-a38c-934e9754167c/스크린샷_2021-10-21_01.42.13.png)

![스크린샷 2021-10-21 01.42.29.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/418c7878-51cc-424d-aa5e-d1050d71b724/스크린샷_2021-10-21_01.42.29.png)

## Four sources of packet delay

- Total nodal delay($d_{nodal}$)
    
    ![스크린샷 2021-10-21 16.14.14.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/419ff7d1-5ff3-477f-887e-86cab09f7075/스크린샷_2021-10-21_16.14.14.png)
    
    $$d_{nodal} = d_{proc} + d_{queue} + d_{trans} + d_{prop}$$
    
    1. nodal processing delay($d_{proc}$)
        - check bit errors
        - determine output link
        - typically < msec
        
    2. queuing delay($d_{queue}$)
        - time waiting at output link for transmission
        - depends on congestion level of router
        - `가장 중요한 부분이 되었다.`
        - L: packet length (bits)
        - R: link bandwidth (bps)
        - a: average packet arrival rate (packets/sec)
        - La/R: traffic intensity (assuming infinite queue size)
            
            ![스크린샷 2021-10-21 16.21.36.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/892c3b5d-8a7e-4ec3-b5da-083f52df5fda/스크린샷_2021-10-21_16.21.36.png)
            
        
    3. transmission delay($d_{trans}$)
        - L: packet length (bits)
        - R: link bandwidth (bps)
        - $d_{trans}$ = L/R
        
    4. propagation delay($d_{prop}$)
        - d: length of physical link
        - s: propagation speed (통신 매체에 따라 달라짐)
        - $d_{prop}$ = d/s
    

## End-to-End Delay

- the total delay from source to destination.
- N-1 Routers.
- Queuing Delays are negligible.
- End-to-End Delay: $N \times (d_{proc} + d_{trans} + d_{prop})$

## Throughput

- rate (bits/time unit) that bits transferred between sender/receiver
- bottleneck link: link on end-end path that constrains end-end throughput

![스크린샷 2021-10-21 16.27.11.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b035a38d-cd4c-4137-8406-52f10ed2eb2c/스크린샷_2021-10-21_16.27.11.png)

## Network security

1. Put malware into hosts via Internet
    1. virus: self-replicating infection by receiving/executing object. (e.g., e-mail
    attachment)
    2. worm: self-replicating infection by passively receiving object that gets itself executed.
    3. spyware: malware can record keystrokes, web sites visited, upload info to collection site.
    4. botnet: infected host can be enrolled in botnet
    
2. Attack server, network infrastructure
    1. DoS(Denial of Service)
    2. DDoS(Distribute Denial of Service)
    3. attackers make resources unavailable.
    
3. Sniffing
    - packet sniffing: `다른 목적지인 패킷을 도청하여 읽고 저장한다.`
    
    ![스크린샷 2021-10-21 16.36.16.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4fb66b56-0832-4bc9-b526-8504a8f2b734/스크린샷_2021-10-21_16.36.16.png)
    
4. IP spoofing
    - send packet with false source address.
    - `IP를 속여서 패킷을 보낸다.`
    
    ![스크린샷 2021-10-21 16.36.31.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/05d677c6-2b6e-4ca1-9b75-28692091589f/스크린샷_2021-10-21_16.36.31.png)