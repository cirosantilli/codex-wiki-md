<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For real $x$, the function $F(x)=x^2e^{-x}$ has [derivative](../../../../../../derivative.md) $F'(x)=x(2-x)e^{-x}$. It decreases from infinity to zero on the negative half-line, increases from zero to $4e^{-2}$ on $(0,2)$, and then decreases to zero. Hence sufficiently small positive $\epsilon$ gives exactly three real roots: two near zero and one tending to positive infinity.

Set $\delta=\sqrt\epsilon$ and write either small root as $x=s\delta+A\delta^2+O(\delta^3)$, with $s=\pm1$. Expanding $x^2e^{-x}$ gives $\delta^2+s(2A-1)\delta^3+O(\delta^4)$. Matching its value to $\delta^2$ fixes $A=1/2$. Thus the two [asymptotic expansions](../../../../../../asymptotic-expansion.md) are

$$
\boxed{x_-=-\sqrt\epsilon+\frac\epsilon2+O(\epsilon^{3/2}),\qquad x_+=\sqrt\epsilon+\frac\epsilon2+O(\epsilon^{3/2}).}
$$

For the large root, put $L=\log(1/\epsilon)$. Taking logarithms gives $x-2\log x=L$, so $x/L\to1$. Writing $x=L+r$ then gives $r=2\log L+2\log(1+r/L)$. Iteration yields

$$
\boxed{x_{\rm large}=L+2\log L+O\!\left(\frac{\log L}{L}\right).}
$$

Its two [asymptotic expansion](../../../../../../asymptotic-expansion.md) terms are of different logarithmic orders; a regular power series in $\epsilon$ cannot describe it.

As an exact check, the [real branches of Lambert W](../../../../../../real-branches-of-lambert-w.md) give $x_-=-2W_0(\sqrt\epsilon/2)$, $x_+=-2W_0(-\sqrt\epsilon/2)$ and $x_{\rm large}=-2W_{-1}(-\sqrt\epsilon/2)$. If complex roots are intended instead, there are infinitely many, given by $-2W_j(\pm\sqrt\epsilon/2)$. For each fixed nonprincipal branch their two logarithmic terms follow from $W_j(z)=L_j-\log L_j+O(\log|L_j|/|L_j|)$, where $L_j=\log z+2\pi ij$ and logarithms are continued on that branch. The three real roots are the ones selected above.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
