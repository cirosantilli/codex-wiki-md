<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a rational $\ell\times n$ [matrix](../../../../../matrix.md) $A$, write its columns as $c_1,\ldots,c_n$. It is [partition regular](../../../../../partition-regular-matrix.md) if every [finite colouring](../../../../../finite-coloring.md) of $\mathbb N$ admits positive integers $x_1,\ldots,x_n$, all of one colour, with $A\mathbf x=0$. Repeated coordinates are allowed. The [columns condition](../../../../../columns-property.md) is an ordered partition

$$
[n]=B_1\sqcup\cdots\sqcup B_s
$$

into nonempty blocks such that

$$
\sum_{i\in B_1}c_i=0,\qquad
\sum_{i\in B_j}c_i\in\operatorname{span}_{\mathbb Q}\{c_i:i\in B_1\cup\cdots\cup B_{j-1}\}\quad(j>1).
$$

[Rado's theorem](../../../../../rado-s-theorem.md) states that **a rational matrix is partition regular if and only if it satisfies the [columns condition](../../../../../columns-property.md)**. We prove both implications.

For necessity, clear denominators so the columns are integral. For every disjoint pair of index sets $I,B$ with $B\ne\varnothing$ and

$$
v_B=\sum_{i\in B}c_i\notin\operatorname{span}_{\mathbb Q}\{c_i:i\in I\},
$$

choose a rational [linear functional](../../../../../linear-functional.md) annihilating all columns in $I$ but not $v_B$. Such a functional exists by extending a [basis](../../../../../basis.md) of the indicated [linear span](../../../../../linear-span.md) to include $v_B$, prescribing zero on the former and one on the latter. Clearing its denominators produces an integer-coefficient functional $f_{I,B}$ with $f_{I,B}(v_B)$ a nonzero integer. There are only finitely many pairs $I,B$. Choose a [prime number](../../../../../prime-number.md) $p$ dividing none of these nonzero evaluations; if there are no bad pairs, choose any prime.

Use the [last nonzero digit coloring](../../../../../last-nonzero-digit-coloring.md) for this prime. Namely, write $x=p^{\nu_p(x)}u$ with $p\nmid u$ and colour $x$ by $u\bmod p\in\{1,\ldots,p-1\}$. By [partition regularity](../../../../../partition-regular-matrix.md), obtain a positive [monochromatic](../../../../../monochromatic-set.md) solution. Let the distinct [P-adic valuations](../../../../../p-adic-valuation.md) of its coordinates be

$$
v_1<\cdots<v_s,
$$

and put $B_j=\{i:\nu_p(x_i)=v_j\}$. All unit parts $u_i$ have a common nonzero residue $t$ modulo $p$.

For a block $B_j$, let $I=B_1\cup\cdots\cup B_{j-1}$. If its column sum were outside the earlier [linear span](../../../../../linear-span.md), apply $f_{I,B_j}$ to the equation $\sum_i c_ix_i=0$. Earlier-block contributions are exactly zero. Divide the remaining equation by $p^{v_j}$ and reduce modulo $p$. Higher-valuation terms vanish, leaving

$$
0\equiv t\,f_{I,B_j}\!\left(\sum_{i\in B_j}c_i\right)\pmod p.
$$

This contradicts the choice of $p$ and $t\not\equiv0$. Consequently every block sum lies in the earlier [linear span](../../../../../linear-span.md). For $j=1$ that span is $\{0\}$, so its sum is zero. This proves the [columns condition](../../../../../columns-property.md) by the [finite separating-functional proof of the columns condition](../../../../../finite-separating-functional-proof-of-the-columns-condition.md).

For sufficiency, suppose the blocks satisfy the [columns condition](../../../../../columns-property.md). Choose rational coefficients $\alpha_{ij}$, for $i\in B_1\cup\cdots\cup B_{j-1}$, such that

$$
\sum_{i\in B_j}c_i+\sum_{i\in B_1\cup\cdots\cup B_{j-1}}\alpha_{ij}c_i=0\quad(j>1).
$$

Take a positive integer $c$ clearing all their denominators and an integer $p\ge1$ at least as large as every $|c\alpha_{ij}|$. An [M-p-c set](../../../../../m-p-c-set.md) with generators $z_1,\ldots,z_s$ consists of all values

$$
cz_h+\sum_{j>h}\lambda_jz_j,
\qquad \lambda_j\in\mathbb Z,\quad |\lambda_j|\le p,
$$

with every such value positive. The generators are therefore chosen with $cz_h>p\sum_{j>h}z_j$. Positivity is part of the configuration, not achieved by deleting inconvenient values.

Use the permitted [monochromatic m-p-c set theorem](../../../../../monochromatic-m-p-c-set-theorem.md) to obtain one such [monochromatic](../../../../../monochromatic-set.md) set. For each $i\in B_h$, put

$$
x_i=cz_h+\sum_{j>h}c\alpha_{ij}z_j.
$$

Every $x_i$ is a positive element of that set, because its non-leading coefficients are integers of magnitude at most $p$. In the sum $\sum_i c_ix_i$, the coefficient of $z_1$ is $c\sum_{i\in B_1}c_i=0$, and the coefficient of each $z_j$ with $j>1$ is

$$
c\left(\sum_{i\in B_j}c_i+\sum_{i\in B_1\cup\cdots\cup B_{j-1}}\alpha_{ij}c_i\right)=0.
$$

Thus $A\mathbf x=0$. This is an explicit [Rado solution inside an m-p-c set](../../../../../rado-solution-inside-an-m-p-c-set.md) and proves sufficiency.

For the [Finite sums theorem](../../../../../finite-sums-theorem.md), define

$$
FS(x_1,\ldots,x_k)=\left\{\sum_{i\in I}x_i:\varnothing\ne I\subseteq[k]\right\}.
$$

To deduce its monochromaticity from [Rado's theorem](../../../../../rado-s-theorem.md), introduce variables $z_I$ for all nonempty $I\subseteq[k]$ and equations

$$
z_I-\sum_{i\in I}z_{\{i\}}=0\qquad(|I|\ge2).
$$

Let $A_k$ be their coefficient [matrix](../../../../../matrix.md), and partition its columns by $B_j=\{I:\min I=j\}$. For a fixed $j$, the vector with $I$-coordinate $1$ when $j\in I$, and $0$ otherwise, solves this homogeneous system: in every row both sides count whether $j$ belongs to its indexing set. Hence

$$
\sum_{I\in B_j}c_I+
\sum_{\substack{\min I<j\\j\in I}}c_I=0.
$$

The first block sum is zero, and each later block sum lies in the [linear span](../../../../../linear-span.md) of earlier columns. This proves the [columns partition for finite-sums systems](../../../../../columns-partition-for-finite-sums-systems.md). The positive [monochromatic](../../../../../monochromatic-set.md) solution supplied by [Rado's theorem](../../../../../rado-s-theorem.md) has $x_i=z_{\{i\}}>0$, and its other coordinates are exactly all the nonempty finite sums. Therefore **$FS(x_1,\ldots,x_k)$ is [monochromatic](../../../../../monochromatic-set.md)**. For $k=1$ a singleton is immediate. Equivalently, the full positive [M-p-c set](../../../../../m-p-c-set.md) with $m=k,p=c=1$ directly contains every such sum, by taking its leading index to be the least index in $I$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
