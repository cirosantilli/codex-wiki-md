<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $\epsilon\to0^+$. A root on the smaller scale has $x=\epsilon u$, giving $u+2+\epsilon u^3=0$. Put $u=u_0+\epsilon u_1+O(\epsilon^2)$. Successive [coefficients](../../../../coefficient.md) give $u_0=-2$ and $u_1+u_0^3=0$, hence $u_1=8$. The real root is therefore

$$
\boxed{x_0=-2\epsilon+8\epsilon^2+O(\epsilon^3).}
$$

The other [dominant balance](../../../../dominant-balance.md) is between the cubic and linear terms, requiring $x=\epsilon^{1/2}z$. Set $t=\epsilon^{1/2}$; the equation becomes $z^3+z+2t=0$. At $t=0$ the two nonzero roots are $z_0=\pm i$. With $z=z_0+t z_1+O(t^2)$, the first correction satisfies $(3z_0^2+1)z_1+2=0$, so $-2z_1+2=0$ and $z_1=1$. Thus

$$
\boxed{x_+=i\epsilon^{1/2}+\epsilon+O(\epsilon^{3/2}),\qquad
x_-=-i\epsilon^{1/2}+\epsilon+O(\epsilon^{3/2}).}
$$

The limiting roots in both rescalings are simple, so the [implicit function theorem](../../../../implicit-function-theorem.md) justifies these regular expansions in their respective small parameters. The fractional powers in the original variable are a [fractional-power root expansion](../../../../fractional-power-root-expansion.md). The real [derivative](../../../../derivative.md) $3x^2+\epsilon$ is strictly positive; the cubic therefore has exactly one real root. Its other roots are the displayed [complex conjugate](../../../../complex-conjugate.md) pair, accounting for all three roots. Their leading real corrections sum to $-2\epsilon+\epsilon+\epsilon=0$, as required by the absence of a quadratic [coefficient](../../../../coefficient.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
