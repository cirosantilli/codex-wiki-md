<h1 id="33c/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Under

$$
a_j=\frac12e^{u_j/2},
$$

the [chain rule](../../../../../../../chain-rule.md) gives $dot a_j=(a_j/2)\dot u_j$. Part (ii) and $a_j>0$ therefore imply

$$
\frac12\dot u_j=a_{j+1}^2-a_{j-1}^2
=\frac14\left(e^{u_{j+1}}-e^{u_{j-1}}\right).
$$

Consequently

$$
\boxed{
\dot u_j=\frac12\left(e^{u_{j+1}}-e^{u_{j-1}}\right),
\qquad 1\leq j\leq n-1.
}
$$

The conventions $u_0=u_n=-\infty$ give $e^{u_0}=e^{u_n}=0$, exactly matching $a_0=a_n=0$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [33C](../../../33c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
