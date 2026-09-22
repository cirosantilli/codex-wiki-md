<h1 id="5a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Rewrite the equation as

$$
y''+q(x)y=0,
\qquad
q(x)=\frac1{\sqrt{1+x^3}}.
$$

On $[2,6]$, one has $q(x)\leq1/3$. If a nontrivial solution had two zeros, choose two consecutive ones $\alpha<\beta$ in that interval. Then $\beta-\alpha\leq4<\pi\sqrt3$.

The solution

$$
\varphi(x)=
\cos\left(\frac{x-(\alpha+\beta)/2}{\sqrt3}\right)
$$

of $\varphi''+\frac13\varphi=0$ is strictly positive on $[\alpha,\beta]$. Since $q\leq1/3$ and the coefficients are not identical on this interval, the [Sturm comparison theorem](../../../../../../sturm-comparison-theorem.md) requires $\varphi$ to have a zero between $\alpha$ and $\beta$, a contradiction. Hence every nontrivial solution has

$$
\boxed{\text{at most one zero on }[2,6]}.
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5A](../../5a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
