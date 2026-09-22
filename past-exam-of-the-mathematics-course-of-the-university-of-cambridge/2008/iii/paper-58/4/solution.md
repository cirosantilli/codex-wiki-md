<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [EPR criterion of reality](../../../../../epr-criterion-of-reality.md) proposes that a quantity has an element of physical reality if its value can be predicted with certainty without disturbing the system. To use remote predictions this way, one additionally assumes locality: the choice and execution of a [measurement in quantum mechanics](../../../../../quantum-measurement-split.md) on separated particles cannot disturb the local physical properties of the remaining particle. The contradiction below is with this combination of the criterion and locality, rather than with a definition of reality alone.

Use the [computational basis](../../../../../computational-basis.md) $|0\rangle=|\uparrow\rangle$, $|1\rangle=|\downarrow\rangle$ and the conventional [Pauli matrices](../../../../../pauli-matrices.md)

$$
X|0\rangle=|1\rangle,\quad X|1\rangle=|0\rangle,\qquad
Y|0\rangle=i|1\rangle,\quad Y|1\rangle=-i|0\rangle.
$$

For each site $j$, let $O_j$ be the [tensor product](../../../../../tensor-product.md) of $X$ at that site and $Y$ at all other sites. For $N=4M+3$, the number of $Y$ factors is $N-1=4M+2$, so

$$
O_j|0^N\rangle=i^{N-1}|1^N\rangle=-|1^N\rangle,\qquad
O_j|1^N\rangle=(-i)^{N-1}|0^N\rangle=-|0^N\rangle.
$$

The minus sign in the given [GHZ state](../../../../../greenberger-horne-zeilinger-state.md) then implies

$$
O_j|\psi\rangle=|\psi\rangle\quad\text{for every }j,
\qquad X^{\otimes N}|\psi\rangle=-|\psi\rangle.
$$

Hence **every one-$X$, remaining-$Y$ product has measurement outcome $+1$ with certainty, while the all-$X$ product has outcome $-1$ with certainty**. These are experimentally separate local [Pauli measurements](../../../../../measurement-of-a-pauli-observable.md) on identically prepared copies, not joint measurements of $X$ and $Y$ on the same particle.

For a chosen site, the other $N-1$ sites can determine its $X$ outcome with certainty by measuring $Y$ and using the corresponding $O_j$ relation. They can determine its $Y$ outcome with certainty by selecting an $O_\ell$ with $\ell\ne j$, measuring $X$ at $\ell$ and $Y$ at all other remote sites. Since $N\geq3$, both choices are available. Locality and the [EPR criterion of reality](../../../../../epr-criterion-of-reality.md) therefore assign each site definite values $x_j,y_j\in\{+1,-1\}$, independent of which remote choice is made, even though [quantum theory](../../../../../quantum-theory-split.md) does not jointly measure the local $X$ and $Y$.

The certain one-$X$ correlations require those assigned values to obey

$$
x_j\prod_{k\ne j}y_k=+1\qquad(j=1,\ldots,N).
$$

Multiplying these scalar equations gives

$$
1=\prod_{j=1}^N x_j\prod_{k=1}^N y_k^{N-1}=\prod_{j=1}^N x_j,
$$

since $N-1$ is even and $y_k^2=1$. Thus the all-$X$ product would necessarily be $+1$. But its quantum value is $-1$, giving

$$
\boxed{\prod_jx_j=+1\ \text{from local predetermined values},\qquad
\prod_jx_j=-1\ \text{from quantum theory}.}
$$

The equations cannot hold even for one assignment of values, so allowing a probability distribution over assignments cannot remove the contradiction. This is the [GHZ contradiction for N congruent to 3 modulo 4](../../../../../ghz-contradiction-for-n-congruent-to-3-modulo-4.md) for every $M\geq0$. Multiplying classical assigned values is crucial: one must not commute the incompatible local [Pauli operators](../../../../../pauli-operator.md) as though they were ordinary numbers. Their noncommutativity is exactly what permits the quantum correlations to evade the classical product argument.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
