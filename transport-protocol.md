# Transport protocol

↑ **Parent:** [Layered network architecture](layered-network-architecture.md)

A [transport protocol](transport-protocol.md) provides communication services between its transport [endpoints](communication-endpoint.md) over an underlying network. [Transmission Control Protocol](transmission-control-protocol.md) supplies a reliable ordered byte stream; [User Datagram Protocol](user-datagram-protocol.md) supplies datagrams without that built-in recovery service. Applications can implement further mechanisms over either interface.

**Table of contents**

- [Flow control](flow-control.md)
  - [Backpressure](backpressure.md)
- [Sliding window protocol](sliding-window-protocol.md)
  - [Receive window](receive-window.md)
  - [Send window](send-window.md)
- [Acknowledgement](acknowledgement.md)
  - [Delayed acknowledgement](delayed-acknowledgement.md)
- [Transport sequence number](transport-sequence-number.md)
- [Retransmission (data networks)](retransmission-data-networks.md)
- [Transport port](transport-port.md)
- [QUIC](quic.md)
- [User Datagram Protocol](user-datagram-protocol.md)
- [Transmission Control Protocol](transmission-control-protocol.md)
  - [Zero-window probe](zero-window-probe.md)
    - [Persist timer](persist-timer.md)
  - [Silly window syndrome](silly-window-syndrome.md)
    - [Nagle's algorithm](nagle-s-algorithm.md)
  - [TCP segment](tcp-segment.md)

## ↑ Ancestors (4)

1. [Layered network architecture](layered-network-architecture.md)
2. [Computer network](computer-network-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Layered network architecture](layered-network-architecture.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computer-networks/2/b/solution.md)
- [Solution](past-exam-of-the-internet-technologies-and-regulation-course-of-the-university-of-oxford/2019/1/solution.md)
- [Solution](past-exam-of-the-internet-technologies-and-regulation-course-of-the-university-of-oxford/2020/1/solution.md)
- [QUIC](quic.md)
- [Transport port](transport-port.md)
- [Transport protocol](transport-protocol.md)
