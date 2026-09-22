<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Interpret the [language of ordered rings](../../../../../language-of-ordered-rings.md) in the standard [natural numbers](../../../../../natural-number.md), with nonlogical symbols $0,1,+,\times,<$. We give a single [first-order formula](../../../../../first-order-formula.md) $F(n,y)$ defining $y=n!$, rather than a separate expression with $n$ multiplication signs. The key is [Gödel beta-function sequence coding](../../../../../godel-beta-function-sequence-coding.md). The remainder relation

$$
B(b,c,i,r)\quad\Longleftrightarrow\quad r<1+(i+1)c\ \land\ \exists q\,[b=q(1+(i+1)c)+r]
$$

uses only the allowed symbols; all variables range over $\mathbb N$. With $c>0$, it assigns a unique remainder $r$ at each position $i$.

The [factorial graph formula via remainder coding](../../../../../factorial-graph-formula-via-remainder-coding.md) asserts that one code contains the initial value $1$, the final value $y$, and every recurrence step. Here is the fully expanded formula, with no remainder-function or factorial symbol:

$$
\begin{aligned}
F(n,y)\;\equiv\;\exists b\,\exists c\,\exists q_0\,\exists q_1\;\bigl[\;&0<c\ \land\ b=q_0(1+c)+1\\
&\land\ y<1+(n+1)c\ \land\ b=q_1(1+(n+1)c)+y\\
&\land\ \forall i\,\bigl(i<n\ \to\ \exists u\,\exists v\,\exists q_2\,\exists q_3\;[\\
&\qquad u<1+(i+1)c\ \land\ b=q_2(1+(i+1)c)+u\\
&\qquad\land\ v<1+((i+1)+1)c\ \land\ b=q_3(1+((i+1)+1)c)+v\\
&\qquad\land\ v=(i+1)u]\bigr)\;\bigr].
\end{aligned}
$$

The first equation represents remainder $1$ at position zero: its omitted explicit remainder bound follows from $c>0$. The second line represents remainder $y$ at position $n$. The universally checked equations represent the adjacent remainders and impose multiplication by $i+1$. Uniqueness of remainders therefore forces them, successively, to be $0!,1!,\ldots,n!$, proving $F(n,y)\Rightarrow y=n!$ by [mathematical induction](../../../../../mathematical-induction.md). When $n=0$, the recurrence clause is empty and the two endpoint clauses force $y=1$.

Conversely, choose a positive $c$ larger than every value in the finite sequence $0!,1!,\ldots,n!$ and divisible by each positive integer at most $n$. The moduli $d_i=1+(i+1)c$, $0\leq i\leq n$, are pairwise coprime. Indeed, for $i<j$, a common divisor of $d_i,d_j$ divides $(j-i)c$ and is coprime to $c$, so divides $j-i$. Since $j-i$ divides $c$, the common divisor must be one. The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) gives a nonnegative $b$ with $b\equiv i!\pmod{d_i}$ for every $i$. The chosen values are smaller than their moduli, so they are the actual remainders; the appropriate quotient witnesses then make $F(n,n!)$ true. Thus

$$
\boxed{F(n,y)\quad\Longleftrightarrow\quad y=n!}.
$$

**The formula has fixed length, independent of $n$.** For example, writing its displayed syntax in plain text with one-character variables, ordinary parentheses, and explicit logical connectives takes fewer than $1000$ characters and fewer than $500$ logical-symbol tokens. Its length is therefore $O(1)$ as a uniform definition of the graph. Numeral names for particular input values, if substituted for the variables, add their own encoding lengths. Over the ordered ring $\mathbb Z$, restrict every quantifier to nonnegative integers and require $n,y\geq0$; this gives the same definition on its nonnegative part. It is the chosen arithmetic structure, not ring axioms alone, that makes the formula define factorial.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
