<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $B=B(0,R)$, with $R>0$. Its [indicator function](../../../../../../indicator-function.md) has [L2 norm](../../../../../../l2-norm.md) squared $\pi R^2$ and [total variation seminorm on a domain](../../../../../../total-variation-seminorm-on-a-domain.md) $2\pi R$. On the family $u=c\chi_B$, the objective is $2\pi\alpha R|c|+\tfrac12\pi R^2(c-1)^2$, whose minimizer is $c=(1-2\alpha/R)_+$. To prove global optimality, a [total variation calibration](../../../../../../total-variation-calibration.md) is needed.

Define the bounded radial [vector field](../../../../../../vector-field.md)

$$
z(x)=\begin{cases}x/R,&|x|\le R,\\Rx/|x|^2,&|x|>R.\end{cases}
$$

It satisfies $|z|\le1$ and has a [continuous](../../../../../../continuous-function.md) normal component across $\partial B$. Its [distributional divergence](../../../../../../distributional-divergence.md) therefore has no boundary measure, and direct differentiation yields $q=\operatorname{div}z=(2/R)\chi_B\in L^2$. Although $z$ is not compactly supported, multiply it by a [smooth](../../../../../../smooth-function.md) radial cutoff equal to one through radius $T$ and zero beyond $2T$. The extra divergence has magnitude $O(R/T^2)$ on an annulus of area $O(T^2)$, hence [L2 norm](../../../../../../l2-norm.md) $O(R/T)$. Smoothing the [continuous](../../../../../../continuous-function.md) piecewise field gives compactly supported [smooth](../../../../../../smooth-function.md) admissible test [vector fields](../../../../../../vector-field.md) with divergences tending to $q$ in $L^2$, preserving the bound $|z|\le1$. The dual definition therefore gives $\langle q,v\rangle\le J(v)$ for every finite-penalty $v$, and trivially for all other $v$.

Moreover $\langle q,\chi_B\rangle=(2/R)\pi R^2=2\pi R=J(\chi_B)$. By the [subgradient](../../../../../../subgradient.md) characterization of an [absolutely one-homogeneous functional](../../../../../../absolutely-one-homogeneous-functional.md), $q\in\partial J(c\chi_B)$ for every $c>0$, and $q\in\partial J(0)$. If $0<\alpha<R/2$, choose $c=1-2\alpha/R$; then $(g-c\chi_B)/\alpha=q$. If $\alpha\ge R/2$, choose $u=0$; then $g/\alpha=(R/(2\alpha))q$ belongs to $\partial J(0)$, since multiplying the dual bound by a number in $[0,1]$ preserves it. The previous optimality criterion proves

$$
\boxed{u(x)=\left(1-\frac{2\alpha}{R}\right)_+\chi_{B(0,R)}(x).}
$$

The quadratic fidelity is [strictly convex](../../../../../../strictly-convex-function.md), so this minimizer is unique, including the threshold $\alpha=R/2$. The disk retains its radius on the positive branch and disappears on the zero branch; this is [total variation denoising of a disk](../../../../../../total-variation-denoising-of-a-disk.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
