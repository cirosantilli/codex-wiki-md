# North-east lattice path recurrence

↑ **Parent:** [North-east lattice path](north-east-lattice-path.md)

For [positive integers](positive-integer.md) $a,b$, the [north-east lattice path recurrence](north-east-lattice-path-recurrence.md) is

$$
P(a,b)=P(a-1,b)+P(a,b-1),\qquad P(a,0)=P(0,b)=1.
$$

The boundaries have only straight [north-east lattice paths](north-east-lattice-path.md). The origin counts the zero-step [north-east lattice path](north-east-lattice-path.md) once.[§1.2, Lattice Paths: split by the final horizontal or vertical step](discrete-mathematics-an-open-introduction-3rd-edition-by-oscar-levin.md)

**Proof outline.** A [north-east lattice path](north-east-lattice-path.md) ending at $(a,b)$ has a final step either from $(a-1,b)$ or from $(a,b-1)$. Deleting that step gives a shorter [north-east lattice path](north-east-lattice-path.md); appending it reverses the operation. The two classes are disjoint and exhaust all possibilities, so the [rule of sum](addition-principle.md) adds their counts. At $(4,3)$, the arrivals from $(3,3)$ contribute $\binom63=20$, while those from $(4,2)$ contribute $\binom62=15$: altogether $20+15=35$.

Set $P(a,b)=0$ if either [integer](integer-split.md) coordinate is negative. Then the same [recurrence relation](recurrence-relation.md) applies on the nonnegative axes away from $(0,0)$: one predecessor contributes one, and the other contributes zero. Initialize $P(0,0)=1$ separately; applying the [recurrence relation](recurrence-relation.md) there would incorrectly give zero.

Computing the grid once in increasing order of $a+b$ is [dynamic programming](dynamic-programming.md): every entry uses two earlier entries. If a specified [point](point-geometry.md) is forbidden, set its count to zero, then continue the same [recurrence relation](recurrence-relation.md) at allowed [points](point-geometry.md). This counts [north-east lattice paths](north-east-lattice-path.md) avoiding the forbidden [points](point-geometry.md), provided the origin and endpoint are allowed. The last-step argument remains valid because appending a step to an allowed endpoint cannot visit any new intermediate [integer lattice](integer-lattice.md) [point](point-geometry.md).

## ↑ Ancestors (6)

1. [North-east lattice path](north-east-lattice-path.md)
2. [Lattice path](lattice-path.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [North-east lattice path](north-east-lattice-path.md)
- [North-east lattice path recurrence](north-east-lattice-path-recurrence.md)
- [Pascal's triangle](pascal-s-triangle.md)
