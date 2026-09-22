# Layered network architecture

↑ **Parent:** [Computer network](computer-network-split.md)

A [layered network architecture](layered-network-architecture.md) separates responsibilities behind communication interfaces. A [transport protocol](transport-protocol.md) can offer an application a service built over [Internet Protocol](internet-protocol.md) without requiring each underlying network to implement that application. Layer boundaries are engineering choices: the [end-to-end principle](end-to-end-principle.md) helps assess which properties a lower layer can actually establish.

**Table of contents**

- [Data link layer](data-link-layer.md)
  - [Framing](framing.md)
    - [Bit stuffing](bit-stuffing.md)
    - [Frame delimiter](frame-delimiter.md)
  - [Frame (networking)](frame-networking.md)
- [Transport protocol](transport-protocol.md)
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

## ↑ Ancestors (3)

1. [Computer network](computer-network-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Layered network architecture](layered-network-architecture.md)
- [Solution](past-exam-of-the-internet-technologies-and-regulation-course-of-the-university-of-oxford/2020/1/solution.md)
