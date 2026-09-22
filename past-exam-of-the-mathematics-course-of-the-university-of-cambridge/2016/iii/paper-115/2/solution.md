<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In a [manifold chart](../../../../../manifold-chart.md), write a smooth [differential form](../../../../../differential-form-split.md) as $\eta=\sum_I a_I\,dx^{i_1}\wedge\cdots\wedge dx^{i_p}$, with $I$ increasing. Define its [exterior derivative](../../../../../exterior-derivative.md) by

$$
d\eta=\sum_{I,j}\partial_j a_I\,dx^j\wedge dx^{i_1}\wedge\cdots\wedge dx^{i_p}.
$$

To check that this definition is global, change coordinates to $y$. The [chain rule](../../../../../chain-rule.md) expresses $dx^i$ as $\sum_j(\partial_jx^i)dy^j$. Differentiating it gives zero because the second partial derivatives of $x^i$ are symmetric and $dy^k\wedge dy^j$ is antisymmetric. The coordinate definition satisfies the graded [Leibniz rule](../../../../../leibniz-rule.md), so differentiating the transformed expression for $\eta$ leaves exactly $\sum_I da_I\wedge dx^{i_1}\wedge\cdots\wedge dx^{i_p}$. This agrees with the original formula and proves independence of the [manifold chart](../../../../../manifold-chart.md). The same cancellation of mixed derivatives gives $d^2=0$.

The [de Rham cohomology](../../../../../de-rham-cohomology.md) is therefore

$$
H^p_{\mathrm{dR}}(M;\mathbb R)=
\frac{\ker(d:\Omega^p(M)\to\Omega^{p+1}(M))}
{\operatorname{im}(d:\Omega^{p-1}(M)\to\Omega^p(M))},
$$

the [vector space](../../../../../vector-space-split.md) of [closed differential forms](../../../../../closed-differential-form.md) modulo [exact differential forms](../../../../../exact-differential-form.md).

Here is a [Green-theorem proof of exactness on a disc](../../../../../green-theorem-proof-of-exactness-on-a-disc.md). Identify the disc with a round disc centred at zero, and let $\eta=P\,dx+Q\,dy$ be a [closed differential form](../../../../../closed-differential-form.md). Set $f(x)=\int_{[0,x]}\eta$. For $x$ and $x+h$ in the disc, [Green theorem](../../../../../green-theorem.md) on the oriented triangle with vertices $0,x,x+h$ gives zero boundary integral, since $\partial_xQ-\partial_yP=0$. Hence

$$
f(x+h)-f(x)=\int_{[x,x+h]}\eta
=\int_0^1\eta_{x+sh}(h)\,ds.
$$

Taking $h=\varepsilon v$ and dividing by $\varepsilon$ yields $df_x(v)=\eta_x(v)$. The radial integral defining $f$ is smooth, so $\eta=df$ and

$$
\boxed{H^1_{\mathrm{dR}}(\Delta;\mathbb R)=0}.
$$

Degenerate triangles follow by continuity. The same proof works on any star-shaped plane domain, including the whole plane.

Integration requires an [orientation](../../../../../orientation-of-a-simplex.md): take $M$ to be an oriented compact $n$-dimensional [smooth manifold](../../../../../smooth-manifold.md) without boundary. The [Generalized Stokes theorem](../../../../../generalized-stokes-theorem.md) says $\int_Md\beta=0$ for every smooth $(n-1)$-form $\beta$. Every $n$-form is closed by dimension, and changing it by an [exact differential form](../../../../../exact-differential-form.md) leaves its integral unchanged. Thus

$$
[\eta]\longmapsto\int_M\eta
$$

is a well-defined [linear map](../../../../../linear-map.md) $H^n_{\mathrm{dR}}(M;\mathbb R)\to\mathbb R$. Compactness alone does not supply the orientation omitted from the printed integration statement.

For an $n$-dimensional [Lie group](../../../../../lie-group.md), choose a nonzero $\lambda\in\Lambda^nT_e^*G$ and define the [invariant volume form on a Lie group](../../../../../invariant-volume-form-on-a-lie-group.md) by

$$
\omega_g(v_1,\ldots,v_n)
=\lambda\bigl(d(L_{g^{-1}})_gv_1,\ldots,d(L_{g^{-1}})_gv_n\bigr).
$$

Each $dL_{g^{-1}}$ is an [isomorphism](../../../../../isomorphism.md), so $\omega$ is nowhere zero and defines an [orientation](../../../../../orientation-of-a-simplex.md). The composition identity $L_{(hg)^{-1}}\circ L_h=L_{g^{-1}}$ gives $L_h^*\omega=\omega$. Moreover, every [left-invariant differential form](../../../../../left-invariant-differential-form.md) of degree $n$ is determined by its value at $e$, so the space of such forms is one-dimensional.

Under the supplied invariant-representative assumption, all [top-degree de Rham cohomology](../../../../../top-degree-de-rham-cohomology.md) classes are multiples of $[\omega]$. For compact $G$, orient it so $\omega$ is positive; then $\int_G\omega>0$, whereas the [Generalized Stokes theorem](../../../../../generalized-stokes-theorem.md) makes every exact top form have integral zero. Therefore $[\omega]\ne0$ and

$$
\boxed{H^n_{\mathrm{dR}}(G;\mathbb R)\cong\mathbb R}
$$

under that assumption. For actual compact [Lie groups](../../../../../lie-group.md), this argument applies when $G$ is [connected](../../../../../connected-space.md). The supplied assumption fails for disconnected groups: on $S^1\times\mathbb Z/2$, the two components have independent degree-one classes, while globally left-invariant top forms form only a one-dimensional space. In general the [top-degree de Rham cohomology of a compact Lie group](../../../../../top-degree-de-rham-cohomology-of-a-compact-lie-group.md) is $\mathbb R^c$, where $c$ is its number of [connected components](../../../../../connected-component.md).

For $S^2$, use $U=S^2\setminus\{N\}$ and $V=S^2\setminus\{S\}$. [Stereographic projection](../../../../../stereographic-projection.md) identifies each with the plane. The disc argument gives $\eta|_U=df_U$ and $\eta|_V=df_V$ for any [closed differential one-form](../../../../../closed-differential-one-form.md) $\eta$. The overlap $U\cap V$ is [connected](../../../../../connected-space.md), so $d(f_U-f_V)=0$ makes the difference a constant. Adjust one potential by that constant; they glue to a global [smooth function](../../../../../smooth-function.md) $f$ with $df=\eta$. Thus

$$
\boxed{H^1_{\mathrm{dR}}(S^2;\mathbb R)=0}.
$$

Finally, $S^3$ is a compact connected [Lie group](../../../../../lie-group.md): the identification

$$
(a,b)\longmapsto\begin{pmatrix}a&b\\-\overline b&\overline a\end{pmatrix},
\qquad |a|^2+|b|^2=1,
$$

identifies it smoothly with the [special unitary group](../../../../../special-unitary-group.md) $SU(2)$. Matrix multiplication and inversion supply its smooth group operations. The preceding invariant-volume argument therefore gives

$$
\boxed{H^3_{\mathrm{dR}}(S^3;\mathbb R)\cong\mathbb R}.
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 115](../../paper-115-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
