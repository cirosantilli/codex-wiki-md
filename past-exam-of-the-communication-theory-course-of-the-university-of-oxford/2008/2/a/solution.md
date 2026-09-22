<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite [probability distribution](../../../../probability-distribution-split.md),

$$
H(X)=-\sum_{p_i>0}p_i\log_2p_i,
$$

with $0\log_20=0$. If the positive support has size $s\le n$, apply the given strict [Jensen inequality](../../../../jensen-s-inequality.md) to the [random variable](../../../../random-variable-split.md) $Z=1/p_X$:

$$
H(X)=\mathbb E\log_2 Z\le\log_2\mathbb EZ=\log_2s\le\log_2n.
$$

Equality requires $s=n$ and $Z$ constant almost surely, so all probabilities are $1/n$. Conversely the uniform distribution attains this bound. Thus $\boxed{H(X)\le\log_2n}$, with exactly that equality case.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
