<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $m=|s|$, $\ell_i=|w_i|$, and let $D(i,j)$ be the minimum number of words chosen from $w_1,\ldots,w_i$, in their given order, whose [concatenation](../../../../../concatenation.md) equals the length-$j$ [prefix of a list](../../../../../prefix-of-a-list.md) of $s$. Use $\infty$ for impossibility. The boundary values are

$$
D(0,0)=0,\qquad D(0,j)=\infty\quad(j>0).
$$

For $i\geq1$,

$$
D(i,j)=\min\left\{
D(i-1,j),\quad
1+D(i-1,j-\ell_i)\ \text{if }j\geq\ell_i\text{ and }s[j-\ell_i:j]=w_i
\right\}.
$$

Here $s[a:b]$ denotes indices $a,\ldots,b-1$. The first case omits $w_i$. In the second, the last selected word is $w_i$, so removing it leaves a solution using only earlier words for the shorter prefix. These are exhaustive alternatives. Conversely either alternative constructs a valid solution, proving the [dynamic programming](../../../../../dynamic-programming.md) recurrence. Even an empty word causes no cycle because both alternatives use row $i-1$.

Fill rows in increasing $i$ and store the chosen alternative for every finite entry. If $D(n,m)=\infty$, report no solution. Otherwise trace back from $(n,m)$: a skip moves to $(i-1,j)$; a take records index $i$ and moves to $(i-1,j-\ell_i)$. Reverse the recorded indices to obtain the required [subsequence](../../../../../subsequence.md). Ties may choose either valid predecessor.

There are $(n+1)(m+1)$ states. A substring comparison costs $O(\ell_i)$, so under the given bounds $m=O(n)$ and $\ell_i=O(1)$ the running time is **$O(n^2)$**, with $O(n^2)$ storage including reconstruction choices. Two rows give $O(m)$ working storage if only the optimum count is needed. For the source example, the optimum is **three words, indices $(2,5,6)$**, whose concatenation is `010111`. This is [ordered word concatenation dynamic programming](../../../../../ordered-word-concatenation-dynamic-programming.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
