<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For [integer partitions](../../../../../integer-partition.md) $\mu\subseteq\lambda$, set $\lambda/\mu=\{(i,j):\mu_i<j\le\lambda_i\}$. A [semistandard Young tableau](../../../../../semistandard-young-tableau.md) on it has weakly increasing rows, strictly increasing columns and positive integer entries. Its weight is $x^T=\prod_{(i,j)}x_{T(i,j)}$; their sum is the [Skew Schur function](../../../../../skew-schur-function.md) $s_{\lambda/\mu}$. Define

$$
h_r(x)=\sum_{i_1\le\cdots\le i_r}x_{i_1}\cdots x_{i_r}\quad(r>0),
\qquad h_0=1,\qquad h_r=0\quad(r<0).
$$

The [Jacobi–Trudi identity](../../../../../jacobi-trudi-identity.md), including its skew form, is

$$
\boxed{s_{\lambda/\mu}
=\det\!\left[h_{\lambda_i-\mu_j-i+j}\right]_{1\le i,j\le\ell},}
$$

where $\ell$ is any common padded length at least $\ell(\lambda)$. Taking $\mu$ empty gives the ordinary [Schur function](../../../../../schur-polynomial.md) formula.

For a proof, first use finitely many variables $x_1,\ldots,x_N$. A directed northeast path from $A_j=(\mu_j-j,1)$ to $B_i=(\lambda_i-i,N)$ has one horizontal step for each unit of the horizontal displacement. Give such a step at height $r$ weight $x_r$, and vertical steps weight one. The weakly increasing sequence of step heights shows that the sum of its weights is $h_{\lambda_i-\mu_j-i+j}$.

The [determinant](../../../../../determinant.md) result needed is the [nonintersecting lattice-path determinant](../../../../../nonintersecting-lattice-path-determinant.md): in an acyclic weighted network, the [determinant](../../../../../determinant.md) of the single-path sums is the signed sum over vertex-disjoint path families, with sign the [permutation](../../../../../permutation.md) of the paired endpoints. To prove it, expand the [determinant](../../../../../determinant.md) and its products of path sums. An intersecting family has a first intersection in a fixed topological order. Choose the first two indexed paths there and swap their tails. Their total weight stays the same, their endpoint [permutation](../../../../../permutation.md) changes by one [transposition](../../../../../transposition-permutation.md), and the operation is its own inverse. All intersecting families cancel. Only the disjoint families remain.

In this planar network the starting and finishing points occur in the same strict left-to-right order, so disjoint paths have identity endpoint pairing. For the path in row $i$, associate its horizontal step from coordinate $j-i-1$ to $j-i$ with cell $(i,j)$. Reading its height gives the tableau entry. Weak increase follows from northward movement; nonintersection with the path for the next row is exactly the strict column condition. Conversely a tableau constructs the paths, and the strict column inequalities keep them disjoint. This weight-preserving [bijection](../../../../../bijection.md) proves the [determinant](../../../../../determinant.md) formula. Arbitrary $N$ gives its stable [symmetric function](../../../../../symmetric-function.md) version.

The dual [determinant](../../../../../determinant.md) will also be useful below. Allow steps $(0,1)$ or $(1,1)$, assigning weight $x_r$ to a diagonal step reaching level $r$. A single path uses distinct levels, so its sum is the [elementary symmetric function](../../../../../elementary-symmetric-polynomial.md) $e_r$, rather than $h_r$. The same cancellation proof leaves tableaux with strict rows and weak columns. Transposing them gives

$$
s_{\lambda'/\mu'}=\det[e_{\lambda_i-\mu_j-i+j}],
\qquad
s_{\lambda/\mu}=\det[e_{\lambda_i'-\mu_j'-i+j}],
$$

with $e_0=1$ and $e_r=0$ for $r<0$.

Put $n=|\lambda|-|\mu|$. A squarefree weight $x_1\cdots x_n$ in $s_{\lambda/\mu}$ uses every label once, so it is counted by the number $f^{\lambda/\mu}$ of [standard skew Young tableaux](../../../../../standard-skew-young-tableau.md). In one [determinant](../../../../../determinant.md) product $\prod_i h_{r_i}$, the signed [permutation](../../../../../permutation.md) gives $\sum_i r_i=n$. If any $r_i<0$ the product is zero; otherwise the squarefree coefficient is the number of ways to distribute the distinct labels into groups of sizes $r_i$, namely $n!/\prod_i r_i!$. [Coefficient extraction](../../../../../coefficient-extraction.md) therefore gives the [standard skew tableau determinant](../../../../../standard-skew-tableau-determinant.md)

$$
\boxed{f^{\lambda/\mu}
=n!\det\!\left[\frac1{(\lambda_i-\mu_j-i+j)!}\right]_{1\le i,j\le\ell}.}
$$

Negative factorial arguments mean zero entries, and $0!=1$. The empty skew shape has count one, as this convention requires.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
