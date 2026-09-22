<h1 id="21g/solution">Solution</h1>

↑ **Parent:** [21G](../21g.md)

Given [group homomorphisms](../../../../../group-homomorphism.md) $i_A:C\to A$ and $i_B:C\to B$, their [amalgamated free product](../../../../../amalgamated-free-product.md) is a group $A*_CB$ with maps $j_A:A\to A*_CB$ and $j_B:B\to A*_CB$ satisfying $j_Ai_A=j_Bi_B$, such that every pair $f_A:A\to H$, $f_B:B\to H$ satisfying $f_Ai_A=f_Bi_B$ factors through a unique homomorphism $A*_CB\to H$.

The [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) says that if $X=U_1\cup U_2$, where $U_1,U_2$, and $U_1\cap U_2$ are open and path-connected and $x_0\in U_1\cap U_2$, then the inclusion maps induce

$$
\pi_1(X,x_0)\cong
\pi_1(U_1,x_0)*_{\pi_1(U_1\cap U_2,x_0)}
\pi_1(U_2,x_0).
$$

Here is a direct proof of the requested generation statement. For a [based loop](../../../../../based-loop.md) $\gamma$ in $X$, the [Lebesgue number lemma](../../../../../lebesgue-number-lemma.md) supplies a subdivision

$$
0=t_0<t_1<\cdots<t_m=1
$$

such that every arc $\gamma|_{[t_{j-1},t_j]}$ lies in one $U_{\varepsilon_j}$. Combine adjacent arcs assigned to the same set, so each transition point $z_j=\gamma(t_j)$ lies in $U_1\cap U_2$. Since the intersection is [path-connected](../../../../../path-connected-space.md), choose a path $q_j$ in it from $x_0$ to $z_j$, taking $q_0=q_m$ constant. Then

$$
q_{j-1}*\gamma|_{[t_{j-1},t_j]}*\overline{q_j}
$$

is a loop in $U_{\varepsilon_j}$. In the product of their classes, each $\overline{q_j}*q_j$ cancels by [path reversal](../../../../../path-reversal.md), leaving $[\gamma]$. Thus the two inclusion images generate $\pi_1(X,x_0)$, as summarized by [generation of a fundamental group by two open sets](../../../../../generation-of-a-fundamental-group-by-two-open-sets.md).

Now let $a,b$ be the standard generators in the [fundamental group of the torus](../../../../../fundamental-group-of-the-torus.md). A [Möbius band](../../../../../mobius-band.md) retracts to a core circle, while its boundary traverses that core twice. If $x$ and $y$ denote the core classes of the two attached bands, the [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) gives

$$
\pi_1(Y)
\cong
\langle a,b,x,y\mid [a,b]=1,\ x^2=ab,\ y^2=a^2b^3\rangle.
$$

The two attaching classes $A=ab$ and $B=a^2b^3$ commute. Their exponent matrix has determinant

$$
\det\begin{pmatrix}1&1\\2&3\end{pmatrix}=1,
$$

so they form a basis of $\langle a,b\rangle\cong\mathbb Z^2$, with

$$
a=A^3B^{-1},\qquad b=A^{-2}B.
$$

Substituting $A=x^2$ and $B=y^2$ eliminates $a,b$ and leaves the two-generator one-relator presentation

$$
\boxed{\pi_1(Y)\cong\langle x,y\mid[x^2,y^2]=1\rangle.}
$$

This is the calculation in [two Möbius bands attached to a torus](../../../../../two-mobius-bands-attached-to-a-torus.md).

Finally send $x$ to $(12)$ and $y$ to $(23)$ in the [symmetric group](../../../../../symmetric-group.md) $S_3$. Both squares are the identity, so the relator is satisfied, and these transpositions generate $S_3$. We obtain a surjective [group homomorphism](../../../../../group-homomorphism.md) from $\pi_1(Y)$ onto the nonabelian group $S_3$. Therefore $\pi_1(Y)$ is nonabelian.

## ↑ Ancestors (10)

1. [21G](../21g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
