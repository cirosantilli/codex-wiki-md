<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the diamond coordinates, the horizontal line through $(u,v)$ has $2(n-|u|)+1$ points and the vertical line has $2(n-|v|)+1$ points. There is a numerical constant $a>0$, independent of $n$ and of the starting point, such that the walk enters the middle diamond $D_{n/2}$ within two steps with probability at least $a$. To see this, suppose $|u|\leq|v|$, so $|u|\leq n/2$. With probability at least $1/2$ the first move uses the longer horizontal line, and a fixed positive fraction of its choices have $|v'|\leq n/4$. From $(u,v')$, the vertical line has length at least $3n/2$, is chosen with probability bounded below, and a fixed positive fraction of its points satisfy $|u'|+|v'|\leq n/2$. The case $|v|\leq|u|$ is symmetric.

Now couple two copies. Independently use the preceding construction until both lie in $D_{n/2}$, an event having probability at least $a^2$ in two steps. From $(u,v)$ and $(u',v')$ in that diamond, their horizontal line ranges overlap in at least $n+1$ values. A [maximal coupling](../../../../../../maximal-coupling.md) of the next moves can therefore, with probability bounded below, send them to $(u,w)$ and $(u',w)$ for the same $|w|\leq n/2$. Their vertical lines are then identical, and another maximal coupling makes the two states equal with probability bounded below. Thus there are constants $k$ and $b>0$, independent of $n$, for which the two copies coalesce during every block of $k$ steps with conditional probability at least $b$.

The coupling time consequently has a geometric tail. By the [coupling inequality for total variation](../../../../../../coupling-inequality-for-total-variation.md), for each fixed $0<\varepsilon<1$,

$$
t_{\mathrm{mix}}(\varepsilon)\leq k\left\lceil\frac{\log(1/\varepsilon)}{-\log(1-b)}\right\rceil=O_\varepsilon(1).
$$

Since a nontrivial chain has mixing time bounded below by a positive constant, the mixing time has constant order.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
