<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

Suppose all infinite [binary sequences](../../../../../bitstream.md) could be listed as $\epsilon^{(1)},\epsilon^{(2)},\ldots$, where $\epsilon^{(j)}=(\epsilon^{(j)}_1,\epsilon^{(j)}_2,\ldots)$. Define another [binary sequence](../../../../../bitstream.md) by $d_j=1-\epsilon^{(j)}_j$. It differs from the $j$th listed sequence at its $j$th entry, so it is absent from the list. This contradiction is [Cantor's diagonal argument](../../../../../cantor-s-diagonal-argument.md), proving that

$$
\boxed{\{0,1\}^{\mathbb N}\text{ is uncountable}.}
$$

To transfer this result to $[0,1]$, map a [binary sequence](../../../../../bitstream.md) to

$$
f(\epsilon)=\sum_{j=1}^{\infty}\frac{2\epsilon_j}{3^j}.
$$

This lies in $[0,1]$ because $\sum_{j\geq1}2/3^j=1$. If two sequences first differ at index $j$, with $\epsilon_j=1$ and $\eta_j=0$, then

$$
f(\epsilon)-f(\eta)\geq\frac2{3^j}-\sum_{n=j+1}^{\infty}\frac2{3^n}=\frac1{3^j}>0.
$$

Thus $f$ is an [injection](../../../../../injective-function.md), avoiding the ambiguous expansions that would arise from unrestricted binary digits in base two. An injection from an [uncountable set](../../../../../uncountable-set.md) into $[0,1]$ proves that $\boxed{[0,1]\text{ is uncountable}}$.

For $\Sigma(\mathbb Z)$, a nondecreasing sequence bounded above can take only finitely many integer values, all lying between its first term and an integer upper bound. Every strict increase raises its value by at least one, so only finitely many strict increases occur. It is therefore eventually constant. Every such sequence has the form

$$
(a_1,\ldots,a_N,a_N,a_N,\ldots)
$$

for some finite list of integers. The set of finite integer lists is a [countable set](../../../../../countable-set.md): at stage $j$, list the tuples of length at most $j$ whose entries have absolute value at most $j$, omitting earlier duplicates. Each stage is finite and every finite tuple occurs at some stage. Constant sequences give an injection of $\mathbb Z$ into the collection, so

$$
\boxed{\Sigma(\mathbb Z)\text{ is countably infinite}.}
$$

This is the discrete-order phenomenon that [bounded nondecreasing integer sequences are eventually constant](../../../../../bounded-nondecreasing-integer-sequences-are-eventually-constant.md).

For $\Sigma(\mathbb Q)$, use a different encoding, into rational [partial sums](../../../../../partial-sum.md):

$$
s_n(\epsilon)=\sum_{j=1}^n\frac{\epsilon_j}{3^j}.
$$

Each $s_n$ is a [rational number](../../../../../rational-number.md), the sequence is nondecreasing, and $s_n\leq1/2$. If two binary inputs first differ at $j$, their $j$th partial sums differ by $3^{-j}$, so their output sequences differ. This defines an [injection](../../../../../injective-function.md) of the uncountable binary-sequence set into $\Sigma(\mathbb Q)$. Thus [bounded nondecreasing rational sequences are uncountable](../../../../../bounded-nondecreasing-rational-sequences-are-uncountable.md). Finally, every such rational sequence is also an admissible real sequence, so inclusion into $\Sigma(\mathbb R)$ is injective. Consequently

$$
\boxed{\Sigma(\mathbb Q)\text{ and }\Sigma(\mathbb R)\text{ are both uncountable}.}
$$

Boundedness and monotonicity force eventual constancy for integer values, but not for rational or real values; countability of the set of possible individual terms does not imply countability of all infinite sequences of those terms.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
