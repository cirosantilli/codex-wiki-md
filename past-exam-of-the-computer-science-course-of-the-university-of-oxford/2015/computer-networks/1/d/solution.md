<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A physical link can deliver a continuous stream of [bits](../../../../../bit.md); the [data link layer](../../../../../data-link-layer.md) needs to identify where each separately meaningful unit begins and ends. [Framing](../../../../../framing.md) supplies those boundaries, so the receiver can separate the [data-link frame](../../../../../frame-networking.md) header, data and checking information, associate an [error detection and correction](../../../../../error-detection-and-correction.md) result with a particular [data-link frame](../../../../../frame-networking.md), and regain alignment after damaged input.

Timing the individual [bits](../../../../../bit.md) is insufficient: knowing where each [bit](../../../../../bit.md) begins does not tell the receiver which [bit](../../../../../bit.md) starts a new [data-link frame](../../../../../frame-networking.md). Thus

$$
\boxed{\text{framing partitions a bit stream into recognizable data-link units}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Computer networks](../../../computer-networks-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
