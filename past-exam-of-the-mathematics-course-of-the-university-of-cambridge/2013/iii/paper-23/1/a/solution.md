<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [primitive Dirichlet character](../../../../../../primitive-dirichlet-character.md) modulo $q$ is a [Dirichlet character](../../../../../../dirichlet-character.md) which is not induced from a character of a proper divisor of $q$. To determine the inducing [primitive Dirichlet character](../../../../../../primitive-dirichlet-character.md), use the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) to decompose

$$
(\mathbb Z/q\mathbb Z)^\times\cong\prod_{p^k\parallel q}(\mathbb Z/p^k\mathbb Z)^\times.
$$

On each factor choose the least exponent $c_p\in\{0,\ldots,k\}$ through whose reduction the restricted character factors. Exponent zero means the trivial unit group modulo one. Put $q_0=\prod_pp^{c_p}$ and define $\chi_0$ on the units modulo $q_0$ by these descended factors, extending by zero off the units. Every reduction of unit groups is [surjective](../../../../../../surjective-function.md), so the descended character is unique. Its local exponents cannot be decreased, hence it is primitive. The original character is $\chi(n)=\chi_0(n)$ when $(n,q)=1$, and zero otherwise.

Any other inducing modulus must have exponent at least $c_p$ at every [prime](../../../../../../prime-number.md), by restriction to the corresponding local factor. Therefore $q_0$ is the unique minimal modulus, the [conductor of a Dirichlet character](../../../../../../conductor-of-a-dirichlet-character.md), and $\chi_0$ is the unique [primitive Dirichlet character](../../../../../../primitive-dirichlet-character.md) inducing $\chi$. The argument also explains why removing extra [prime](../../../../../../prime-number.md) factors can change values at [integers](../../../../../../integer.md) that were nonunits for $q$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
