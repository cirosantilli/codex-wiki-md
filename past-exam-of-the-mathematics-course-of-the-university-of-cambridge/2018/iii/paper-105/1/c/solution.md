<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose $x$ at which $Du(x)$ is finite and the $p$-mean version of the [Lebesgue differentiation theorem](../../../../../../lebesgue-differentiation-theorem.md) holds:

$$
\varepsilon_x(r):=\left(\frac1{|Q_r(x)|}\int_{Q_r(x)}|Du(z)-Du(x)|^p dz\right)^{1/p}\longrightarrow0.
$$

These conditions hold [almost everywhere](../../../../../../almost-everywhere.md). On a cube about $x$, subtract the affine function and put $v(y)=u^*(y)-u^*(x)-Du(x)\cdot(y-x)$. Its [weak derivative](../../../../../../weak-derivative.md) is $Dv=Du-Du(x)$ and $v(x)=0$. Approximate $u$ as in part (b) and subtract the same affine function from the approximants. [Uniform convergence](../../../../../../uniform-convergence.md) and convergence of their [weak derivatives](../../../../../../weak-derivative.md) extend part (a)'s estimate to $v$, giving

$$
|v(y)|\leq Cr^{1-n/p}\|Du-Du(x)\|_{L^p(Q_r(x))}
=Cr\varepsilon_x(r)\qquad(y\in Q_r(x)).
$$

For $h\ne0$, choose $r=4|h|$ and $y=x+h$. It follows that

$$
\frac{|u^*(x+h)-u^*(x)-Du(x)\cdot h|}{|h|}
\leq4C\varepsilon_x(4|h|)\longrightarrow0.
$$

This is precisely classical [Fréchet derivative](../../../../../../frechet-derivative.md) differentiability, not merely existence of coordinate derivatives. Therefore the [differentiability almost everywhere of supercritical Sobolev functions](../../../../../../differentiability-almost-everywhere-of-supercritical-sobolev-functions.md) gives

$$
\boxed{D_{\mathrm{classical}}u^*(x)=D_{\mathrm{weak}}u(x)\quad\text{for almost every }x.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
