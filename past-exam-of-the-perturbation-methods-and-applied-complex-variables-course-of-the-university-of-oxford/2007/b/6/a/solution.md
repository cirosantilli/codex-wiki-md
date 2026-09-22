<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Conformality](../../../../../conformality.md) implies $f'(0)\neq0$, so $a_1\neq0$. Apply the stated [Green's theorem](../../../../../green-theorem.md) with $F=z^n\bar z$:

$$
M_n=\frac1{2i}\oint_\Gamma z^n\bar z\,dz
=\frac1{2i}\oint_{|\zeta|=1}f(\zeta)^n
\left(\sum_{j=1}^N\bar a_j\zeta^{-j}\right)f'(\zeta)\,d\zeta.
$$

Here $\bar\zeta=\zeta^{-1}$ on the [unit circle](../../../../../complex-unit-circle.md). The lowest power in $f^nf'$ is $\zeta^n$, while the most negative power in the conjugate [polynomial](../../../../../polynomial-split.md) is $\zeta^{-N}$. For $n\geq N$ their product has no $\zeta^{-1}$ term. The [residue theorem](../../../../../residue-theorem.md) gives **$M_n=0$ for all $n\geq N$**.

When $N=2$, the residue for $n=0$ is $|a_1|^2+2|a_2|^2$. For $n=1$, expand

$$
ff'=a_1^2\zeta+3a_1a_2\zeta^2+2a_2^2\zeta^3.
$$

Only $a_1^2\zeta\,\bar a_2\zeta^{-2}$ contributes. Therefore

$$
\boxed{M_0=\pi(|a_1|^2+2|a_2|^2),\qquad M_1=\pi a_1^2\bar a_2.}
$$

The first is the area; the second records its complex first moment, and need not be real.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
