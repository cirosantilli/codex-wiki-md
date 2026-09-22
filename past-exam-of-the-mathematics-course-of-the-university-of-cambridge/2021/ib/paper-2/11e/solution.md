<h1 id="11e/solution">Solution</h1>

↑ **Parent:** [11E](../11e.md)

The [Poincaré half-plane model](../../../../../poincare-half-plane-model.md) is

$$
\mathbb H=\{z=x+iy:y>0\},
\qquad
ds^2=\frac{dx^2+dy^2}{y^2},
$$

with the orientation inherited from the complex plane. For

$$
\gamma(z)=\frac{az+b}{cz+d},
\qquad
\begin{pmatrix}a&b\\c&d\end{pmatrix}\in SL_2(\mathbb R),
$$

one has

$$
\gamma'(z)=\frac1{(cz+d)^2},
\qquad
\operatorname{Im}\gamma(z)=\frac{\operatorname{Im}z}{|cz+d|^2}.
$$

These identities show directly that $\gamma^*ds^2=ds^2$. The map is holomorphic with nonzero derivative, so it preserves orientation. The matrices $I$ and $-I$ induce the same map, giving the action of [PSL2(R)](../../../../../psl2-r.md).

Conversely, let $F$ be an orientation-preserving isometry. The PSL2(R) action is transitive on $\mathbb H$, so compose $F$ with an element taking $F(i)$ back to $i$. The resulting isometry fixes $i$ and acts on $T_i\mathbb H$ by an orientation-preserving orthogonal map, hence a rotation. The stabilizer of $i$ in PSL2(R),

$$
\left\{
\begin{bmatrix}
\cos\alpha&\sin\alpha\\
-\sin\alpha&\cos\alpha
\end{bmatrix}
\right\},
$$

realizes every such tangent rotation. An isometry is determined by its value and differential at one point because it preserves geodesics and the [exponential map](../../../../../exponential-map-riemannian-geometry.md). Thus the composed isometry belongs to PSL2(R), and so does $F$.

The map $\tau(z)=-\overline z$ is an orientation-reversing isometry. Composing any orientation-reversing isometry with $\tau$ gives an orientation-preserving one, so

$$
\operatorname{Isom}(\mathbb H)
=PSL_2(\mathbb R)\sqcup PSL_2(\mathbb R)\tau.
$$

A hyperbolic line is a vertical Euclidean line or a semicircle orthogonal to the real axis. Its [hyperbolic reflection](../../../../../hyperbolic-reflection.md) $\sigma_\ell$ is the unique orientation-reversing isometry that fixes every point of $\ell$. If $\ell,\ell'$ meet at angle $\theta$, then

$$
\rho=\sigma_\ell\sigma_{\ell'}
$$

is the hyperbolic rotation about $A$ through angle $2\theta$. The generators satisfy

$$
\sigma_\ell^2=\sigma_{\ell'}^2=1,
\qquad
\sigma_\ell\rho\sigma_\ell=\rho^{-1}.
$$

If $\theta/\pi=p/q$ in lowest terms, then $\rho$ has order $q$ and the generated group is the finite [dihedral group](../../../../../dihedral-group.md) of order $2q$. If $\theta/\pi$ is irrational, $\rho$ has infinite order and the generated group is the [infinite dihedral group](../../../../../infinite-dihedral-group.md). In the degenerate case $\ell=\ell'$, the group has order two.

## ↑ Ancestors (10)

1. [11E](../11e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
