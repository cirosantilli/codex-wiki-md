# Application correctness is not determined by a network trace

↑ **Parent:** [End-to-end principle](end-to-end-principle.md)

Suppose an application's required property depends on [endpoint](communication-endpoint.md) state that is not determined by the network trace. Consider two executions with identical messages and forwarding behaviour: in one the receiver stores the received byte correctly; in the other it corrupts that byte after reception. The network trace is the same, but the required stored-file correctness differs. Any decision based only on that trace must give the same answer in both executions and therefore cannot establish the property for all executions.

This is an indistinguishability argument for that failure model, not a claim that network checks are useless. A link checksum may reduce transmission errors while an application [endpoint](communication-endpoint.md) still has to check the property that spans its storage and processing. Specify the [endpoint](communication-endpoint.md) boundary before claiming an end-to-end guarantee.

## ↑ Ancestors (6)

1. [End-to-end principle](end-to-end-principle.md)
2. [Internet architecture](internet-architecture.md)
3. [Internet](internet.md)
4. [Computer network](computer-network-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-internet-technologies-and-regulation-course-of-the-university-of-oxford/2019/1/solution.md)
- [Solution](past-exam-of-the-internet-technologies-and-regulation-course-of-the-university-of-oxford/2020/1/solution.md)
