<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**The claim needs a complete number of logarithmic decades.** For the normalized [log-uniform distribution](../../../../../../log-uniform-distribution.md) on the specified range, $U=\log_{10}X$ is uniform on $(a,b)$. Digit $i$ corresponds to $\{U\}\in[\log_{10}i,\log_{10}(i+1))$. If $b-a=m$ is a positive integer, the integral of a period-one indicator over $(a,a+m)$ is $m$ times its integral over one period. Thus [Benford law from logarithmic uniformity](../../../../../../benford-law-from-logarithmic-uniformity.md) gives

$$
\boxed{\mathbb P(D=i)=\log_{10}(1+1/i)
\quad\text{when }b-a\in\mathbb N.}
$$

This proves the intended case of integers $a<b$, and even permits noninteger $a$ when the span is an integer.

For arbitrary real $a<b$, the exact formula instead is

$$
\boxed{\mathbb P(D=i)=\frac1{b-a}\sum_{k\in\mathbb Z}
\left[\min\{b,k+\log_{10}(i+1)\}
-\max\{a,k+\log_{10}i\}\right]_+.}
$$

Only finitely many terms are nonzero. For a counterexample take $a=0$, $b=\log_{10}2$: then $1<X<2$, so the leading digit is always one. That is not [Benford law](../../../../../../benford-law.md). The unrestricted range in the PDF needs this qualification.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
