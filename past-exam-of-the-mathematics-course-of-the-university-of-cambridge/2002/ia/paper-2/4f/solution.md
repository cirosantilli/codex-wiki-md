<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

After $n+1$ independent tosses, an even count arises in exactly two disjoint ways: an even count after $n$ tosses followed by a tail, or an odd count followed by a head. [Independence](../../../../../independent-random-variables.md) of the last toss from the preceding ones therefore gives

$$
\pi_{n+1}=(1-p)\pi_n+p(1-\pi_n)=p+(1-2p)\pi_n.
$$

Subtracting the [fixed point](../../../../../fixed-point.md) $1/2$ turns this into the [linear recurrence](../../../../../linear-recurrence-relation.md)

$$
\pi_{n+1}-\tfrac12=(1-2p)(\pi_n-\tfrac12).
$$

As zero is even, $\pi_0=1$, so **the probability is**

$$
\boxed{\pi_n=\frac{1+(1-2p)^n}{2}.}
$$

For $p=1/2$ this is $1/2$ for every $n\ge1$; for $p=0$ it is always one; for $p=1$ it alternates between one and zero according to the parity of $n$.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
