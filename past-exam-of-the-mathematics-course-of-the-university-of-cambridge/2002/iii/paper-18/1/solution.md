<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The displayed torus-only [Weyl integration formula](../../../../../weyl-integration-formula.md) needs $\varphi$ to be a [class function](../../../../../class-function.md), meaning $\varphi(xgx^{-1})=\varphi(g)$. This hypothesis is implicit in the usual formula but is not printed here. We prove the general version for a continuous function, then specialize:

$$
\int_G\varphi(g)\,dg
=\frac1{|W|}\int_T\int_{G/T}\varphi(xtx^{-1})\,d\mu(xT)\,|\Delta(t)|^2\,dt.
$$

Here $dg$ and $dt$ are probability [Haar measures](../../../../../haar-measure.md); $d\mu$ is the invariant probability measure on the [homogeneous space](../../../../../homogeneous-space.md) $G/T$; and $W=N_G(T)/T$ is the finite [Weyl group](../../../../../weyl-group.md).

We use the following standard maximal-torus facts, as permitted: every element of a connected [compact Lie group](../../../../../compact-lie-group.md) lies in some [maximal torus](../../../../../maximal-torus.md); all maximal tori are conjugate; two elements of a fixed $T$ are conjugate in $G$ exactly when they are in the same $W$-orbit; and the complexified [Lie algebra](../../../../../lie-algebra-split.md) decomposes into $\mathfrak t_{\mathbb C}$ and one-dimensional [root spaces](../../../../../root-space.md). Opposite [roots of a root system](../../../../../root-of-a-root-system.md) give real two-dimensional planes in $\mathfrak t^\perp$. At an element $t$ for which no root character has value one, the identity component of its centralizer is $T$.

Choose a positive [root system](../../../../../root-system.md) $\Phi^+$. Regard each root $\alpha$ as a [character](../../../../../character-of-a-representation.md) $\alpha:T\to U(1)$ through the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md). A convenient globally defined denominator is

$$
\Delta_0(t)=\prod_{\alpha\in\Phi^+}(1-\alpha(t)^{-1}).
$$

The usual [Weyl denominator](../../../../../weyl-denominator.md) additionally has a unit-modulus factor $e^\rho(t)$, with $\rho$ half the sum of positive roots. Where that half-weight is not a global torus character, it may be interpreted on a covering torus; the squared modulus is nevertheless unambiguous. In either convention,

$$
|\Delta(t)|^2=|\Delta_0(t)|^2
=\prod_{\alpha\in\Phi^+}|1-\alpha(t)|^2.
$$

Average an [inner product](../../../../../inner-product.md) on $\mathfrak g$ over the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) to make it invariant. It defines a bi-invariant [Riemannian metric](../../../../../riemannian-metric.md) on $G$ and the quotient metric on $G/T$. Consider the conjugation map

$$
q:G/T\times T\to G,\qquad q(xT,t)=xtx^{-1}.
$$

At $(T,t)$, identify the source tangent directions with $X\in\mathfrak t^\perp$ and $Y\in\mathfrak t$, and translate the target tangent vector to the identity by $t^{-1}$. Differentiating gives

$$
dq_{(T,t)}(X,Y)=(\operatorname{Ad}(t^{-1})-I)X+Y.
$$

The two summands are orthogonal. On a real root plane, $\operatorname{Ad}(t^{-1})$ is a rotation with complex eigenvalues $\alpha(t)^{-1},\alpha(t)$. Thus the absolute real [Jacobian determinant](../../../../../jacobian-determinant.md) on this plane is $|1-\alpha(t)|^2$. The torus direction contributes one. Therefore the [conjugation Jacobian for a compact Lie group](../../../../../conjugation-jacobian-for-a-compact-lie-group.md) is

$$
\boxed{J_q(t)=|\Delta(t)|^2.}
$$

This is also the Jacobian for the normalized measures: the Riemannian submersion has fibers isometric to $T$, so $\operatorname{vol}(G)=\operatorname{vol}(G/T)\operatorname{vol}(T)$; the probability-volume normalization factors cancel.

Let $T_{\rm reg}$ be the elements for which $J_q\neq0$. The restriction of $q$ is a local [diffeomorphism](../../../../../diffeomorphism.md) onto the regular elements of $G$. It is $|W|$-to-one. Indeed, fixing $t_0\in T_{\rm reg}$, any pair with $xtx^{-1}=t_0$ has $xTx^{-1}=T$, because conjugation identifies the identity components of the two centralizers. Thus $x\in N_G(T)$, and there is exactly one pair $(xT,x^{-1}t_0x)$ for each coset in $N_G(T)/T$. This argument does not require the full centralizer of $t_0$ to be connected.

The nonregular locus has measure zero. In $T$ it is a finite union of sets $\alpha(t)=1$ of smaller dimension; their conjugation images are images of smaller-dimensional manifolds under $q$, and hence have zero volume in $G$. The change-of-variables formula for the regular covering therefore gives

$$
|W|\int_G\varphi(g)\,dg
=\int_T\int_{G/T}\varphi(xtx^{-1})\,d\mu(xT)\,|\Delta(t)|^2\,dt.
$$

For a [class function](../../../../../class-function.md), the inner integral is $\varphi(t)$, proving the required formula with its correct hypothesis.

Without conjugation invariance, the torus-only expression can be false. For $G=SU(2)$ with diagonal $T$, take $\varphi(g)=|g_{12}|^2$. It vanishes on $T$, whereas its group integral is $1/2$: the two squared coordinates of a Haar-distributed unit column have equal means and sum to one. Thus the conjugacy average cannot simply be dropped.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
