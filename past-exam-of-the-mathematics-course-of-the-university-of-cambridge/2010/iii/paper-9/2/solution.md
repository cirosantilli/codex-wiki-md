<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Here is the matrix form of [Rado's theorem](../../../../../rado-s-theorem.md). A [matrix](../../../../../matrix.md) $A$ with entries in the [rational numbers](../../../../../rational-number.md) and columns $a_1,\ldots,a_n$ is a [partition regular matrix](../../../../../partition-regular-matrix.md) if every [finite coloring](../../../../../finite-coloring.md) of the [positive integers](../../../../../positive-integer.md) admits a vector $x\in\mathbb N^n$ whose coordinates are [monochromatic](../../../../../monochromatic-set.md) and for which $Ax=0$. Its [columns condition](../../../../../columns-property.md) asks for an ordered partition into nonempty blocks $B_1,\ldots,B_s$, with

$$
b_1:=\sum_{i\in B_1}a_i=0,\qquad b_j:=\sum_{i\in B_j}a_i\in\operatorname{span}_{\mathbb Q}\{a_i:i\in B_1\cup\cdots\cup B_{j-1}\}\quad(j>1).
$$

**[Rado's theorem](../../../../../rado-s-theorem.md) states that these two conditions are equivalent.** Coordinates need not be distinct; positivity is required for every coordinate.

First prove necessity using the [finite separating-functional proof of the columns condition](../../../../../finite-separating-functional-proof-of-the-columns-condition.md). Clearing denominators does not change either the [kernel](../../../../../kernel-of-a-linear-map.md) or the [columns condition](../../../../../columns-property.md), so assume that $A$ has [integer](../../../../../integer.md) entries. For each pair of disjoint index sets $I,B\subseteq\{1,\ldots,n\}$, with $B$ nonempty, for which $b_B=\sum_{i\in B}a_i$ is outside the rational [linear span](../../../../../linear-span.md) of the $I$-columns, choose an integer [linear functional](../../../../../linear-functional.md) $\ell_{I,B}$ such that

$$
\ell_{I,B}(a_i)=0\ (i\in I),\qquad \ell_{I,B}(b_B)\ne0.
$$

Such a [linear functional](../../../../../linear-functional.md) exists: extend a [basis](../../../../../basis.md) over the [rational numbers](../../../../../rational-number.md) of the indicated [linear span](../../../../../linear-span.md) by $b_B$, prescribe values zero on the former basis and one on $b_B$, extend to a [basis](../../../../../basis.md) of the ambient [vector space over the rational numbers](../../../../../vector-space-over-the-rational-numbers.md), and then clear the functional's denominators. There are only finitely many pairs $(I,B)$. Choose a [prime number](../../../../../prime-number.md) $p$ larger than the absolute values of all their nonzero evaluations; if there are none, choose any [prime number](../../../../../prime-number.md).

Color $x>0$ by its [last nonzero digit coloring](../../../../../last-nonzero-digit-coloring.md) value, namely

$$
u(x):=x/p^{v_p(x)}\pmod p\in\{1,\ldots,p-1\},
$$

where $v_p$ is the [P-adic valuation](../../../../../p-adic-valuation.md). By [partition regularity](../../../../../partition-regular-matrix.md), choose a positive solution $Ax=0$ all of whose coordinates have the same nonzero digit $u$. Group its indices into nonempty blocks $B_1,\ldots,B_s$ according to increasing distinct [P-adic valuations](../../../../../p-adic-valuation.md) $\nu_1<\cdots<\nu_s$.

Suppose that a block sum $b_j$ is outside the rational [linear span](../../../../../linear-span.md) of the earlier columns, and put $I=B_1\cup\cdots\cup B_{j-1}$, taking $I=\varnothing$ for $j=1$. Apply the selected [linear functional](../../../../../linear-functional.md) $\ell_{I,B_j}$ to $Ax=0$. The earlier terms vanish exactly. Divide the remaining integer equality by $p^{\nu_j}$ and reduce modulo $p$. Later blocks vanish modulo $p$, while each coordinate in $B_j$ contributes its common digit $u$. We obtain

$$
0\equiv u\,\ell_{I,B_j}(b_j)\pmod p,
$$

which is impossible by the choice of $p$ and because $u\not\equiv0\pmod p$. Thus each block sum lies in the earlier [linear span](../../../../../linear-span.md). For the first block, this span is zero, so $b_1=0$. This proves the [columns condition](../../../../../columns-property.md).

For sufficiency, assume the [columns condition](../../../../../columns-property.md) and choose rational coefficients $\lambda_{ij}$, for $i\in B_1\cup\cdots\cup B_{j-1}$, such that

$$
b_j+\sum_{i\in B_1\cup\cdots\cup B_{j-1}}\lambda_{ij}a_i=0\qquad(j>1).
$$

Choose a positive integer $c$ clearing all these coefficients' denominators and a positive integer $p$ with $p\geq|c\lambda_{ij}|$ for every coefficient. Use the permitted [monochromatic m-p-c set theorem](../../../../../monochromatic-m-p-c-set-theorem.md), in the suffix convention for an [m-p-c set](../../../../../m-p-c-set.md), to obtain positive generators $z_1,\ldots,z_s$ such that the full set

$$
D=\bigcup_{h=1}^s\left\{cz_h+\sum_{j>h}\mu_jz_j:\mu_j\in\mathbb Z,\ |\mu_j|\leq p\right\}
$$

is positive and [monochromatic](../../../../../monochromatic-set.md). The positivity of the full [m-p-c set](../../../../../m-p-c-set.md) is important: we do not discard expressions that happen to be negative. For $i\in B_h$, set

$$
x_i=cz_h+\sum_{j>h}c\lambda_{ij}z_j.
$$

All these coordinates belong to $D$, so they are positive and [monochromatic](../../../../../monochromatic-set.md). On collecting coefficients of each $z_j$, their matrix product is

$$
Ax=c z_1b_1+\sum_{j=2}^s c z_j\left(b_j+\sum_{i\in B_1\cup\cdots\cup B_{j-1}}\lambda_{ij}a_i\right)=0.
$$

This explicit [Rado solution inside an m-p-c set](../../../../../rado-solution-inside-an-m-p-c-set.md) proves sufficiency and completes the proof of [Rado's theorem](../../../../../rado-s-theorem.md).

To deduce the [Finite sums theorem](../../../../../finite-sums-theorem.md) directly from the [columns condition](../../../../../columns-property.md), introduce one positive variable $y_F$ for each nonempty $F\subseteq\{1,\ldots,k\}$ and impose

$$
\sum_{i\in F}y_{\{i\}}-y_F=0\qquad(|F|\geq2).
$$

For $k=1$ there are no equations and any positive integer works. For $k\geq2$, write $a_F$ for the column belonging to $y_F$. Partition the columns into blocks $B_j=\{F:\min F=j\}$ in the order $j=1,\ldots,k$. Consider the row indexed by a set $H$ with $|H|\geq2$. The sum of the columns in $B_j$ has row value

$$
\boldsymbol{1}_{\{j\in H\}}-\boldsymbol{1}_{\{\min H=j\}}.
$$

For $j=1$ this is always zero. For $j>1$ it equals one exactly for those $H$ with $\min H<j$ and $j\in H$. Each such $a_H$ is the negative coordinate vector in row $H$, and it belongs to an earlier block. Therefore

$$
\sum_{F\in B_j}a_F=-\sum_{\substack{|H|\geq2,\ \min H<j\\j\in H}}a_H\quad(j>1),
$$

which verifies the [columns condition](../../../../../columns-property.md), rather than assuming the desired [Finite sums theorem](../../../../../finite-sums-theorem.md). Apply [Rado's theorem](../../../../../rado-s-theorem.md) to this system. Its [monochromatic](../../../../../monochromatic-set.md) positive solution satisfies $y_F=\sum_{i\in F}x_i$ with $x_i=y_{\{i\}}$, and hence

$$
\boxed{\operatorname{FS}(x_1,\ldots,x_k)=\left\{\sum_{i\in F}x_i:\varnothing\ne F\subseteq\{1,\ldots,k\}\right\}\text{ is monochromatic}.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
