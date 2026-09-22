<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**Euclidean Lipschitz continuity does not imply Carnot-Carathéodory Lipschitz continuity.** In the exponential coordinates above take the vertical path $\gamma(t)=(0,0,t)$. It is Euclidean [Lipschitz continuous](../../../../../../lipschitz-continuity.md), but

$$
d_{CC}(\gamma(s),\gamma(t))=c\,|t-s|^{1/2},\qquad
c=d_{CC}(e,(0,0,1))>0.
$$

Indeed left invariance reduces to the central increment, graded dilation gives the square-root factor, and reversal changes the sign without changing the distance.

One can also see the scale directly. A horizontal curve starting at the identity satisfies $\dot z=(x\dot y-y\dot x)/2$. If it ends on the vertical axis, its planar projection is a closed loop and

$$
z=\tfrac12\int(x\,dy-y\,dx).
$$

For a projection of length $L$ starting at zero, $\sup|(x,y)|\le L$, so $|z|\le L^2/2$. Thus reaching a central displacement $z$ requires length at least $\sqrt{2|z|}$, while a square loop with the appropriate signed area gives length at most $4\sqrt{|z|}$. In particular $d_{CC}(\gamma(s),\gamma(t))/|t-s|$ is unbounded as $t\to s$. Vertical displacement records area, which scales quadratically with horizontal length.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
