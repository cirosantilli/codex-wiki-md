<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [skew Young diagram](../../../../../skew-young-diagram.md) $\lambda/\mu$ is the difference of two nested [Young diagrams](../../../../../young-diagram.md). A [semistandard Young tableau](../../../../../semistandard-young-tableau.md) is a filling of precisely those cells by positive integers, weakly increasing along each occupied row and strictly increasing down each occupied column. It can be viewed as its filled diagram, or equivalently as a chain

$$
\mu=\nu^{(0)}\subseteq\nu^{(1)}\subseteq\nu^{(2)}
\subseteq\cdots\subseteq\lambda,
$$

where $\nu^{(r)}/\nu^{(r-1)}$ is a [horizontal strip](../../../../../horizontal-strip.md) consisting of the cells labeled $r$. Indeed, the weak row and strict column inequalities ensure that the cells labeled at most $r$, together with $\mu$, form a partition diagram, and equal labels cannot share a column. Conversely such a chain gives the tableau.

For a tableau $T$, let $c_r(T)$ count its entries $r$, put $x^T=\prod_r x_r^{c_r(T)}$, and define

$$
s_{\lambda/\mu}(x)=\sum_Tx^T,\qquad s_\lambda=s_{\lambda/\varnothing}.
$$

There are finitely many tableaux for any fixed number of allowed letters, and the sum has total degree $|\lambda|-|\mu|$.

To prove symmetry directly, use a [Bender-Knuth involution](../../../../../bender-knuth-involution.md) for each adjacent pair of letters $i,i+1$. Pair any $i$ and $i+1$ that occur in the same column and leave them fixed; strictness makes them consecutive in that column. In a row the remaining unpaired entries have the form $i^a(i+1)^b$, between any fixed paired letters. Replace that block by $i^b(i+1)^a$. Rows stay weakly ordered. A free $i$ can be changed to $i+1$ without equaling the entry below, because such a below entry would have been paired with it; likewise changing a free $i+1$ to $i$ cannot equal the entry above. Other neighboring letters are outside $\{i,i+1\}$, so strict columns are preserved. The paired cells remain the same, and repeating the operation restores each free block. The paired letters contribute equally to the two contents, while every free block exchanges its contributions. Thus the involution is a weight-preserving [bijection](../../../../../bijection.md) after exchanging $x_i,x_{i+1}$. Adjacent exchanges generate all finite variable [permutations](../../../../../permutation.md), proving

$$
\boxed{s_{\lambda/\mu}\in\Lambda_{|\lambda|-|\mu|}.}
$$

The skew [Jacobi–Trudi identity](../../../../../jacobi-trudi-identity.md) gives a second proof, since its [determinant](../../../../../determinant.md) entries are already symmetric.

Define the [Kostka number](../../../../../kostka-number.md) $K_{\lambda\mu}$ to count straight-shape [Semistandard Young tableaux](../../../../../semistandard-young-tableau.md) with shape $\lambda$ and content $\mu$, meaning $\mu_i$ copies of label $i$. Suppose such a tableau exists. Strict columns imply that an entry in row $r$ is at least $r$. Therefore all entries from $1,\ldots,r$ lie in the first $r$ rows, giving

$$
\mu_1+\cdots+\mu_r\le\lambda_1+\cdots+\lambda_r
\quad\text{for every }r.
$$

Hence

$$
\boxed{K_{\lambda\mu}\ne0\ \Longrightarrow\ \lambda\ge\mu
\quad\text{in dominance order}.}
$$

For content $\lambda$, the $\lambda_1$ copies of $1$ have nowhere to go except row one and fill it. The $\lambda_2$ copies of $2$ then fill row two, and induction fills row $r$ with $r$. This filling exists and is unique, so $\boxed{K_{\lambda\lambda}=1}$.

Symmetry identifies equal coefficients for each rearrangement of a content, hence

$$
s_\lambda=\sum_{\mu\vdash|\lambda|}K_{\lambda\mu}m_\mu.
$$

The [monomial symmetric functions](../../../../../monomial-symmetric-function.md) form a [basis](../../../../../basis.md). In any total order extending dominance, this change-of-basis [matrix](../../../../../matrix.md) is triangular with diagonal one. It is invertible in each degree, so

$$
\boxed{\{s_\lambda:\lambda\in\operatorname{Par}\}\text{ is a }\mathbb Q
\text{-basis of }\Lambda.}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
