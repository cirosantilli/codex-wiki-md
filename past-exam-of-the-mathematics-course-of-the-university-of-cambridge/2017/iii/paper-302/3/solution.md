<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The triple bond in the original [Dynkin diagram](../../../../../dynkin-diagram.md) gives the [Cartan integers](../../../../../cartan-integer.md)

$$
\langle\beta,\alpha^\vee\rangle=-1,\qquad\langle\alpha,\beta^\vee\rangle=-3,
$$

where $\alpha$ is the [long root](../../../../../long-root.md) and $\beta$ the [short root](../../../../../short-root.md). Their product is $4\cos^2\theta=3$, and the [inner product](../../../../../inner-product.md) of distinct [simple roots](../../../../../simple-root.md) is nonpositive. The ratio of the two integers gives the squared-length ratio. Therefore

$$
\boxed{\theta=\frac{5\pi}{6}=150^\circ,\qquad\frac{\|\alpha\|}{\|\beta\|}=\sqrt3.}
$$

It is convenient to normalize $(\alpha,\alpha)=6$, $(\beta,\beta)=2$ and $(\alpha,\beta)=-3$. Scaling the [inner product](../../../../../inner-product.md) does not affect the [root system](../../../../../root-system.md) or the fundamental-weight relations.

For nonproportional roots $\gamma,\delta$, the [root-string theorem](../../../../../root-string-theorem.md) states that the [root string](../../../../../root-string.md) is consecutive:

$$
S_{\gamma,\delta}=\{\delta-p\gamma,\ldots,\delta+q\gamma\},\qquad p,q\in\mathbb Z_{\ge0},\qquad p-q=\frac{2(\delta,\gamma)}{(\gamma,\gamma)}.
$$

The endpoints are maximal, and reflection in $\gamma$ reverses the string. The [Cartan integer](../../../../../cartan-integer.md) determines $p-q$, not in general the total $p+q+1$ by itself. This result follows by restricting the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) to the [sl2 subalgebra associated with a root](../../../../../sl2-subalgebra-associated-with-a-root.md). If the roots are distinct [simple roots](../../../../../simple-root.md), $\delta-\gamma$ cannot be a root: its simple-root coefficients have opposite signs. Thus $p=0$ and

$$
\boxed{|S_{\gamma,\delta}|=1-\langle\delta,\gamma^\vee\rangle.}
$$

Here length means number of roots; the number of intervals between them is one less. Distinctness matters. If $\gamma=\delta$, a reduced [root system](../../../../../root-system.md) gives the set $\{\gamma,-\gamma\}$, with a missing zero between them, so the consecutive-string theorem and the displayed simple-root formula do not apply.

In the [G2 root system](../../../../../g2-root-system.md), the initial strings are

$$
\boxed{S_{\alpha,\beta}=\{\beta,\alpha+\beta\},\qquad S_{\beta,\alpha}=\{\alpha,\alpha+\beta,\alpha+2\beta,\alpha+3\beta\}.}
$$

For $\delta=\alpha+3\beta$, $\langle\delta,\alpha^\vee\rangle=-1$. Since $\delta-\alpha=3\beta$ is not a root in a [reduced root system](../../../../../reduced-root-system.md), $p=0$ and $q=1$: this generates $2\alpha+3\beta$. The remaining strings explain why the construction stops. The $\alpha$-strings through $\beta$ and $\alpha+\beta$ are the same two-element string; the one through $\alpha+2\beta$ is a singleton since subtracting $\alpha$ gives $2\beta$, and its [Cartan integer](../../../../../cartan-integer.md) is zero; the one through $2\alpha+3\beta$ is the string $\{\alpha+3\beta,2\alpha+3\beta\}$. The $\beta$-strings through $\alpha$, $\alpha+\beta$, $\alpha+2\beta$ and $\alpha+3\beta$ are the initial four-element string. Finally, $2\alpha+3\beta$ is orthogonal to $\beta$; its $\beta$-string is a singleton because $2\alpha+2\beta=2(\alpha+\beta)$ is not a root. Apply the same reasoning to negatives. Using the permitted completeness of this procedure gives

$$
\boxed{\Phi=\pm\{\beta,\alpha,\alpha+\beta,\alpha+2\beta,\alpha+3\beta,2\alpha+3\beta\}.}
$$

