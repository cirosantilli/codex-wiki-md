<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Charnes-Cooper transformation](../../../../../../charnes-cooper-transformation.md) on the positive-denominator region:

$$
t=\frac1{d^Tx+\beta},\qquad y=tx.
$$

It gives $Ay\le bt$, $d^Ty+\beta t=1$ and $c^Ty+\alpha t=(c^Tx+\alpha)/(d^Tx+\beta)$.

We must check that allowing $t=0$ introduces no false feasible solution. If $t=0$, then $Ay\le0$. The [recession cone](../../../../../../recession-cone.md) of the nonempty [linear polyhedron](../../../../../../linear-polyhedron.md) $P=\{x:Ax\le b\}$ is $\{y:Ay\le0\}$. Indeed for $x_0\in P$, $x_0+uy\in P$ for every $u\ge0$. Boundedness of $P$ therefore forces $y=0$, contradicting $d^Ty=1$. Thus every transformed feasible point has $t>0$.

Conversely set $x=y/t$. The constraints give $x\in P$ and $d^Tx+\beta=1/t>0$, with the same objective value. The assumed original optimizer with positive denominator supplies a transformed feasible point. Every transformed point corresponds to an original point and has objective at most that optimizer's value. Hence **the transformed [linear program](../../../../../../linear-programming.md) attains the original optimum, and its optimizer recovers $x=y/t$.** Positivity on every point of $P$ is not needed here; the given positive-denominator optimum suffices.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
