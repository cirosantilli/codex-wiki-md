<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

Let $G$ act on its underlying set by left multiplication. The resulting homomorphism

$$
\lambda:G\longrightarrow S_G\cong S_n,
\qquad
\lambda_g(x)=gx,
$$

is injective because $\lambda_g(e)=g$. This is [Cayley theorem](../../../../../cayley-s-theorem.md). If $g\ne e$, then $gx=x$ would imply $g=e$ after right cancellation, so every nonidentity permutation in the image is fixed-point free.

If $|G|$ is even, pair every element with its inverse. Elements not equal to their inverses occur in pairs. Since the identity is self-inverse and the group has even size, there must be another self-inverse element $g\ne e$. It has order two.

A permutation is odd when its [sign](../../../../../sign-homomorphism.md) is $-1$. If a subgroup $H\leq S_m$ contains an odd element, the restriction

$$
\operatorname{sgn}:H\to\{1,-1\}
$$

is surjective. Its kernel is the set of even elements and has index two. Each coset has the same size, so precisely half of $H$ is odd.

Now let $n=4k+2$. An element of order two in the fixed-point-free regular representation is a product of

$$
\frac n2=2k+1
$$

disjoint transpositions, so it is odd. The image $H\cong G$ therefore has an index-two normal subgroup of even permutations. Its order is $2k+1>1$, so it is nontrivial and proper. Hence

$$
\boxed{G\text{ is not simple}}.
$$

Nonabelian simple groups of even order do exist; the smallest example is the alternating group $A_5$, of order sixty.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