The short positive roots are $\beta,\alpha+\beta,\alpha+2\beta$, of squared length two; the other three are long, of squared length six. Each [root space](../../../../../root-space.md) is one-dimensional and the [Cartan subalgebra](../../../../../cartan-subalgebra.md) has dimension two, so

$$
\boxed{\dim G_2=2+12=14.}
$$

Here the dimension refers to the [Lie algebra](../../../../../lie-algebra-split.md), with one Cartan generator per rank, not just the number of roots.

Write a prospective weight as $w=a\alpha+b\beta$. The pairings with simple [coroots](../../../../../coroot.md) are

$$
\langle w,\alpha^\vee\rangle=2a-b,\qquad\langle w,\beta^\vee\rangle=-3a+2b.
$$

The [fundamental weights](../../../../../fundamental-weight.md) are dual to those [coroots](../../../../../coroot.md). Solving the two linear systems gives, in the long-root-first numbering of this paper,

$$
\boxed{\omega_1=2\alpha+3\beta,\qquad\omega_2=\alpha+2\beta.}
$$

The representation with [Dynkin labels](../../../../../dynkin-label.md) $(0,1)$ has [highest weight](../../../../../highest-weight-of-a-representation.md) $\lambda=\omega_2$, a short root. Numbering the short root first, as some references do, would call this the $(1,0)$ representation instead; the representation itself is unchanged.

The weight set of a finite-dimensional irreducible [highest-weight representation](../../../../../highest-weight-representation.md) is invariant under the [Weyl group](../../../../../weyl-group.md) and lies in the [convex hull](../../../../../convex-hull.md) of the orbit of its [highest weight](../../../../../highest-weight-of-a-representation.md). All weights also differ from the [highest weight](../../../../../highest-weight-of-a-representation.md) by an element of the [root lattice](../../../../../root-lattice.md). The orbit of $\lambda$ comprises the six short roots, so all six are weights. The [lowering operators](../../../../../lowering-operator.md) give the chain

$$
\alpha+2\beta\ \xrightarrow{-\beta}\ \alpha+\beta\ \xrightarrow{-\alpha}\ \beta\ \xrightarrow{-\beta}\ 0\ \xrightarrow{-\beta}\ -\beta\ \xrightarrow{-\alpha}\ -\alpha-\beta\ \xrightarrow{-\beta}\ -\alpha-2\beta.
$$

In particular zero occurs: at weight $\beta$, its pairing with $\beta^\vee$ is two, so the lowering operator is nonzero by the finite-dimensional [sl2 Lie algebra](../../../../../sl2-lie-algebra.md) representation theory. The $\beta$-string through it is the usual three-weight string $\beta,0,-\beta$; higher weight $2\beta$ would lie outside the highest-weight convex hull.

There can be no further weights. Every point of that convex hull has squared norm at most $\|\lambda\|^2=2$, while a root-lattice point has

$$
\|a\alpha+b\beta\|^2=6a^2-6ab+2b^2=\frac32a^2+2\left(b-\frac32a\right)^2.
$$

The integer solutions of the bound $\|w\|^2\le2$ are precisely zero and the six short roots: $a=0$ gives $b=-1,0,1$; $a=1$ gives $b=1,2$; and $a=-1$ gives $b=-1,-2$. Thus

$$
\boxed{\operatorname{Wt}V(0,1)=\{0,\pm\beta,\pm(\alpha+\beta),\pm(\alpha+2\beta)\},\qquad\dim V(0,1)=7.}
$$

The final dimension uses the stipulated nondegeneracy of the weights. It also agrees with the [Weyl dimension formula](../../../../../weyl-dimension-formula.md) without that stipulation. The zero weight is not in the Weyl orbit of the nonzero weights, so this is not a [minuscule representation](../../../../../minuscule-representation.md).

<a id="3/image-g2-roots-and-weights-of-its-seven-dimensional-representation"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-302-g2-roots.png)

**[Figure 1](#3/image-g2-roots-and-weights-of-its-seven-dimensional-representation). G2 roots and weights of its seven-dimensional representation**. The twelve [roots of a root system](../../../../../root-of-a-root-system.md) and seven [weights](../../../../../weight-representation-theory.md) in the long-root-first convention.

In the diagram above, a coordinate label $(a,b)$ means $a\alpha+b\beta$. The left panel contains all twelve [roots of a root system](../../../../../root-of-a-root-system.md); the right panel contains the six short-root weights and the zero weight. The long-root-first convention is the same as in the calculations.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
