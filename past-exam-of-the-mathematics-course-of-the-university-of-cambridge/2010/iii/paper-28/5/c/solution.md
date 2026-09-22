<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose a nonconstant [polynomial](../../../../../../polynomial-split.md) $P$ has no zero in $\mathbb C$. Its reciprocal $g=1/P$ is then an entire [holomorphic function](../../../../../../holomorphic-function.md). If $d\geq1$ is the degree and $a_d\ne0$ its leading coefficient, division by $z^d$ shows $P(z)/z^d\to a_d$ as $|z|\to\infty$. Hence $|P(z)|\to\infty$, so $g(z)\to0$. Continuity on compact disks now makes $g$ bounded on all of $\mathbb C$.

Fix $z\in\mathbb C$ and let $B$ be standard [planar Brownian motion](../../../../../../planar-brownian-motion.md) started at zero. By part (a) and [Itô formula](../../../../../../ito-s-lemma.md), both components of $g(z+B_t)$ are [local martingales](../../../../../../local-martingale.md). Since $g$ is bounded, they are true [martingales](../../../../../../martingale-split.md), and

$$
g(z)=\mathbb E[g(z+B_t)]\qquad(t\geq0).
$$

For $\varepsilon>0$, choose $R$ such that $|g(w)|\leq\varepsilon$ whenever $|w|>R$, and write $K=\sup_w|g(w)|$. The two-dimensional Gaussian density of $z+B_t$ is bounded by $1/(2\pi t)$, so

$$
\mathbb P(|z+B_t|\leq R)\leq\frac{\pi R^2}{2\pi t}=\frac{R^2}{2t}.
$$

Consequently

$$
|g(z)|\leq\mathbb E|g(z+B_t)|\leq\varepsilon+\frac{KR^2}{2t}.
$$

Let $t\to\infty$, then $\varepsilon\downarrow0$, to obtain $g(z)=0$. This is impossible for $1/P$. Thus

$$
\boxed{\text{Every nonconstant complex polynomial has a complex zero.}}
$$

This [Brownian proof of the fundamental theorem of algebra](../../../../../../brownian-proof-of-the-fundamental-theorem-of-algebra.md) uses only harmonicity, the bounded-martingale property and the spreading Gaussian transition density. It does not use either maximum principle from part (b), nor does it incorrectly assume that planar Brownian motion hits a specified point.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
