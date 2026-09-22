<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Consistency was established in part (a). By the [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md), convergence additionally requires the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md). Since $\rho(w)=(w-1)(w-\alpha)$, its roots lie in the closed [unit disk](../../../../../../unit-disk.md) with each unit-modulus root simple exactly for

$$
\boxed{-1\leq\alpha<1.}
$$

The endpoint $\alpha=-1$ is [zero-stability](../../../../../../zero-stability.md) although it has a simple parasitic root at minus one; $\alpha=1$ has a repeated root at one and is excluded.

For every parameter in this convergent range, the leading coefficient of $\sigma$ is $(5+\alpha)/12>0$, while

$$
\sigma(-1)=-(1-\alpha)/3<0.
$$

Since $\sigma(w)\to+\infty$ as $w\to-\infty$, it has a real root $w_*<-1$. Its other real root lies between minus one and one because $\sigma(1)=1-\alpha>0$, so the exterior root is simple.

On the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md), the [amplification polynomial of a multistep method](../../../../../../amplification-polynomial-of-a-multistep-method.md) is $P_z(w)=\rho(w)-z\sigma(w)$, with $z=h\lambda$. For $|z|\to\infty$, the equivalent polynomial $-P_z/z=\sigma-\rho/z$ tends coefficientwise to $\sigma$, and its leading coefficient stays nonzero. Choose a small closed disk about $w_*$ lying wholly outside the [unit disk](../../../../../../unit-disk.md) and containing no other root of $\sigma$. On its boundary $|\sigma|$ has a positive minimum, while $|\rho/z|$ is smaller for every sufficiently large $|z|$. [Rouché's theorem](../../../../../../rouche-s-theorem.md) then puts one root of $P_z$ inside this exterior disk for all such complex $z$.

That root violates the stability [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md). Hence there is a finite radius $R_\alpha$ beyond which no point belongs to the [absolute stability](../../../../../../linear-stability-domain.md) domain:

$$
\boxed{\mathcal S_\alpha\subseteq\{z\in\mathbb C:|z|\leq R_\alpha\},\qquad-1\leq\alpha<1.}
$$

This proves boundedness in every complex direction, rather than only excluding [A-stability](../../../../../../a-stability.md). It is an instance of [exterior roots of the derivative polynomial bound multistep stability](../../../../../../exterior-roots-of-the-derivative-polynomial-bound-multistep-stability.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
