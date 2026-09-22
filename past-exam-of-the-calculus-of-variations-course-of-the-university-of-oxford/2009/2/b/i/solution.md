<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

At zero, the sixth-power term has zero second [derivative](../../../../../derivative.md), so

$$
\delta^2I_\lambda(0)(\varphi,\varphi)=2Q_\lambda(\varphi),\qquad Q_\lambda(u)=\int_0^\pi(u'^2-\lambda^2u^2)dx.
$$

For $0<\lambda<1$, the Jacobi solution $z(x)=\cos(\lambda(x-\pi/2))$ is strictly positive on $[0,\pi]$. The preceding identity gives $Q_\lambda(u)=\int z^2[(u/z)']^2>0$ for nonzero zero-trace $u$.

To control the nonlinear remainder, a uniform lower bound follows directly. Let $m=\min z>0$, $K=\max|z'|$, and $v=u/z$. Since $\max z=1$ and $\int v^2\leq(\pi^2/2)\int v'^2$ by the elementary endpoint estimate,

$$
\int u'^2\leq2K^2\int v^2+2\int v'^2\leq(K^2\pi^2+2)\int v'^2.
$$

Thus $Q_\lambda(u)\geq c_\lambda\int u'^2$ with $c_\lambda=m^2/(K^2\pi^2+2)>0$. Also $\int u^6\leq\|u\|_\infty^4(\pi^2/2)\int u'^2$, so

$$
I_\lambda(u)\geq\left(c_\lambda-\frac{\pi^2}{4018}\|u\|_\infty^4\right)\int u'^2.
$$

This is positive for every nonzero admissible $u$ sufficiently close to zero in $W^{1,\infty}$. Therefore **zero has positive [second variation](../../../../../second-variation.md) and is a strict weak local minimizer**. No sharp [Poincaré inequality](../../../../../poincare-inequality.md) has been assumed in this proof.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the calculus of variations course of the University of Oxford](../../../../split.md)
6. [Calculus of variations course of the University of Oxford](../../../../../calculus-of-variations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
