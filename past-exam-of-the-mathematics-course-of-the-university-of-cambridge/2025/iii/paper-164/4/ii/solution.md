<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $\delta=d_R(X,Y)$, $A=U_1+U_2$, $B=V_1+V_2$, and $S=A+B$. Distances depend only on distributions, so all variables used in any one application may be realized as [independent random variables](../../../../../../independent-random-variables.md).

First, the [entropy submodularity for three independent sums](../../../../../../entropy-submodularity-for-three-independent-sums.md) implies

$$
d_R(U_1+U_2,X)
\leq\frac12\bigl(2d_R(U,X)+d_R(U,U)\bigr),
$$

and analogously for $V$. The [Entropic Ruzsa triangle inequality](../../../../../../entropic-ruzsa-triangle-inequality.md) gives $d_R(U,U)\leq2d_R(U,X)$ and $d_R(V,V)\leq2d_R(V,Y)$. Consequently the [relevance of independent self-sums](../../../../../../relevance-of-independent-self-sums.md) gives

$$
p+q:=d_R(A,X)+d_R(B,Y)\leq2C\delta.
$$

Apply the [Conditioned entropic Ruzsa distance of a summand](../../../../../../conditioned-entropic-ruzsa-distance-of-a-summand.md) first to $(A,B,X)$ and then to $(B,A,Y)$:

$$
\begin{aligned}
d_R(A\mid S;X)&\leq\frac12\bigl(d_R(A,X)+d_R(B,X)+d_R(A,B)\bigr),\\
d_R(B\mid S;Y)&\leq\frac12\bigl(d_R(B,Y)+d_R(A,Y)+d_R(A,B)\bigr).
\end{aligned}
$$

Three applications of the [Entropic Ruzsa triangle inequality](../../../../../../entropic-ruzsa-triangle-inequality.md) give

$$
d_R(B,X)\leq q+\delta,
\qquad
d_R(A,Y)\leq p+\delta,
\qquad
d_R(A,B)\leq p+\delta+q.
$$

Adding all these bounds yields

$$
\begin{aligned}
d_R(A\mid S;X)+d_R(B\mid S;Y)
&\leq2(p+q+\delta)\\
&\leq(4C+2)\delta.
\end{aligned}
$$

**Thus the required absolute constants may be taken as $a=4$ and $b=2$.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 164](../../../paper-164-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
