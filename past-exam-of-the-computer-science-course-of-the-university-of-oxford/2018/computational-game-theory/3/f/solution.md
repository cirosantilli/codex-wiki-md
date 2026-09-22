<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Remove any plane types with zero count, retaining the increasing order of the remaining lengths; if none remain, return the empty allocation. For the retained types put $s_0=0$ and $N_i=\sum_{\ell=i}^k n_\ell$. Then every plane of type $j$ has [Shapley value](../../../../../shapley-value.md)

$$
\boxed{\phi_j=\lambda\sum_{i=1}^j\frac{s_i-s_{i-1}}{N_i}.}
$$

Compute suffix counts $N_i$ in a backward pass. In a forward pass, accumulate $A\gets A+\lambda(s_i-s_{i-1})/N_i$ and output $A$ as the common payment for type $i$.

For correctness, layer $i$ costs $\lambda(s_i-s_{i-1})$ and is required by exactly $N_i$ planes. A particular requiring plane is earliest among these in a random ordering with probability $1/N_i$. Its expected [marginal contribution](../../../../../marginal-contribution.md) to the layer is therefore that layer's cost divided by $N_i$. Summing the layers it requires proves the formula. This is the [Shapley value of an airport game](../../../../../shapley-value-of-an-airport-game.md).

The two passes use $O(k)$ arithmetic operations. If every individual payment must be explicitly listed, add the unavoidable $O(|N|)$ output work. For counts given in binary, the compact per-type output is polynomial in the input size; expanding an exponentially large number of identical entries need not be. With integer lengths and rational $\lambda$, all fractions can be computed exactly with polynomial bit complexity: a common denominator divides a product of at most $k$ suffix counts, whose bit length is $O(k\log|N|)$, in addition to the input denominator of $\lambda$. For arbitrary real $\lambda$, the same rational factors give symbolic multiples of it.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
