<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $[m]$ be an alphabet. A [combinatorial line](../../../../../../combinatorial-line.md) in $[m]^N$ is obtained by choosing a nonempty set of active coordinates, fixing every other coordinate, and putting the same variable letter in all active coordinates. The [Hales-Jewett theorem](../../../../../../hales-jewett-theorem.md) states that, for every pair of [positive integers](../../../../../../positive-integer.md) $m,k$, some $N$ makes every $k$-coloring of $[m]^N$ contain a monochromatic combinatorial line.

We prove it by [mathematical induction](../../../../../../mathematical-induction.md) on $m$. The case $m=1$ is immediate. Suppose the result is known for the alphabet $[m-1]$, with any finite number of colors. Order each line by its variable letter, and call its last point its focus. Say that $r$ lines are color-focused when they share a focus, each line with its focus removed is monochromatic, and those $r$ punctured lines have different colors.

We claim that for every $1\leq r\leq k$ there is $N_r$ such that every $k$-coloring of $[m]^{N_r}$ contains either a monochromatic line or $r$ color-focused lines. For $r=1$, restrict a coloring to $[m-1]^{N_1}$ with $N_1=HJ(m-1,k)$. A monochromatic line there becomes a punctured line over $[m]$ after adjoining the point obtained by putting $m$ in every active coordinate. It is either already monochromatic or is one color-focused line.

Assume $n=N_r$ works for $r$, and put

$$
N=HJ\left(m-1,k^{m^n}\right).
$$

View $[m]^{n+N}$ as $[m]^n\times[m]^N$. For $b\in[m-1]^N$, record the entire color pattern

$$
\bigl(c(a,b)\bigr)_{a\in[m]^n}.
$$

This is a coloring with at most $k^{m^n}$ colors, so the induction hypothesis on the alphabet supplies a line on which this pattern is constant. Adjoin its focus $b^+$, whose active coordinates contain the letter $m$, and write $L$ for the resulting line over $[m]$. Thus $c(a,b)$ is independent of $b\in L\setminus\{b^+\}$ for every $a$. It defines a $k$-coloring $c'(a)$ of $[m]^n$.

If $c'$ has a monochromatic line, fixing any $b\in L\setminus\{b^+\}$ gives one for $c$. Otherwise there are $r$ color-focused lines for $c'$, with common focus $f$. Couple the active coordinates of each of those lines with the active coordinates of $L$; this produces $r$ punctured lines focused at $(f,b^+)$. The line obtained by fixing the first component at $f$ and varying along $L$ supplies one more. Its punctured color differs from the preceding $r$ colors, since equality with one of them would make the corresponding $c'$-line monochromatic. Hence there are $r+1$ color-focused lines. The claim follows by induction on $r$.

Take $r=k$. The common focus has one of the $k$ colors, so it completes the punctured line of that color to a monochromatic line. This proves the Hales-Jewett theorem.

A $d$-dimensional [combinatorial subspace](../../../../../../combinatorial-subspace.md) has $d$ disjoint nonempty active coordinate sets, one for each independent variable. The [Extended Hales-Jewett theorem](../../../../../../extended-hales-jewett-theorem.md) says that, given $m,k,d$, every $k$-coloring of $[m]^n$ contains such a monochromatic subspace when $n$ is large enough. To deduce it, choose

$$
N=HJ(m^d,k)
$$

and identify

$$
[m]^{dN}=\left([m]^d\right)^N.
$$

A monochromatic combinatorial line over the alphabet $[m]^d$ becomes a monochromatic $d$-parameter set over $[m]$: within every active block, its first coordinates form the first variable set, its second coordinates form the second, and so on. Thus $n=dN$ suffices.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
