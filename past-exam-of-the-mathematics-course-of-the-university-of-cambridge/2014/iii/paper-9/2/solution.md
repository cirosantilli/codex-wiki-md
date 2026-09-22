<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A rational matrix $A=(a_1\ \cdots\ a_n)$ is [partition regular](../../../../../partition-regular-matrix.md) over the positive integers if every finite colouring of $\mathbb N$ admits a vector $x\in\mathbb N^n$ whose coordinates all have the same colour and satisfy $Ax=0$. Equal coordinates are allowed. [Rado's theorem](../../../../../rado-s-theorem.md) says that this holds exactly when the columns can be partitioned into nonempty blocks $I_0,\ldots,I_t$ with

$$
b_0=\sum_{i\in I_0}a_i=0,\qquad b_j=\sum_{i\in I_j}a_i\in\operatorname{span}_{\mathbb Q}\{a_i:i\in I_0\cup\cdots\cup I_{j-1}\}\quad(j\geq1).
$$

This is the [columns condition](../../../../../columns-property.md). Clearing an overall denominator lets us prove necessity for an integer matrix.

Suppose the [columns condition](../../../../../columns-property.md) fails. There are only finitely many ordered partitions of the finite column index set. For each ordered partition, choose a failing block: its sum $b_j$ is outside the rational span of preceding columns, with that span interpreted as zero for the first block. Finite-dimensional [linear algebra](../../../../../linear-algebra-split.md) gives a rational [linear functional](../../../../../linear-functional.md) vanishing on that span but not on $b_j$. For completeness, take a basis of the span, append $b_j$, extend to a basis of the column space, and prescribe values zero on the first basis vectors and one on $b_j$. Clearing the functional's denominators gives an integer row functional $\ell$ with $\ell(b_j)\ne0$.

Choose one prime $p$ larger than the absolute values of all these finitely many nonzero integers $\ell(b_j)$. Colour each positive integer by its first nonzero base-$p$ digit:

$$
\chi_p(x)=p^{-v_p(x)}x\pmod p\in\{1,\ldots,p-1\}.
$$

Assume a monochromatic solution $x$ exists, and partition its coordinates into blocks of equal [P-adic valuation](../../../../../p-adic-valuation.md), ordered by increasing valuations $v_0<\cdots<v_t$. Their first nonzero digit is a common $d\ne0\pmod p$. For this ordered partition take its chosen failing block $I_j$ and functional $\ell$. Apply $\ell$ to $\sum_i a_ix_i=0$. All preceding-block terms disappear exactly. Divide the remaining integer equation by $p^{v_j}$ and reduce modulo $p$. Later blocks disappear, while the current block gives

$$
0\equiv d\,\ell\left(\sum_{i\in I_j}a_i\right)\pmod p.
$$

This contradicts the prime's choice. Thus the colouring has no monochromatic solution, proving necessity. This is the [finite separating-functional proof of the columns condition](../../../../../finite-separating-functional-proof-of-the-columns-condition.md); it needs neither a limiting argument nor a bound on the valuations themselves.

For sufficiency, suppose the blocks satisfy the [columns condition](../../../../../columns-property.md). Choose rational coefficients $q_{ji}$, for $i$ in preceding blocks, such that

$$
b_j+\sum_{i\in I_0\cup\cdots\cup I_{j-1}}q_{ji}a_i=0\qquad(j\geq1).
$$

Let $c$ be a positive integer clearing their denominators, and choose an integer $P\geq1$ bounding all $|cq_{ji}|$. Use the allowed [monochromatic m-p-c set theorem](../../../../../monochromatic-m-p-c-set-theorem.md) with $t+1$ generators. We use the triangular convention in which the resulting positive integer set contains every number

$$
cu_j+\sum_{k=j+1}^t\lambda_ku_k\qquad(0\leq j\leq t,\quad \lambda_k\in\mathbb Z,\ |\lambda_k|\leq P)
$$

in one colour. This is an [m-p-c set](../../../../../m-p-c-set.md), with the generator indices reversed if the alternative lower-triangular convention is used. The permitted theorem applies to either convention, since it applies to every finite number of generators. Its set lies in $\mathbb N$, so all of the displayed combinations are positive.

For $i\in I_j$, define

$$
x_i=cu_j+\sum_{k=j+1}^t cq_{ki}u_k.
$$

Each coordinate belongs to that monochromatic set. Summing the column contributions and collecting coefficients of $u_k$ gives

$$
\sum_i a_ix_i=c\sum_{k=0}^t u_k\left[b_k+\sum_{i\in I_0\cup\cdots\cup I_{k-1}}q_{ki}a_i\right]=0.
$$

For $k=0$ the inner sum is empty and $b_0=0$. This proves sufficiency by a [Rado solution inside an m-p-c set](../../../../../rado-solution-inside-an-m-p-c-set.md), and completes the theorem.

For the requested application, choose

$$
\boxed{r=1.}
$$

The matrix, in the coordinate order $(x,y,z,w)$, has columns

$$
a_x=(3,1)^T,\quad a_y=(1,-2)^T,\quad a_z=(-3,0)^T,\quad a_w=(0,-1)^T.
$$

The block $I_0=\{x,z,w\}$ has zero sum. The remaining column satisfies $a_y=-a_z/3+2a_w$, so it is in the span of the first block. By [Rado's theorem](../../../../../rado-s-theorem.md), positive monochromatic $x,y,z,w$ satisfy the system. In particular,

$$
\boxed{3x+y=3z,\qquad x-2y=w>0.}
$$

One can see the positivity directly in the same triangular construction: a monochromatic set containing $3u+\lambda v$ for $|\lambda|\leq6$, together with $3v$, gives

$$
x=3u,\quad y=3v,\quad z=3u+v,\quad w=3u-6v.
$$

All four are positive because they belong to that positive [m-p-c set](../../../../../m-p-c-set.md). This is a [partition-regular system forcing an ordered Schur relation](../../../../../partition-regular-system-forcing-an-ordered-schur-relation.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
