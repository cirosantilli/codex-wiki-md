<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\mathcal A$ contain the $n$ [database attributes](../../../../../database-attribute.md) of $R$, and let $F$ contain the given [functional dependencies](../../../../../functional-dependency.md) for $R$. To compute the [attribute closure](../../../../../attribute-closure.md) $X^+$, start with $X$ and repeatedly add $V$ for every [functional dependency](../../../../../functional-dependency.md) $U\to V$ with $U\subseteq X^+$, stopping when a full scan adds nothing.

Enumerate every $X\subseteq\mathcal A\setminus\{a\}$. For each, test whether $X$ is not a [superkey](../../../../../superkey.md) but becomes one on adding $a$:

$$
\boxed{\text{return yes if }X^+\ne\mathcal A\quad\text{and}\quad(X\cup\{a\})^+=\mathcal A.}
$$

If no enumerated $X$ passes both tests, return no. A direct implementation is
```
for each subset X of attributes(R) minus {a}:
    if closure(X, F) != attributes(R):
        if closure(X union {a}, F) == attributes(R):
            return yes
return no
```
If a [candidate key](../../../../../candidate-key.md) $K$ contains $a$, choose $X=K\setminus\{a\}$. Minimality makes $X$ fail the [superkey](../../../../../superkey.md) test while $X\cup\{a\}=K$ passes it, so the [algorithm](../../../../../algorithm-split.md) finds a witness.

Conversely, suppose an enumerated $X$ passes. Starting from $X\cup\{a\}$, repeatedly discard any [database attribute](../../../../../database-attribute.md) other than $a$ whose removal preserves the [superkey](../../../../../superkey.md) property. The process terminates at a [superkey](../../../../../superkey.md) $K$ minimal with respect to these deletions. Removing $a$ cannot leave a [superkey](../../../../../superkey.md): $K\setminus\{a\}\subseteq X$, and a subset of $X$, which is not a [superkey](../../../../../superkey.md), cannot determine more [database attributes](../../../../../database-attribute.md) than $X$. Hence $K$ is a [candidate key](../../../../../candidate-key.md) containing $a$. The [algorithm](../../../../../algorithm-split.md) need not carry out this minimization to return the correct yes/no answer; it establishes why the witness test suffices.

For an explicit [analysis of algorithms](../../../../../analysis-of-algorithms.md), let $L$ be the total encoded length of the [functional dependencies](../../../../../functional-dependency.md), counting their left and right [database attribute](../../../../../database-attribute.md) occurrences and delimiters. With Boolean membership arrays, one complete dependency scan costs $O(L)$. There are at most $n$ productive scans, followed by one unproductive scan, so a naive [attribute closure](../../../../../attribute-closure.md) costs $O(nL+n)$. There are $2^{n-1}$ subsets and at most two [attribute closure](../../../../../attribute-closure.md) computations per subset. Thus

$$
\boxed{\text{time }O\!\left(2^n n(L+1)\right),\qquad\text{space }O(n+L).}
$$

This is an exponential-time [algorithm](../../../../../algorithm-split.md) in the number of [database attributes](../../../../../database-attribute.md), not a polynomial-time claim. Subsets can be generated successively rather than stored all at once. The argument applies to [functional dependencies](../../../../../functional-dependency.md) within the [database relation](../../../../../database-relation.md) $R$; dependencies belonging to unrelated [database relations](../../../../../database-relation.md) do not constrain its [candidate keys](../../../../../candidate-key.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Databases](../../../databases-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
