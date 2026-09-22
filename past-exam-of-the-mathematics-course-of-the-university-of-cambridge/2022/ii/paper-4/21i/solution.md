<h1 id="21i/solution">Solution</h1>

↑ **Parent:** [21I](../21i.md)

Cut the square model of the [Klein bottle](../../../../../klein-bottle.md) along the midline parallel to the pair of sides whose identification reverses orientation. Each half becomes a [Möbius band](../../../../../mobius-band.md), and the two new boundary circles are identified. If $a$ and $b$ are the core loops of these two bands, each boundary travels twice around its core. The [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) therefore gives

$$
\boxed{
\pi_1(K,k_0)
\cong\langle a,b\mid a^2b^{-2}=1\rangle
}.
$$

Writing $x=a^{-1}b$ and $y=a$ converts this into the standard Klein-bottle presentation

$$
\langle x,y\mid yxy^{-1}=x^{-1}\rangle.
$$

The orientation homomorphism sends both $a$ and $b$ to the nonzero element of $C_2$. Its kernel is the index-two subgroup

$$
H=\langle a^2,a^{-1}b\rangle\cong\mathbb Z^2.
$$

By the classification of connected covering spaces, $H$ determines the [orientation double cover of the Klein bottle](../../../../../orientation-double-cover-of-the-klein-bottle.md)

$$
p:(T^2,x_0)\longrightarrow(K,k_0).
$$

Choosing torus generators $\alpha,\beta$ along the two translation directions, we may take

$$
\boxed{
p_*(\alpha)=a^2,
\qquad
p_*(\beta)=a^{-1}b
}.
$$

These commute: the standard relation says that $a$ conjugates $a^{-1}b=x$ to $x^{-1}$, so $a^2$ centralizes $x$.

The space $Y$ is the [mapping cylinder](../../../../../mapping-cylinder.md) of $p$ with its unused end omitted. Sliding $(x,t)$ to $(x,0)$ gives a deformation retraction of $Y$ onto the bottom quotient $T^2/{\sim}\cong K$. Hence

$$
\boxed{
\pi_1(Y,y_0)\cong\pi_1(K,k_0)
\cong\langle a,b\mid a^2b^{-2}\rangle
}.
$$

Finally suppose $U\subseteq X$ is open and homeomorphic to $Y$, and identify the bottom copy of $K$ inside $U$. This $K$ is compact and therefore closed in the Hausdorff space $X$. Apply van Kampen, in its groupoid form if intersections are disconnected, to

$$
X=U\cup(X\setminus K).
$$

The intersection $U\setminus K$ deformation retracts to a positive-height torus, and its map to $\pi_1(U)\cong\pi_1(K)$ has image precisely

$$
p_*\pi_1(T^2)=H.
$$

The orientation homomorphism

$$
\pi_1(U)\longrightarrow\pi_1(U)/H\cong C_2
$$

is zero on this intersection, so it is compatible with the trivial homomorphism from $\pi_1(X\setminus K)$ to $C_2$. The pushout property in van Kampen extends it to a surjection

$$
\pi_1(X)\twoheadrightarrow C_2.
$$

Therefore

$$
\boxed{X\text{ cannot be simply connected}}.
$$

This is the [Klein-bottle mapping-cylinder obstruction to simple connectivity](../../../../../klein-bottle-mapping-cylinder-obstruction-to-simple-connectivity.md).

## ↑ Ancestors (10)

1. [21I](../21i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
