<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Part (b) immediately gives $\sqrt I\subseteq I(V(I))$. For the reverse inclusion, let $h\in I(V(I))$. The case $h=0$ is immediate, so assume $h\neq0$. [Noetherianity](../../../../noetherian-ring.md) gives finite generators $I=(f_1,\ldots,f_r)$.

Use the [Rabinowitsch trick](../../../../rabinowitsch-trick.md): in the [polynomial ring](../../../../polynomial-ring.md) with one auxiliary variable, form

$$
J=(f_1,\ldots,f_r,1-th)\subseteq k[x_1,\ldots,x_n,t].
$$

Apply the assumed maximal-ideal description to [polynomial rings](../../../../polynomial-ring.md), including this [ring](../../../../ring.md) in $n+1$ variables. If $J$ were proper, it would lie in the [maximal ideal](../../../../maximal-ideal.md) of some [point](../../../../point-geometry.md) $(a,b)$. Then $a\in V(I)$ and $1-bh(a)=0$, impossible because $h$ vanishes on $V(I)$. Therefore $J$ is the whole [ring](../../../../ring.md), and there is an identity

$$
1=\sum_{i=1}^r P_i(x,t)f_i(x)+Q(x,t)(1-th(x)).
$$

Substitute $t=h^{-1}$ in the [localization](../../../../localization-of-a-ring.md) $R_h$. The last term vanishes; clearing the finitely many powers of $h$ from the remaining denominators yields $h^N\in I$ for some $N$. Thus $h\in\sqrt I$ and

$$
\boxed{I(V(I))=\sqrt I.}
$$

This proves the strong [Hilbert Nullstellensatz](../../../../hilbert-nullstellensatz.md) from the polynomial-ring weak form by converting nonvanishing into an extra equation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebraic Geometry course of the University of Oxford](../../../split.md)
5. [Algebraic Geometry course of the University of Oxford](../../../../algebraic-geometry-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
