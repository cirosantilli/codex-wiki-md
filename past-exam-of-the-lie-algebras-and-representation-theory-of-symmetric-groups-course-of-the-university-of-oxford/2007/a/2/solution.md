<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [Cartan subalgebra](../../../../cartan-subalgebra.md) is a nilpotent [Lie subalgebra](../../../../lie-subalgebra.md) equal to its [normalizer of a Lie subalgebra](../../../../normalizer-of-a-lie-subalgebra.md). Write $H=L_{0,x}$ for a choice $x\in A$ attaining the minimum dimension, and let $h=\dim H$. For $y\in A$, the subalgebra $H$ is invariant under $\operatorname{ad}(x+ty)$ because $A\subseteq H$. On $L/H$, the operator induced by $\operatorname{ad}x$ is invertible: $H$ is its full generalized zero eigenspace, and the [finite-dimensional Fitting decomposition](../../../../finite-dimensional-fitting-decomposition.md) separates that from the invertible part.

The determinant of the operator induced by $\operatorname{ad}(x+ty)$ on $L/H$ is a [polynomial](../../../../polynomial-split.md) in $t$, nonzero at zero. Thus it is nonzero for all but finitely many $t\in K$. For these values, the generalized zero eigenspace $L_{0,x+ty}$ lies in $H$. Minimality of $\dim H$ among elements from $A$ forces equality. Hence $\operatorname{ad}(x+ty)|_H$ is nilpotent for all but finitely many $t$.

Each nonleading coefficient of its [characteristic polynomial](../../../../characteristic-polynomial.md) is a [polynomial](../../../../polynomial-split.md) in $t$. Since $K$ is infinite, a [polynomial](../../../../polynomial-split.md) vanishing at all but finitely many elements is identically zero. The coefficient of degree $i$ in the [matrix](../../../../matrix.md) entries is homogeneous of degree $i$; its highest possible $t^i$ coefficient is the corresponding characteristic coefficient of $\operatorname{ad}y|_H$. All these vanish, so that operator has [characteristic polynomial](../../../../characteristic-polynomial.md) $T^h$ and is nilpotent by the [Cayley-Hamilton theorem](../../../../cayley-hamilton-theorem-split.md). Thus

$$
\boxed{H\subseteq L_{0,y}\qquad(y\in A).}
$$

For existence, choose an $L_{0,x}=H$ of smallest dimension among all $x\in L$. Since $x\in H$, it also minimizes the same set with $x$ restricted to $A=H$. Applying the proved statement makes every $\operatorname{ad}y|_H$ nilpotent. [Engel's theorem](../../../../engel-s-theorem.md) makes $H$ nilpotent, and the allowed self-idealizer property makes it self-normalizing. Therefore it is a [Cartan subalgebra](../../../../cartan-subalgebra.md), illustrating [Cartan subalgebra existence from a minimal Engel subalgebra](../../../../cartan-subalgebra-existence-from-a-minimal-engel-subalgebra.md).

For the three-dimensional example, direct use of the brackets gives $C_L(z)=Kz$ for every nonzero $z$: the equations $[u,z]=0$ are the vanishing of all two-by-two minors of the two coordinate [vectors](../../../../vector.md), so they are proportional. Every nonzero nilpotent [Lie algebra](../../../../lie-algebra-split.md) has a nonzero center, as seen from its last nonzero lower-central term. A nilpotent subalgebra $H$ with a central nonzero element $z$ must therefore satisfy $H\subseteq C_L(z)=Kz$, and has dimension one. The zero subalgebra is not self-normalizing. Thus **all [Cartan subalgebras](../../../../cartan-subalgebra.md) have dimension one**. For example $Ka$ is nilpotent and its normalizer is $Ka$, so such subalgebras do occur.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../split.md)
5. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
