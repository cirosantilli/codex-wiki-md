<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The all-time conclusion in the original PDF is false. The [expanding-flow transformation of a wave equation](../../../../../../../expanding-flow-transformation-of-a-wave-equation.md) makes both the correct forward statement and a counterexample transparent. Put

$$
X=\rho e^{-t},\qquad S=e^{-t}>0,\qquad u(\rho,t)=w(X,S).
$$

For $D=\partial_t+\rho\partial_\rho$, the expanded operator from part (i) is $D^2+D-\partial_\rho^2$. In the new variables $D=-S\partial_S$ and $\partial_\rho=S\partial_X$, hence

$$
(D^2+D-\partial_\rho^2)u=S^2(w_{SS}-w_{XX}).
$$

Thus it is the ordinary [wave equation](../../../../../../../wave-equation-split.md) on the half-plane $S>0$. By the [D'Alembert formula](../../../../../../../d-alembert-s-formula.md), any $C^2$ solution has the form

$$
u(\rho,t)=F(e^{-t}(\rho+1))+G(e^{-t}(\rho-1)).
$$

At $t=0$, differentiating the zero displacement with respect to $\rho$ and using the zero velocity gives, for $-1<\rho<1$,

$$
F'(\rho+1)+G'(\rho-1)=0,\qquad
(\rho+1)F'(\rho+1)+(\rho-1)G'(\rho-1)=0.
$$

Subtracting $(\rho-1)$ times the first equation from the second gives $2F'(\rho+1)=0$, and then $G'(\rho-1)=0$. Thus $F=c$ on $(0,2)$ and $G=-c$ on $(-2,0)$. If $t\geq0$ and $-1<\rho<1$, both arguments remain in those intervals. Consequently the valid forward result is

$$
\boxed{u(\rho,t)=0\quad(-1<\rho<1,\ t\geq0).}
$$

For negative time the arguments need not stay in the initial intervals. Take $F(s)=(s-2)_+^3$ and $G=0$, where $q_+=\max\{q,0\}$. Then

$$
\boxed{u(\rho,t)=\bigl(e^{-t}(\rho+1)-2\bigr)_+^3}
$$

is a global $C^2$ solution, has the prescribed zero initial displacement and velocity on $(-1,1)$, but $u(0,-\log3)=1$. This directly disproves the assertion for $t\in\mathbb R$.

The connection with part (i) is directional [finite propagation speed](../../../../../../../finite-propagation-speed.md). At a future point in the strip, the two characteristics traced back to $t=0$ meet it at $\rho_0=e^{-t}(\rho+1)-1$ and $\rho_0=e^{-t}(\rho-1)+1$, both in $(-1,1)$. For negative time these intersections can lie outside that interval. The lines $\rho=\pm1$ are characteristic barriers for this forward domain of dependence, not barriers in both time directions.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
