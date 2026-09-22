<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First construct the Dirichlet eigensystem. By part (i) and the [Lax-Milgram theorem](../../../../../../../lax-milgram-theorem.md), the inverse $S=A_D^{-1}$ exists from $L^2$ into $H_0^1$. [Elliptic regularity](../../../../../../../elliptic-regularity.md) gives $Sf\in H^2\cap H_0^1$, and the [Rellich-Kondrachov compactness theorem](../../../../../../../rellich-kondrachov-theorem.md) makes $S$ a [compact operator](../../../../../../../compact-operator-split.md) on $L^2$. Symmetry gives

$$
(Sf,g)=B[Sf,Sg]=(f,Sg),
$$

so $S$ is a [self-adjoint operator](../../../../../../../self-adjoint-operator.md). It is injective, and $(Sf,f)=B[Sf,Sf]>0$ for $f\ne0$. The [spectral theorem for compact Hermitian operators](../../../../../../../spectral-theorem-for-compact-hermitian-operators.md) supplies an [orthonormal basis](../../../../../../../orthonormal-basis.md) $(w_m)$ with $Sw_m=\mu_mw_m$, $\mu_m>0$, and $\mu_m\to0$. Put $\lambda_m=\mu_m^{-1}$. Then

$$
\boxed{Lw_m=\lambda_mw_m,\qquad Tw_m=0,\qquad
0<\lambda_m\longrightarrow\infty.}
$$

Repeated [elliptic regularity](../../../../../../../elliptic-regularity.md) makes each $w_m$ smooth up to the boundary.

As with part (ii), the stated characterization omits boundary compatibility. At $k=0$, its right-hand side is finite for every $u\in L^2$ by [Parseval identity](../../../../../../../parseval-identity.md), whereas its left-hand side would require $u\in H_0^1$. At higher orders, the preceding polynomial example is also decisive for the Dirichlet eigensystem: on $(0,\pi)$,

$$
w_m=\sqrt{2/\pi}\sin(mx),\quad\lambda_m=m^2,\quad
(x(\pi-x),w_m)=\begin{cases}4\sqrt{2/\pi}\,m^{-3},&m\text{ odd},\\0,&m\text{ even}.
\end{cases}
$$

Although this function belongs to every ordinary $H^k$, the weighted sum diverges at $k=3$.

The correct [spectral characterization of elliptic Dirichlet domains](../../../../../../../spectral-characterization-of-elliptic-dirichlet-domains.md) is

$$
\boxed{u\in X_k\iff\sum_m\lambda_m^k|(u,w_m)|^2<\infty,\qquad
X_k=D(A_D^{k/2}),}
$$

with $X_k$ defined in part (ii). For finite eigenfunction sums the squared norm $((u,u))_k$ is exactly the weighted sum: even orders follow from $L^lw_m=\lambda_m^lw_m$, and odd orders also use $B[w_m,w_j]=\lambda_m\delta_{mj}$. These sums are dense in $X_1$: if $v$ is $B$-orthogonal to every $w_m$, then $0=B[v,w_m]=\lambda_m(v,w_m)$, so $v=0$. They are dense in $X_0$ by construction, and the isomorphisms $A_D:X_{k+2}\to X_k$ propagate density to every $X_k$. Completion in the equivalent norms from part (ii) proves both directions of the corrected equivalence. In particular, the printed characterization is correct for $k=1,2$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
