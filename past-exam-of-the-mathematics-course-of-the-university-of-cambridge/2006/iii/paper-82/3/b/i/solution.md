<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $X=\epsilon x$ and the [WKB approximation](../../../../../../../wkb-approximation.md)

$$
p=e^{-i\Theta(X)/\epsilon}\bigl[P_0(y,X)+\epsilon P_1(y,X)+\cdots\bigr],\qquad k(X)=\Theta_X(X).
$$

At leading order, the divergence-form acoustic [Helmholtz equation](../../../../../../../helmholtz-equation.md) becomes $P_{0,yy}+[k_0(X)^2-k(X)^2]P_0=0$. The sloping-wall [Neumann boundary condition](../../../../../../../neumann-boundary-condition.md) becomes $P_{0,y}=0$ at $y=\pm R(X)$. In the even transverse family this has [normal modes](../../../../../../../normal-mode.md) $P_0=A(X)\cos(n\pi y/R(X))$, where $n=0,1,\ldots$, and

$$
\boxed{k(X)=\sqrt{k_0(X)^2-\left(\frac{n\pi}{R(X)}\right)^2},\quad
p_0=A(X)\cos\!\left(\frac{n\pi y}{R(X)}\right)
\exp\!\left[-\frac i\epsilon\int^Xk(\xi)d\xi\right].}
$$

For the right-going propagating branch take real positive $k$. The displayed local expression $e^{-ikx}$ in the question must be read as a frozen-coefficient shorthand: the actual slowly varying phase is $\exp[-i\int^x k(\epsilon s)ds]$. Differentiating $e^{-ik(X)x}$ would instead give the erroneous local wavenumber $k+Xk_X$.

The symmetric duct also has odd transverse [normal modes](../../../../../../../normal-mode.md) $\sin[(n+1/2)\pi y/R]$. The integer-cosine form selects the even family requested here, rather than representing every duct mode. The approximation requires smooth slow variation and a positive $k$ separated from cutoff; it fails in a cutoff transition.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 82](../../../../paper-82-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
