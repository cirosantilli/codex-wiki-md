<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

For any function $f:X\to\mathcal P(X)$, form the diagonal subset

$$
D=\{x\in X:x\notin f(x)\}.
$$

If $f$ were [surjective](../../../../../surjective-function.md), some $d\in X$ would satisfy $f(d)=D$. Then $d\in D$ would hold exactly when $d\notin D$, which is impossible. Thus **no set surjects onto its power set**, including the empty-set case. This is [Cantor's theorem](../../../../../cantor-s-theorem.md) proved by the [Cantor diagonal argument](../../../../../cantor-diagonal-argument.md).

Use [real-number pairing by separated digits](../../../../../real-number-pairing-by-separated-digits.md) for an explicit [injection](../../../../../injective-function.md) $\mathbb R^2\to\mathbb R$. First map a real number to $(0,1)$ by $q(x)=\tfrac12+\pi^{-1}\arctan x$, and use its unique [binary expansion](../../../../../binary-expansion.md) that is not eventually all ones. If $q(x)=\sum_{n\geq1}a_n2^{-n}$ and $q(y)=\sum_{n\geq1}b_n2^{-n}$, define

$$
\boxed{J(x,y)=\sum_{n\geq1}\left(\frac{a_n}{3^{2n-1}}+\frac{b_n}{3^{2n}}\right).}
$$

This places the two binary digit strings in alternating ternary positions. Such ternary strings, using only digits zero and one, are unique: at a first differing position $k$, the difference $3^{-k}$ exceeds the maximum tail $\sum_{j>k}3^{-j}=\tfrac12 3^{-k}$. Thus the output recovers both digit strings and both inputs. The use of base three avoids any endpoint ambiguity caused by interleaving digits in base two.

For a fixed $A\subseteq\mathbb R^2$, the [affine sections of a planar set](../../../../../affine-section-of-a-planar-set.md) are indexed by

$$
\mathcal I=\{(\mathbf a,\mathbf b)\in\mathbb R^2\times\mathbb R^2:\mathbf b\ne0\}.
$$

There is an [injection](../../../../../injective-function.md) $\iota:\mathcal I\to\mathbb R$, for example by applying $J$ to each coordinate pair and then once more to those two results. Suppose every subset of $\mathbb R$ were a section of $A$. Define a function from $\mathbb R$ to $\mathcal P(\mathbb R)$ by assigning to $\iota(\mathbf a,\mathbf b)$ the corresponding section, and assigning the empty set to every real outside $\iota(\mathcal I)$. [Injectivity](../../../../../injective-function.md) of $\iota$ makes this definition unambiguous. It would be a [surjection](../../../../../surjective-function.md) onto $\mathcal P(\mathbb R)$, contradicting the first argument. **No planar set has every subset of the real line as a section.** Allowing different parametrizations of the same line does not evade this obstruction.

For all [countable sets](../../../../../countable-set.md), however, **such a planar set does exist**. To build one, first encode every real sequence $s=(s_1,s_2,\ldots)$ by one real number. Let $a_{nk}$ be the canonical binary digits of $q(s_n)$, and choose the explicit indexing

$$
j(n,k)=\frac{(n+k-2)(n+k-1)}2+n\quad(n,k\geq1).
$$

This is a [bijection](../../../../../bijection.md) from positive integer pairs to positive integers. Define the [coding of real sequences by ternary digits](../../../../../coding-of-real-sequences-by-ternary-digits.md)

$$
c(s)=\sum_{n,k\geq1}\frac{a_{nk}}{3^{j(n,k)}}.
$$

The same first-differing-digit argument proves that $c$ is [injective](../../../../../injective-function.md); all its values lie in $[0,1/2]$. Now take

$$
\boxed{A=\{(c(s),s_n):s\in\mathbb R^{\mathbb N},\ n\geq1\}.}
$$

For every nonempty [countable set](../../../../../countable-set.md) $S\subseteq\mathbb R$, choose an enumeration $s$ of $S$, repeating terms if $S$ is finite. On the vertical line with $\mathbf a=(c(s),0)$ and $\mathbf b=(0,1)$, the section of $A$ is precisely $S$: injective sequence coding means no other sequence can contribute extra values in this column. The empty set is the section on the line $x=2$, since all code columns have first coordinate at most $1/2$. This constructs the required [universal planar set for countable real sections](../../../../../universal-planar-set-for-countable-real-sections.md). No assertion about its other, nonvertical sections is needed.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
