<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A [run of a word](../../../../../../run-of-a-word.md) is a maximal consecutive block of equal letters. For every $N\geq1$, use the following [finite coloring](../../../../../../finite-coloring.md) of $[3]^N$, with at most nine colors:

$$
\boxed{\chi(w)=\bigl(w_1,\ R(w)\pmod3\bigr),\qquad
R(w)=1+\sum_{j=1}^{N-1}\mathbf1_{\{w_j\ne w_{j+1}\}}.}
$$

We show that this [run-count obstruction to interval-active lines](../../../../../../run-count-obstruction-to-interval-active-lines.md) excludes every [monochromatic](../../../../../../monochromatic-set.md) [combinatorial line](../../../../../../combinatorial-line.md) with an interval active set $[a,b]$. If $a=1$, its three words already have different first coordinates, so their colors differ. Suppose $a>1$ and denote the letter immediately to the left by $p$. All contributions to $R(w)$ away from the two possible boundaries of $[a,b]$ are independent of its active letter $x$; no internal active boundary contributes a change.

If $b=N$, the only variable contribution is $\mathbf1_{\{p\ne x\}}$, which is $0$ at $x=p$ and $1$ at another letter. If $b<N$, write $q$ for the letter immediately to the right. The variable contribution is

$$
\mathbf1_{\{p\ne x\}}+\mathbf1_{\{x\ne q\}}.
$$

When $p=q$, its values are $0$ and $2$. When $p\ne q$, it equals $1$ at $x=p$ or $x=q$, and equals $2$ at the third letter. In every case these values are distinct modulo $3$. Hence **no dimension works for [alphabet](../../../../../../alphabet.md) size three and nine colors**, which disproves the proposed universal strengthening. For the PDF's illustrative line, choosing either adjacent letter merges one active run with a neighboring run, while choosing any other letter merges neither; this is exactly the boundary effect measured above. Recording the first letter also handles active intervals meeting the beginning, including the entire coordinate set.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
