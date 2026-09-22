<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In a coordinate chart the [Lie derivative of a function](../../../../../lie-derivative-of-a-function.md) and [Lie derivative of a vector field](../../../../../lie-derivative-of-a-vector-field.md) are

$$
\mathcal L_Xf=X^a\partial_af,\qquad(\mathcal L_XY)^a=X^b\partial_bY^a-Y^b\partial_bX^a.
$$

The [Lie derivative of a tensor field](../../../../../lie-derivative-of-a-tensor-field.md) is the extension that respects tensor products and contractions. For a [covector field](../../../../../one-form.md) $\alpha$, differentiate the scalar pairing $\alpha(Y)$ to obtain $(\mathcal L_X\alpha)(Y)=X(\alpha(Y))-\alpha([X,Y])$. In components this gives

$$
(\mathcal L_X\alpha)_a=X^b\partial_b\alpha_a+\alpha_b\partial_aX^b.
$$

Thus for a mixed rank-two [tensor field](../../../../../tensor-field.md), the [coordinate tensor Lie derivative](../../../../../coordinate-tensor-lie-derivative.md) is

$$
(\mathcal L_XS)^a{}_b=X^c\partial_cS^a{}_b-S^c{}_b\partial_cX^a+S^a{}_c\partial_bX^c.
$$

Each upper index contributes a negative derivative of the generator and each lower index a positive one. Explicitly, for type $(m,n)$,

$$
(\mathcal L_XS)^{a_1\cdots a_m}{}_{b_1\cdots b_n}=X^c\partial_cS^{a_1\cdots a_m}{}_{b_1\cdots b_n}-\sum_{r=1}^m(\partial_cX^{a_r})S^{a_1\cdots c\cdots a_m}{}_{b_1\cdots b_n}+\sum_{s=1}^n(\partial_{b_s}X^c)S^{a_1\cdots a_m}{}_{b_1\cdots c\cdots b_n}.
$$

These rules follow by expanding in coordinate vector and covector bases and using the product rule; they define the extension independently of that basis. For a symmetric connection, replacing the partial derivatives by [covariant derivatives](../../../../../covariant-derivative.md) leaves these expressions unchanged because the connection terms cancel.

For the commutator identity, $[\mathcal L_X,\mathcal L_Y]f=[X,Y](f)$ on functions. On a [vector field](../../../../../vector-field.md) $Z$, the [Jacobi identity](../../../../../jacobi-identity.md) gives $[X,[Y,Z]]-[Y,[X,Z]]=[[X,Y],Z]$. The difference $D=[\mathcal L_X,\mathcal L_Y]-\mathcal L_{[X,Y]}$ is a tensor derivation respecting contractions. Since it vanishes on functions and vectors, pairing a covector with every vector shows it vanishes on covectors. Product expansions then show it vanishes on every tensor. This proves the [commutator identity for Lie derivatives](../../../../../commutator-identity-for-lie-derivatives.md):

$$
\boxed{[\mathcal L_X,\mathcal L_Y]=\mathcal L_{[X,Y]}.}
$$

A [Killing vector](../../../../../killing-vector-field.md) generates infinitesimal isometries, meaning $\mathcal L_Kg=0$, equivalently the [Killing equation](../../../../../killing-equation.md) $\nabla_aK_b+\nabla_bK_a=0$ for the metric [Levi-Civita connection](../../../../../levi-civita-connection.md). Linearity in the generator gives $\mathcal L_{aK+bL}g=0$ for real constants $a,b$ whenever $K,L$ are Killing. The identity above likewise gives $\mathcal L_{[K,L]}g=[\mathcal L_K,\mathcal L_L]g=0$. Thus the Killing fields form a real [Lie algebra](../../../../../lie-algebra-split.md); arbitrary nonconstant coefficients would introduce additional derivative terms.

For the rotating star, the hypothesis that there are exactly two independent Killing fields means $[T,\Phi]=aT+b\Phi$ with constant coefficients. Axial symmetry supplies a periodic rotation flow; with the stated asymptotic normalization its generator is $\Phi$ and its period is $2\pi$. Pullback by this flow acts on the Killing algebra, so $e^{2\pi\operatorname{ad}\Phi}=1$. In the basis $(T,\Phi)$, $\operatorname{ad}\Phi$ has matrix

$$
\begin{pmatrix}-a&0\\-b&0\end{pmatrix}.
$$

Its real eigenvalues are $-a$ and zero, so the exponential identity forces $a=0$. The remaining matrix squares to zero; its exponential is then $1+2\pi\operatorname{ad}\Phi$, forcing $b=0$. The [two-dimensional Killing algebra with a periodic generator is abelian](../../../../../two-dimensional-killing-algebra-with-a-periodic-generator-is-abelian.md) result therefore gives $\boxed{[T,\Phi]=0}$.

This uses genuine periodic axial symmetry and the two-dimensional Killing algebra. Mere limits of vector components do not by themselves justify differentiating those limits to evaluate their bracket; the periodic-flow argument avoids that gap. With the usual differentiable asymptotically flat falloff one can also take the bracket at infinity and use independence of the limiting time and angular generators to set both constants to zero.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
