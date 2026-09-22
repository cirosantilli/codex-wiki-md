<h1 id="10f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

This is a [gambler's ruin](../../../../../../gambler-s-ruin.md) hitting problem. For $0<p<1$, let $h_j$ be the [probability](../../../../../../probability.md) of reaching $+3$ before $-3$ when the current difference is $j$. Conditioning on the next [independent](../../../../../../independent-random-variables.md) game gives

$$
h_j=ph_{j+1}+qh_{j-1}\quad(-2\leq j\leq2),\qquad h_{-3}=0,\quad h_3=1.
$$

Stopping occurs almost surely: conditional on being inside the barriers, three consecutive wins by either player force absorption within the next three games. This event has [probability](../../../../../../probability.md) $p^3+q^3>0$, so the chance of surviving $m$ such blocks is at most $(1-p^3-q^3)^m$, which tends to zero.

If $p\ne q$, the characteristic roots of the interior recurrence are $1$ and $r=q/p$, so $h_j=A+Br^j$. Imposing the two boundary values yields

$$
h_j=\frac{1-r^{j+3}}{1-r^6}.
$$

In particular,

$$
h_0=\frac{1-r^3}{1-r^6}=\frac1{1+r^3}
=\frac{p^3}{p^3+q^3}.
$$

For $p=q=1/2$ the recurrence instead has affine solutions, and the boundary values give $h_j=(j+3)/6$, hence $h_0=1/2$. The deterministic cases $p=0,1$ give zero and one respectively. The formula covers all of them continuously:

$$
\boxed{\mathbb P(A\text{ wins overall})=\frac{p^3}{p^3+(1-p)^3},\qquad0\leq p\leq1.}
$$

The stopping argument and the boundary recurrence show why the answer concerns the first barrier reached rather than the win difference after a predetermined number of games.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
