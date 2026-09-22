<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Reserve a [frame delimiter](../../../../../frame-delimiter.md) that cannot occur inside encoded [data-link frame](../../../../../frame-networking.md) contents. For a concrete [bit stuffing](../../../../../bit-stuffing.md) rule, take the flag `01111110`. Between flags the sender inserts a zero after every run of five consecutive one [bits](../../../../../bit.md), including runs in the checking information. The receiver removes that zero when decoding. The flags themselves are transmitted without [bit stuffing](../../../../../bit-stuffing.md). For example, the six payload one [bits](../../../../../bit.md) `111111` are sent as `1111101`, so they cannot imitate the flag's run of six ones.[§§5.1–5.2: flag sequence and bit-stuffed transparency](../../../../../ppp-in-hdlc-like-framing-rfc-1662.md)

The receiver recognizes the flag before treating input as payload. After five ones, a following zero is a stuffed [bit](../../../../../bit.md); a following one cannot be ordinary stuffed payload and requires the delimiter/error handling rules. Consequently a delimiter remains recognizable even if the unencoded data contained its exact pattern. [Bit stuffing](../../../../../bit-stuffing.md) also applies at the end of the payload, so a run cannot spill into a boundary ambiguously.

The [frame delimiter](../../../../../frame-delimiter.md) should be long and distinctive enough to support reliable synchronization in the presence of errors, but frequent flags and the run constraint cost capacity. For the usual family of flags with a longer run of ones, a longer forbidden run makes stuffing less frequent while making the delimiter itself longer. Valid stuffed data never contains an intact flag; false flags can arise when transmission errors damage that guarantee. Their likelihood depends on the error model, rather than merely on the raw frequency of the unencoded pattern.

The [data-link frame](../../../../../frame-networking.md) length balances fixed header/flag/check overhead against [network latency](../../../../../network-latency.md), receiver storage and the cost of a damaged [data-link frame](../../../../../frame-networking.md). If independent [bit](../../../../../bit.md) errors have [probability](../../../../../probability.md) $p$, an $N$-[bit](../../../../../bit.md) transmission has no such error with [probability](../../../../../probability.md) $(1-p)^N$. Longer [data-link frames](../../../../../frame-networking.md) amortize fixed overhead, but have more opportunities for corruption and, when [data retransmission](../../../../../retransmission-data-networks.md) is used, waste more work per failed attempt. They also delay delivery until the whole [data-link frame](../../../../../frame-networking.md) is available. A maximum length limits storage requirements and the damage from a lost boundary. The design balance is

$$
\boxed{\text{unambiguous flags; low stuffing overhead; bounded delay and error-recovery cost}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
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
