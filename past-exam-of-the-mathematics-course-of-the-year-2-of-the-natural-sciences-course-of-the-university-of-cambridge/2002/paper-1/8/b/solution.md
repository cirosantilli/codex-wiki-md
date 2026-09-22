<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose the homogeneous solutions $u(x)=x\ln x$, which vanishes at $1$, and $v(x)=x(\ln x-1)$, which vanishes at $e$. Their [Wronskian](../../../../../wronskian.md) in the order $uv'-u'v$ is $x$. For a source point $1<\xi<e$, seek the [Green's function](../../../../../green-s-function-split.md) as

$$
G(x,\xi)=\begin{cases}A(\xi)u(x),&x<\xi,\\B(\xi)v(x),&x>\xi.\end{cases}
$$

It is continuous at $x=\xi$; otherwise its second [distributional derivative](../../../../../distributional-derivative.md) would contain a derivative of the [Dirac delta function](../../../../../dirac-delta-function.md), which the source does not contain. Integrating the differential equation across the source, using continuity and the leading coefficient one, gives the jump condition

$$
G_x(\xi^+,\xi)-G_x(\xi^-,\xi)=1.
$$

Continuity and this derivative jump require

$$
A u(\xi)=Bv(\xi),\qquad Bv'(\xi)-Au'(\xi)=1.
$$

Solving with the [Wronskian](../../../../../wronskian.md) $\xi$ gives $A=v(\xi)/\xi=\ln\xi-1$ and $B=u(\xi)/\xi=\ln\xi$. Therefore

$$
\boxed{G(x,\xi)=\begin{cases}x\ln x(\ln\xi-1),&1\leq x\leq\xi,\\x(\ln x-1)\ln\xi,&\xi\leq x\leq e.\end{cases}}
$$

The two values at $x=\xi$ are identical. The derivative jump is explicitly

$$
(\ln\xi)\ln\xi-(\ln\xi+1)(\ln\xi-1)=1.
$$

Both endpoint values vanish and the differential expression is zero off the diagonal, completing the verification of the [Green's function](../../../../../green-s-function-split.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
