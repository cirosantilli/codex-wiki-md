<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [Lie algebra representation](../../../../../lie-algebra-representation.md) on a [vector space](../../../../../vector-space-split.md) $V$ is a linear map $R:\mathfrak g\to\operatorname{End}(V)$ preserving the [Lie bracket](../../../../../lie-bracket.md):

$$
R([X,Y])=[R(X),R(Y)].
$$

The [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) acts on $V=\mathfrak g$ by $\operatorname{ad}_X(Y)=[X,Y]$. The [Jacobi identity](../../../../../jacobi-identity.md) gives

$$
[\operatorname{ad}_X,\operatorname{ad}_Y]=\operatorname{ad}_{[X,Y]}.
$$

If $\mathfrak g$ is nonabelian, some $[X,Y]$ is nonzero, so this [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) is not the [trivial Lie algebra representation](../../../../../trivial-lie-algebra-representation.md). **It is the required nontrivial representation of dimension $\dim\mathfrak g$.** Nontriviality does not require its homomorphism to be injective.

For the finite-dimensional algebras here, with normalization one, the [Killing form](../../../../../killing-form.md) is

$$
\boxed{\kappa(X,Y)=\operatorname{tr}(\operatorname{ad}_X\operatorname{ad}_Y).}
$$

It is a [symmetric bilinear form](../../../../../symmetric-bilinear-form.md) by cyclicity of the [matrix trace](../../../../../matrix-trace.md). To prove its invariance, write $A=\operatorname{ad}_X$, $B=\operatorname{ad}_Y$, $C=\operatorname{ad}_Z$. Then

$$
\begin{aligned}
\kappa([Z,X],Y)+\kappa(X,[Z,Y])&=\operatorname{tr}([C,A]B+A[C,B])\\
&=\operatorname{tr}(CAB-ABC)=0.
\end{aligned}
$$

This also gives $\kappa([X,Y],Z)=\kappa(X,[Y,Z])$, the equivalent [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md) identity.

For the unheaded structural requests, a [simple Lie algebra](../../../../../simple-lie-algebra.md) is nonabelian and has no [ideals of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md) other than zero and itself. A [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) has no nonzero solvable [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md); in finite dimension over $\mathbb R$ or $\mathbb C$ this is equivalently a direct sum of [simple Lie algebras](../../../../../simple-lie-algebra.md).

Suppose first that the [Killing form](../../../../../killing-form.md) is [nondegenerate](../../../../../nondegenerate-bilinear-form.md). If $I$ is an abelian [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md) and $X\in I$, then $\operatorname{ad}_X$ maps $\mathfrak g$ into $I$ and vanishes on $I$. Every $\operatorname{ad}_Y$ preserves $I$. Therefore $\operatorname{ad}_X\operatorname{ad}_Y$ has zero diagonal blocks relative to a basis adapted to $I$, and

$$
\kappa(X,Y)=0\qquad(X\in I,\ Y\in\mathfrak g).
$$

Nondegeneracy forces $I=0$. If a nonzero solvable [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md) existed, its last nonzero [derived series of a Lie algebra](../../../../../derived-series-of-a-lie-algebra.md) term would be a nonzero abelian [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md), again impossible. Hence the [solvable radical](../../../../../radical-of-a-lie-algebra.md) is zero, proving

$$
\boxed{\kappa\text{ nondegenerate}\quad\Longrightarrow\quad\mathfrak g\text{ semisimple}.}
$$

This argument proves the needed implication rather than assuming the [Cartan criterion for semisimplicity](../../../../../cartan-criterion-for-semisimplicity.md).

One can also see the direct-sum formulation explicitly through [orthogonal ideal splitting for a nondegenerate Killing form](../../../../../orthogonal-ideal-splitting-for-a-nondegenerate-killing-form.md). For an [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md) $I$, invariance makes $I^\perp$ an [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md). If $X\in I\cap I^\perp$, then $\kappa([X,Y],Z)=\kappa(X,[Y,Z])=0$ for $Y\in I$, $Z\in\mathfrak g$, so $[X,I]=0$. Thus $I\cap I^\perp$ is an abelian [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md), and must vanish. Consequently $\mathfrak g=I\oplus I^\perp$ and the two summands commute. Select a minimal nonzero ideal; it is nonabelian, and any ideal inside it is an ideal of $\mathfrak g$ because the complementary summand commutes with it. It is therefore simple. The restricted form is the remaining summand’s own [Killing form](../../../../../killing-form.md), because the two ideals commute. Repeating the splitting there terminates in a direct sum of simple ideals.

Conversely the [radical of the Killing form](../../../../../radical-of-the-killing-form.md)

$$
K=\{X:\kappa(X,Y)=0\text{ for all }Y\}
$$

is an [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md) by the invariance just proved. For a [simple Lie algebra](../../../../../simple-lie-algebra.md) it is either zero or the whole algebra. The permitted hypothesis that $\kappa$ is not identically zero excludes the second alternative. Thus

$$
\boxed{\mathfrak g\text{ simple and }\kappa\not\equiv0\quad\Longrightarrow\quad\kappa\text{ nondegenerate}.}
$$

The computations in the two following parts illustrate both a nondegenerate compact example and a degenerate algebra with an abelian ideal.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
