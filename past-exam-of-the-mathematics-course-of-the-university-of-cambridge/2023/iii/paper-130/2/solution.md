<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $A$ be a rational matrix with columns $a_1,\ldots,a_n$. It is a [partition regular matrix](../../../../../partition-regular-matrix.md) when every [finite coloring](../../../../../finite-coloring.md) of the [positive integers](../../../../../positive-integer.md) has a monochromatic vector $x$ with $Ax=0$. It has the [columns property](../../../../../columns-property.md) when the column indices have an ordered partition $B_1,\ldots,B_r$ such that

$$
\sum_{i\in B_1}a_i=0
$$

and, for every $s>1$,

$$
\sum_{i\in B_s}a_i\in
\operatorname{span}_{\mathbb Q}\{a_i:i\in B_1\cup\cdots\cup B_{s-1}\}.
$$

[Rado's theorem](../../../../../rado-s-theorem.md) states that $A$ is partition regular if and only if it has the columns property.

First suppose $A$ is partition regular, and clear its denominators. For a [prime number](../../../../../prime-number.md) $p$, apply the [last nonzero digit coloring](../../../../../last-nonzero-digit-coloring.md) in base $p$: if $x=p^{v_p(x)}u$ with $p\nmid u$, its color is $u\bmod p$. Choose a monochromatic solution and group its coordinates into blocks $B_1,\ldots,B_r$ of equal $p$-adic valuation, in increasing order of valuation. Only finitely many ordered partitions are possible, so one partition occurs for infinitely many primes.

For any such prime, divide $\sum_i x_i a_i=0$ by the lowest power of $p$ and reduce modulo $p$. All coordinates in $B_1$ have the same nonzero leading digit $d$, while later blocks vanish, so

$$
d\sum_{i\in B_1}a_i\equiv0\pmod p.
$$

The integer vector $\sum_{i\in B_1}a_i$ is divisible by infinitely many primes and therefore equals zero.

Now fix $s>1$, and let $t$ be the common valuation on $B_s$. Reduction modulo $p^{t+1}$ gives

$$
p^t d\sum_{i\in B_s}a_i+
\sum_{i\in B_1\cup\cdots\cup B_{s-1}}x_i a_i
\equiv0\pmod {p^{t+1}}.
$$

If the first sum of columns were outside the rational [linear span](../../../../../linear-span.md) of the earlier columns, an integer [linear functional](../../../../../linear-functional.md) would vanish on every earlier column but not on that sum. Applying it to the congruence would say that infinitely many primes divide one fixed nonzero integer, a contradiction. Thus the displayed partition has the columns property.

Conversely, suppose $A$ has the columns property. For $s>1$, choose rational numbers $q_{is}$ such that

$$
\sum_{i\in B_s}a_i=
\sum_{i\in B_1\cup\cdots\cup B_{s-1}}q_{is}a_i.
$$

Let $d_{is}$ equal $1$ for $i\in B_s$, equal $-q_{is}$ in the earlier blocks, and equal zero in the later blocks. For $s=1$, let $d_{i1}$ be the indicator of $B_1$. Then

$$
\sum_i d_{is}a_i=0
$$

for every $s$. Choose a positive integer $c$ clearing all denominators and a positive integer $p$ with $|cd_{is}|\leq p$ whenever $s$ is later than the block containing $i$.

By the [monochromatic m-p-c set theorem](../../../../../monochromatic-m-p-c-set-theorem.md), the coloring contains a monochromatic $(r,p,c)$-set with generators $z_1,\ldots,z_r$. Define

$$
y_i=c\sum_{s=1}^r d_{is}z_s.
$$

If $i\in B_t$, then

$$
y_i=cz_t+\sum_{s>t}cd_{is}z_s,
$$

so every $y_i$ lies in that one monochromatic [M-p-c set](../../../../../m-p-c-set.md). Moreover,

$$
\sum_i y_i a_i
=c\sum_s z_s\sum_i d_{is}a_i=0.
$$

Thus $A$ is partition regular, proving Rado's theorem.

For the equation $4x+3y-6z=0$, a monochromatic solution in the last nonzero base-$p$ digit coloring would, at the least $p$-adic valuation among $x,y,z$, force a nonempty subset sum of $4,3,-6$ to vanish modulo $p$. The seven possible sums are

$$
4,\ 3,\ -6,\ 7,\ -2,\ -3,\ 1.
$$

None is divisible by $5$, so base $5$ gives no monochromatic solution. The smaller primes do admit solutions: $(x,y,z)=(3,2,3)$ works for base $2$, whose coloring has one color, and $(3,4,4)$ is monochromatic in base $3$. Hence the smallest prime is

$$
\boxed{5}.
$$

For $x+2y-7z=0$, use the last nonzero base-$11$ digit itself. The nonempty subset sums of $1,2,-7$ are

$$
1,\ 2,\ -7,\ 3,\ -6,\ -5,\ -4,
$$

none zero modulo $11$. This is the required $10$-coloring.

For a $5$-coloring, identify each nonzero residue $d$ modulo $11$ with $-d$, giving the five colors

$$
\{1,10\},\ \{2,9\},\ \{3,8\},\ \{4,7\},\ \{5,6\}.
$$

If a monochromatic solution existed, reduction at the least $11$-adic valuation would give a signed nonempty subset sum of $1,2,-7$ equal to zero modulo $11$. Singles have absolute residues $1,2,7$; pairs have absolute residues $1,3,5,6,8,9$; and triples have absolute residues $4,6,8,10$. None is zero modulo $11$, which proves that this $5$-coloring works.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 130](../../paper-130-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
