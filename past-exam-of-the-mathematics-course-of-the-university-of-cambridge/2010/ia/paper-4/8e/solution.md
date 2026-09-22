<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

A [set](../../../../../set-split.md) is [countable](../../../../../countable-set.md) if it admits an [injective function](../../../../../injective-function.md) into $\mathbb N$, equivalently if it is finite or can be listed in a sequence. The empty [set](../../../../../set-split.md) is included; an infinite [countable set](../../../../../countable-set.md) has a [bijection](../../../../../bijection.md) with $\mathbb N$.

Every [rational number](../../../../../rational-number.md) has a representation $p/q$ with $p\in\mathbb Z$ and $q\ge1$. For each $k\ge1$, there are only finitely many such pairs with $|p|+q=k$. List these finite levels successively, ordering each level by $p$, and discard repeated fractions when they first recur. Every [rational number](../../../../../rational-number.md) appears in some finite level, proving $\boxed{\mathbb Q\text{ is countable}}$.

For the uncountability proof, suppose all numbers in $(0,1)$ could be listed as $r_1,r_2,\ldots$. Choose each decimal expansion not to end in an infinite string of nines, and denote its $j$th digit by $d_{ij}$. Set $b_i=1$ when $d_{ii}\ne1$, and $b_i=2$ otherwise. Then the decimal

$$
s=0.b_1b_2b_3\cdots
$$

defines a number in $(0,1)$ with a unique such expansion, since its digits are only $1$ and $2$. It differs from $r_i$ at digit $i$ for every $i$, contradicting the enumeration. This [Cantor diagonal argument](../../../../../cantor-diagonal-argument.md) proves $\boxed{\mathbb R\text{ is uncountable}}$ because its subset $(0,1)$ already is.

For the union of two [countable sets](../../../../../countable-set.md) $C,D$, take [injective functions](../../../../../injective-function.md) $\iota_C:C\to\mathbb N$ and $\iota_D:D\to\mathbb N$. The map

$$
\iota(x)=\begin{cases}
2\iota_C(x),&x\in C,\\
2\iota_D(x)+1,&x\in D\setminus C
\end{cases}
$$

is injective: it is injective within each branch, and their images have different parity. Thus $\boxed{C\cup D\text{ is countable}}$, regardless of overlap.

The property of $A$ says that both $A$ and its complement are [dense subsets](../../../../../dense-set.md) of the real line. Both possible cardinalities occur. To establish the needed density directly, given $x\in\mathbb R$ and $\varepsilon>0$, choose an integer $q>1/\varepsilon$. Then $\lfloor qx\rfloor/q$ is rational and differs from $x$ by less than $1/q<\varepsilon$. For an irrational approximation, choose a rational $r$ within $\varepsilon/2$ of $x$ and a positive integer $q$ large enough that $\sqrt2/q<\varepsilon/2$. The number $r+\sqrt2/q$ is irrational and lies within $\varepsilon$ of $x$; irrationality follows from that of $\sqrt2$, since otherwise subtracting $r$ and multiplying by $q$ would make $\sqrt2$ rational. To recall the latter fact, a reduced fraction $p/q=\sqrt2$ would satisfy $p^2=2q^2$, forcing $p$ even and then $q$ even, contrary to [coprimality](../../../../../coprime-integers.md). Therefore

$$
\boxed{A=\mathbb Q\text{ is a countable example},\qquad
A=\mathbb R\setminus\mathbb Q\text{ is an uncountable example}.}
$$

The second [set](../../../../../set-split.md) is uncountable because, if it were countable, its union with $\mathbb Q$ would make $\mathbb R$ countable. The same two density arguments give the required approximations from $A$ and from its complement in either example.

Finally, the condition on $B$ makes every one of its points an [isolated point](../../../../../isolated-point.md), so $B$ is a [discrete subset](../../../../../discrete-subset.md) of the real line. Enumerate all rational intervals $(p_j,q_j)$ with $p_j<q_j$; enumerate pairs of indices of the rational list by increasing sum and keep those whose endpoints have the required order. For each $b\in B$, its isolating neighbourhood contains a rational interval $(p_j,q_j)$ containing $b$ and no other point of $B$. Assign to $b$ the least such index $j$. Two distinct points cannot receive the same index, because that interval would then contain two members of $B$. This gives an [injective function](../../../../../injective-function.md) $B\to\mathbb N$ and proves that [discrete subsets of the real line are countable](../../../../../discrete-subsets-of-the-real-line-are-countable.md):

$$
\boxed{B\text{ is countable}.}
$$

Using the least index makes the assignment explicit and requires no arbitrary selection of an uncountable family of intervals.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
