<h1 id="14d/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $\alpha>0$,

$$
G_{\rm CL}(s)
=\frac1{\alpha s+1+k}.
$$

Its only pole is $-(1+k)/\alpha$, so direct inspection gives stability exactly when

$$
\boxed{k>-1}
$$

apart from the excluded boundary.

For the [Nyquist stability criterion](../../../../../../../nyquist-stability-criterion.md), let $L(s)=kG(s)$. The open loop has no right-half-plane poles, so $P=0$. On the clockwise right-half-plane contour, the winding number $N$ of $1+L$ about zero, equivalently of $L$ about $-1$, satisfies

$$
N=P-Z,
$$

where $Z$ is the number of unstable closed-loop poles. The Nyquist locus

$$
L(i\omega)=\frac{k}{1+i\alpha\omega}
$$

is the circle with diameter joining $0$ and $k$ on the real axis, completed by its conjugate half.

If $k>-1$, this circle does not wind around $-1$, so $N=0$, $Z=0$, and the loop is stable. If $k<-1$, it winds once with $N=-1$, so $Z=1$, and the loop is unstable. Nyquist therefore gives precisely the same condition $k>-1$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [14D](../../../14d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
