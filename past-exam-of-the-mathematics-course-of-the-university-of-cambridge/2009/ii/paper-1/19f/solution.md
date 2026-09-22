<h1 id="19f/solution">Solution</h1>

↑ **Parent:** [19F](../19f.md)

The [permutation representation](../../../../../permutation-representation.md) on $\mathbb C^X$ sends the basis vector $e_x$ to $e_{gx}$. Its [character](../../../../../character-of-a-representation.md) is $\pi_X(g)=|X^g|$, because precisely the fixed basis vectors contribute to the trace. [Burnside lemma](../../../../../burnside-s-lemma.md) says that the number of orbits is $|G|^{-1}\sum_g|X^g|$. To prove it, double-count $(g,x)$ with $gx=x$: the count is $\sum_g|X^g|=\sum_x|G_x|$. Each orbit contributes $|Gx||G_x|=|G|$ by the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md).

A pair is fixed under the diagonal action exactly when both entries are fixed. Since permutation characters are real,

$$
\langle\pi_{X_1},\pi_{X_2}\rangle=\frac1{|G|}\sum_g |X_1^g||X_2^g|
=\#(G\backslash(X_1\times X_2)),
$$

by [Burnside lemma](../../../../../burnside-s-lemma.md) on the product.

The [general linear group](../../../../../general-linear-group.md) $\operatorname{GL}_2(q)$ acts on the $q+1$ lines of $\mathbb F_q^2$. It is doubly transitive: choosing nonzero representatives of any two distinct lines gives a basis, and a linear map can send that basis to representatives of any other ordered pair. Thus there are two orbits on ordered pairs, the diagonal and its complement. The [character inner product](../../../../../character-inner-product.md) of this permutation character with itself is two, while the multiplicity of the trivial character is one by transitivity. The sum of squares of irreducible multiplicities is therefore two; the remaining summand is one [irreducible representation](../../../../../irreducible-representation.md), of dimension $(q+1)-1$. **Its dimension is $\boxed q$.**

For $S_n$ acting on two-element subsets, an ordered pair of subsets is classified by intersection size $0,1,2$. All three occur for $n\geq4$, and a permutation carries any pair of a given type to any other. Hence $\langle\pi_Z,\pi_Z\rangle=3$. The natural point [permutation representation](../../../../../permutation-representation.md) is the trivial representation plus the [standard representation of the symmetric group](../../../../../standard-representation-of-the-symmetric-group.md), of dimension $n-1$: its irreducibility also follows from double transitivity and inner product two.

Embed this point representation into $\mathbb C^Z$ by $e_i\mapsto\sum_{j\ne i}e_{\{i,j\}}$. The map is equivariant, and its kernel consists of vectors with $c_i+c_j=0$ for every distinct $i,j$. Three distinct indices force every $c_i=0$, so it is injective for $n\geq3$. Thus the trivial and standard representations each occur in $\mathbb C^Z$. The norm three leaves exactly one further irreducible, with multiplicity one. It is the orthogonal complement of that embedded subspace, equivalently the vectors $a_{ij}=a_{ji}$ satisfying $\sum_{j\ne i}a_{ij}=0$ for every $i$. Its dimension is

$$
\binom n2-n=\frac{n(n-3)}2.
$$

**The constituent dimensions are $\boxed{1,\ n-1,\ n(n-3)/2}$**, each once. For $n=3$, complementation identifies two-element subsets with points, so there are only the trivial and 2-dimensional standard constituents.

## ↑ Ancestors (10)

1. [19F](../19f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
