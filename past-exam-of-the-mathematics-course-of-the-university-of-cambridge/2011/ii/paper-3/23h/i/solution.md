<h1 id="23h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [divisor](../../../../../../divisor.md) $D=\sum_p n_pp$ on the [smooth projective curve](../../../../../../smooth-projective-curve.md),

$$
L(D)=\{f\in k(X)^\times:\operatorname{div}(f)+D\geq0\}\cup\{0\}.
$$

This is a $k$-vector space of [rational functions](../../../../../../rational-function.md) with the prescribed pole bounds. A nonzero rational function on a projective curve has divisor of degree zero. Thus if $\deg D<0$ there can be no nonzero element of $L(D)$.

For any point $p$ with coefficient $n_p$ in $D$, use a [local parameter](../../../../../../local-parameter-on-a-smooth-algebraic-curve.md) $t$ at $p$. The linear map sending $f\in L(D)$ to the residue-field value of $t^{n_p}f$ has kernel $L(D-p)$ and target $k$, since $k$ is algebraically closed. Therefore $\dim L(D)/L(D-p)\leq1$. If $d=\deg D\geq0$, successively subtract a point $d+1$ times. The final divisor has degree $-1$ and no nonzero sections, giving

$$
\boxed{\dim L(D)\leq d+1\quad(d\geq0),\qquad\dim L(D)=0\quad(d<0).}
$$

Equivalently the universally valid bound is $\dim L(D)\leq\max(0,\deg D+1)$. The PDF states the unqualified bound $\dim L(D)\leq\deg D+1$; literally this is false when $\deg D\leq-2$, because its right side is negative. For example $D=-2p$ has $L(D)=0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [23H](../../23h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
