<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [context-free grammar](../../../../../context-free-grammar.md) is a quadruple $(N,\Sigma,P,S)$: $N$ is a finite [set](../../../../../set-split.md) of nonterminal symbols, $\Sigma$ is a disjoint finite [alphabet](../../../../../alphabet.md) of terminal symbols, $S\in N$ is the start symbol, and $P$ is a finite [set](../../../../../set-split.md) of productions $A\to\alpha$, with $A\in N$ and $\alpha\in(N\cup\Sigma)^*$. Its [formal language](../../../../../formal-language.md) consists of the terminal [strings](../../../../../string.md) derivable from $S$.

For the even-length [palindromes](../../../../../palindrome.md) in (b)(ii), take terminal [alphabet](../../../../../alphabet.md) $\{0,1\}$ and the [context-free grammar](../../../../../context-free-grammar.md)

$$
\boxed{S\to0S0\mid1S1\mid\varepsilon.}
$$

Every production adds identical symbols at the two ends, so every generated [string](../../../../../string.md) is an even-length [palindrome](../../../../../palindrome.md). Conversely, remove the matching outer pair of any nonempty even-length [palindrome](../../../../../palindrome.md) and repeat; this constructs its derivation, ending with $\varepsilon$.

For the unequal-block [formal language](../../../../../formal-language.md) in (b)(iv), use

$$
\boxed{\begin{aligned}
S&\to A\mid B,\\
A&\to0A1\mid Z,& Z&\to0Z\mid0,\\
B&\to0B1\mid O,& O&\to1O\mid1.
\end{aligned}}
$$

After $k$ uses of $A\to0A1$, and $j\geq1$ zeros from $Z$, the resulting [string](../../../../../string.md) is $0^{k+j}1^k$, so its zero count is larger. Every such unequal pair with $m>n$ occurs by choosing $k=n,j=m-n$. Similarly $B$ generates exactly $0^k1^{k+j}$ with $j\geq1$, covering precisely $m<n$. The start alternatives cover both possibilities and never equal counts. If positive exponents are required, replace the start productions by $S\to0A1\mid0B1$, which adds one matched pair and ensures both counts are positive.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
