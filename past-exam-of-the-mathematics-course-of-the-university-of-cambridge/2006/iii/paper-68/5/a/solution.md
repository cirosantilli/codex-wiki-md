<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $h=\Delta x$, $k=\mu h$ and $M_r=\sum_{j\in\{-2,-1,1,2\}}a_jj^r$. Along a smooth solution, $\partial_t^r u=\partial_x^r u$. The exact difference $u(x,t+k)-u(x,t-k)$ contains only odd [derivatives](../../../../../../derivative.md). Matching terms through degree four therefore requires

$$
M_0=M_2=M_4=0,\qquad M_1=2\mu,\qquad M_3=2\mu^3.
$$

The first two conditions give $a_{-1}+a_1=a_{-2}+a_2=0$, which also implies $M_4=0$. With $a_{-j}=-a_j$, the remaining equations are $a_1+2a_2=\mu$ and $a_1+8a_2=\mu^3$. Hence

$$
\boxed{a_1=\frac{\mu(4-\mu^2)}3,\qquad a_2=\frac{\mu(\mu^2-1)}6,\qquad a_{-1}=-a_1,\quad a_{-2}=-a_2.}
$$

The fifth spatial moment is $M_5=10\mu^3-8\mu$. After dividing the exact-minus-scheme residual by $2k$, its first possible nonzero term is

$$
\frac{h^4}{120}(\mu^2-1)(\mu^2-4)u_{xxxxx}+O(h^6).
$$

This is the [fourth-order two-step advection stencil](../../../../../../fourth-order-two-step-advection-stencil.md). Thus the normalized [local truncation error](../../../../../../local-truncation-error.md) is $O(h^4)$ at fixed positive [Courant number](../../../../../../courant-number.md), as required. At $\mu=1$ or $2$ the formula translates the physical advection branch exactly, but [consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md) alone does not decide [stability](../../../../../../stability-of-a-numerical-method.md) of all two-level perturbations.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
