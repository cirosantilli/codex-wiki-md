<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $0\le k\le n$, the adjacent [binomial coefficients](../../../../../../binomial-coefficient-split.md) obey

$$
\binom n{k+1}=\binom nk\frac{n-k}{k+1},
\qquad
g(k)=\binom nk\frac{n-2k-1}{k+1}.
$$

Since $\binom nk>0$ and $k+1>0$, the sign is determined by the numerator:

$$
\boxed{g(k)>0\iff0\le k<\frac{n-1}{2}.}
$$

The printed [codomain](../../../../../../codomain.md) $\mathbb N_+$ is inconsistent with the displayed map: $g(n)=-1$, and when $n$ is odd, $g((n-1)/2)=0$. With the usual extension $\binom nk=0$ for $k>n$, $g$ is a [function](../../../../../../function-split.md) $\mathbb N_0\to\mathbb Z$, and $g(k)=0$ for $k>n$; the positive range above remains unchanged. Without that extension, the natural [domain](../../../../../../domain-mathematical-analysis.md) is $\{0,\ldots,n\}$.[Printed page 3, Question 2(b): the map is printed with codomain N+](../../../../../../discrete-mathematics-continuous-mathematics-and-probability-examination-2015-by-university-of-oxford.md)

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
