<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A linear map $T:X\to Y$ is a [weakly compact operator](../../../../../weakly-compact-operator.md) when $T(B_X)$ is relatively weakly compact. Every weakly compact subset of a Banach space is norm bounded, so

$$
\sup_{\lVert x\rVert\leq1}\lVert Tx\rVert<\infty.
$$

Thus even without assuming continuity initially, a weakly compact linear map is bounded.

The key [bidual criterion](../../../../../gantmacher-theorem.md) is

$$
T\text{ is weakly compact}
\quad\Longleftrightarrow\quad
T^{**}(X^{**})\subseteq J_Y(Y).
$$

For the forward implication, approximate $x^{**}\in B_{X^{**}}$ weak-star by points $J_Xx_\alpha$ using the [Goldstine theorem](../../../../../goldstine-theorem.md). Weak compactness supplies a subnet for which $Tx_\alpha$ converges weakly to some $y\in Y$, while weak-star continuity of $T^{**}$ makes $J_YTx_\alpha$ converge to $T^{**}x^{**}$. Hence $T^{**}x^{**}=J_Yy$. Conversely, if the displayed inclusion holds, the weak-star compact set $T^{**}(B_{X^{**}})$ lies in $J_Y(Y)$, where the inherited weak-star topology is the weak topology of $Y$. It is a weakly compact set containing $J_YT(B_X)$.

If $T$ is weakly compact and $y^{***}\in Y^{***}$, restriction of $y^{***}$ to $J_Y(Y)$ defines $y^*\in Y^*$. For $x^{**}\in X^{**}$,

$$
(T^{***}y^{***})(x^{**})
=y^{***}(T^{**}x^{**})
=x^{**}(T^*y^*),
$$

so $T^{***}y^{***}=J_{X^*}(T^*y^*)$. The bidual criterion makes $T^*$ weakly compact. Conversely, if $T^*$ is weakly compact, then $T^{***}(Y^{***})\subseteq J_{X^*}(X^*)$. Every $y^{***}$ annihilating $J_Y(Y)$ is sent to zero, so every $T^{**}x^{**}$ lies in

$$
(J_Y(Y)^\perp)_\perp=J_Y(Y).
$$

The criterion makes $T$ weakly compact. Hence $T$ is weakly compact exactly when $T^*$ is.

The bidual criterion also proves the structure of $\mathcal W(X,Y)$. It is closed under linear combinations. If $T_n\to T$ in operator norm and every $T_n$ is weakly compact, then $T_n^{**}x^{**}\to T^{**}x^{**}$ in norm; the canonical copy $J_Y(Y)$ is norm closed, so $T$ is weakly compact. For bounded composable maps $A$ and $B$, the image condition for $(ATB)^{**}=A^{**}T^{**}B^{**}$ proves the ideal property. Thus the weakly compact operators form a norm-closed [operator ideal](../../../../../operator-ideal-of-weakly-compact-operators.md).

The [Krein-Šmulian theorem](../../../../../krein-smulian-theorem.md) states that the norm-closed convex hull $\overline{\operatorname{co}}K$ of a weakly compact set $K$ is weakly compact. To prove it, view $K$ as a compact Hausdorff space in its weak topology. The probability measures on $K$ form a weak-star compact subset of $C(K)^*$ by the [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md). The barycentre map

$$
\mu\longmapsto b_\mu,
\qquad
x^*(b_\mu)=\int_Kx^*(x)\,d\mu(x)
$$

is weak-star-to-weak continuous; scalar integration and weak compactness ensure that $b_\mu\in X$. Finitely supported probability measures are weak-star dense and their barycentres are precisely $\operatorname{co}K$. The image of all probability measures is therefore the weak closure of $\operatorname{co}K$, and it is weakly compact. A convex set has the same weak and norm closures by the [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md), proving the claim.

If $X$ is reflexive, $B_X$ is weakly compact and every bounded $T:X\to Y$ is weak-to-weak continuous, so $T$ is weakly compact. If $Y$ is reflexive, every bounded subset of $Y$ is relatively weakly compact, with the same conclusion. Thus

$$
\mathcal B(X,Y)=\mathcal W(X,Y)
$$

whenever either space is reflexive.

If $X=\ell^1$ and $Y$ is nonreflexive, the [Eberlein-Šmulian theorem](../../../../../eberlein-smulian-theorem.md) supplies a bounded sequence $(y_n)$ in $Y$ with no weakly convergent subsequence. The formula

$$
T(a)=\sum_{n=1}^\infty a_ny_n
$$

defines a bounded operator $T:\ell^1\to Y$. Since $Te_n=y_n$, it cannot be weakly compact. Therefore $\mathcal B(\ell^1,Y)\ne\mathcal W(\ell^1,Y)$.

This conclusion does not hold for every pair of nonreflexive spaces. Both $c_0$ and $\ell^1$ are nonreflexive, while the [Pitt theorem](../../../../../pitt-theorem.md) says every bounded operator $c_0\to\ell^1$ is compact and hence weakly compact. Thus

$$
\boxed{\mathcal B(c_0,\ell^1)=\mathcal W(c_0,\ell^1).}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
