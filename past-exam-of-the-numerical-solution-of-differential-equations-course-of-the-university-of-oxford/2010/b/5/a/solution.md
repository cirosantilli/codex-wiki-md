<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The coefficient signs alone do not imply the assertion as printed. Two interior nodes can have rows $L_h\psi_1=\psi_2-\psi_1$ and $L_h\psi_2=\psi_1-\psi_2$, with a separate boundary node. Taking interior values one and boundary value zero satisfies every stated coefficient inequality and $L_h\psi=0$, but its maximum is not on the boundary. Connectedness of the geometric domain does not ensure connectedness of this stencil graph.

The usual extra assumption is that every interior node has a path of positive stencil coefficients to a prescribed boundary node. Under this assumption let $M\geq0$ be the global maximum and suppose an interior node $p$ attains it. Then

$$
0\leq L_h\psi_p
=\sum_{r\ne p}c_{p,r}(\psi_r-M)
+\left(\sum_{r\ne p}c_{p,r}-c_{p,p}\right)M\leq0.
$$

All summands are nonpositive, so equality forces $\psi_r=M$ at every neighbor with $c_{p,r}>0$. Propagate along a path to the boundary to find a boundary node with value $M$. This proves **the [discrete maximum principle](../../../../../discrete-maximum-principle.md) under [boundary-reaching stencil connectivity](../../../../../boundary-reaching-stencil-connectivity.md)**, and exhibits why the literal hypotheses need that qualification.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
