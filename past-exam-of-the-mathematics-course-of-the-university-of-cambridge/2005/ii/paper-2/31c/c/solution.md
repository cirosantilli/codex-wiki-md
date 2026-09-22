<h1 id="31c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The given Riccati ansatz is $v'=-iv^2+iz/6$. Differentiating it and substituting for $v'$ shows

$$
v''=-2ivv'+i/6=-2v^3+zv/3+i/6.
$$

It therefore selects $C=i/6$ in the preceding scaled Painleve equation. Write $v=-i\Psi'/\Psi$. The quadratic terms cancel in the ansatz, leaving

$$
-i\left(\frac{\Psi''}{\Psi}+\frac z6\right)=0,
\qquad\Psi''+\frac z6\Psi=0.
$$

Thus every nonzero solution of the indicated [Airy equation](../../../../../../airy-equation.md) gives the local mKdV solution

$$
\boxed{q(x,t)=-it^{-1/3}\frac{\Psi'(xt^{-1/3})}{\Psi(xt^{-1/3})},\qquad t>0,}
$$

on intervals where $\Psi\ne0$. For example $\Psi(z)=A\operatorname{Ai}(-z/6^{1/3})+B\operatorname{Bi}(-z/6^{1/3})$, with constants not both zero, has the required equation. This branch is generally complex and meromorphic; the printed ansatz itself includes $i$. A real $v$ on a real interval would require simultaneously $v'=0$ and $v^2=z/6$, which is impossible on an interval. Hence this particular ansatz does not furnish a nontrivial real-valued mKdV profile.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [31C](../../31c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
