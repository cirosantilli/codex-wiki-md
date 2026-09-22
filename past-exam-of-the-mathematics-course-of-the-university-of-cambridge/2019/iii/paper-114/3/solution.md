<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An $R$-orientation of a rank-$d$ real [vector bundle](../../../../../vector-bundle.md) $E\to B$ is a locally coherent choice of generator of $H^d(E_b,E_b\setminus\{0\};R)$ in every fibre. Equivalently, it is represented by a [Thom class](../../../../../thom-class.md) $u_E\in H^d(D(E),S(E);R)$ restricting to the chosen generator on each fibre pair. If $e(E)\in H^d(B;R)$ is the [Euler class](../../../../../euler-class-of-a-vector-bundle.md), the [Gysin sequence](../../../../../gysin-sequence-of-a-sphere-bundle.md) of its unit sphere bundle contains

$$
\cdots\to H^{q-d}(B;R)\xrightarrow{\smile e(E)}H^q(B;R)
\to H^q(S(E);R)\to H^{q-d+1}(B;R)\xrightarrow{\smile e(E)}H^{q+1}(B;R)\to\cdots.
$$

The diagonal quotient defining $L(p)$ is the [three-dimensional lens space as a circle bundle](../../../../../three-dimensional-lens-space-as-a-circle-bundle.md) $S^1\to L(p)\to S^2$ with Euler class $p$ times a generator. With integral coefficients, the only nontrivial Euler-class map is multiplication by $p:H^0(S^2;\mathbb Z)\to H^2(S^2;\mathbb Z)$. Exactness gives

$$
\boxed{H^j(L(p);\mathbb Z)\cong
\begin{cases}
\mathbb Z,&j=0,3,\\
\mathbb Z/p,&j=2,\\
0,&\text{otherwise}.
\end{cases}}
$$

Modulo $p$, the Euler class vanishes, so the same [Gysin sequence](../../../../../gysin-sequence-of-a-sphere-bundle.md) gives

$$
\boxed{H^j(L(p);\mathbb F_p)\cong\mathbb F_p\quad(0\leq j\leq3),}
$$

with all other groups zero.

For the coefficient sequence $0\to\mathbb Z\xrightarrow{p}\mathbb Z\to\mathbb F_p\to0$, the [long exact sequence from a coefficient sequence](../../../../../long-exact-sequence-from-a-coefficient-sequence.md) contains

$$
0=H^1(L(p);\mathbb Z)\to H^1(L(p);\mathbb F_p)
\xrightarrow{\delta}H^2(L(p);\mathbb Z)
\xrightarrow{p}H^2(L(p);\mathbb Z).
$$

The last map is zero and both middle groups have order $p$, so $\delta$ is an isomorphism. Reduction $H^2(L(p);\mathbb Z)\to H^2(L(p);\mathbb F_p)$ is likewise an isomorphism. Their composite is the [Bockstein isomorphism for a three-dimensional lens space](../../../../../bockstein-isomorphism-for-a-three-dimensional-lens-space.md)

$$
\boxed{\beta:H^1(L(p);\mathbb F_p)\xrightarrow{\sim}H^2(L(p);\mathbb F_p).}
$$

If $a'=na$ is another generator, linearity of the [Bockstein homomorphism](../../../../../bockstein-homomorphism.md) and bilinearity of the [cup product](../../../../../cup-product.md) give

$$
\boxed{t(a')=n^2t(a).}
$$

Moreover $t(a)\ne0$: $\beta(a)$ is nonzero, and the [Poincare duality](../../../../../poincare-duality.md) pairing $H^1\times H^2\to H^3\cong\mathbb F_p$ is nondegenerate. If $h:L(p)\to L(p)$ is an orientation-reversing [homotopy equivalence](../../../../../homotopy-equivalence.md) and $h^*a=na$, naturality gives

$$
n^2t(a)=t(h^*a)
=\langle h^*(a\smile\beta a),[L(p)]\rangle
=\langle a\smile\beta a,h_*[L(p)]\rangle
=-t(a).
$$

Cancelling the nonzero $t(a)$ yields $n^2\equiv-1\pmod p$. Thus **$-1$ must be a [quadratic residue](../../../../../quadratic-residue.md) modulo $p$**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
