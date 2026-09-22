<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume $q(z)=w'(z)$ is single-valued and a [holomorphic function](../../../../../holomorphic-function-split.md) between $C$ and a sufficiently large enclosing [circle](../../../../../circle.md) $|z|=R$. There are no fluid singularities in that region, so [Cauchy's integral theorem](../../../../../cauchy-s-integral-theorem.md) permits [contour deformation](../../../../../contour-deformation.md):

$$
\Gamma+iM=\oint_Cq(z)\,dz=\oint_{|z|=R}q(z)\,dz.
$$

Use the exterior [Laurent series](../../../../../laurent-series.md) about zero, valid for $|z|$ larger than every finite singularity:

$$
q(z)=\sum_{n=-\infty}^{\infty}a_nz^n,\qquad a_{-1}=b_1.
$$

It converges uniformly on the chosen [circle](../../../../../circle.md), permitting termwise [contour integration](../../../../../contour-integration.md). For integer $n$, parameterization by $z=Re^{i\theta}$ gives

$$
\oint_{|z|=R}z^n\,dz=iR^{n+1}\int_0^{2\pi}e^{i(n+1)\theta}\,d\theta
=\begin{cases}2\pi i,&n=-1,\\0,&n\ne-1.\end{cases}
$$

Only the $z^{-1}$ coefficient survives, proving

$$
\boxed{\Gamma+iM=2\pi i b_1.}
$$

Thus if $b_1=\alpha+i\beta$, then $\Gamma=-2\pi\beta$ and $M=2\pi\alpha$. A [uniform flow](../../../../../uniform-flow.md) contributes a constant to $q$ and changes neither integral. The [Laurent series](../../../../../laurent-series.md) here is an exterior expansion; it need not converge in a punctured neighborhood of zero if other singularities intervene.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
