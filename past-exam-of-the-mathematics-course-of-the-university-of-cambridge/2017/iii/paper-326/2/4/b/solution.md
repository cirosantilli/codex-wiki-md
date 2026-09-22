<h1 id="2/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [approximate source bound for coercive Tikhonov regularization](../../../../../../../approximate-source-bound-for-coercive-tikhonov-regularization.md) first allows a fixed sufficiently large $r$ to make $\eta_r$ small, then a sufficiently small $\alpha$ to make $\sqrt\alpha\beta r$ small. This order of limits proves $R_\alpha f\to K^\dagger f$ for every datum in its domain.

For the noise error let $v=R_\alpha g$. Its [normal equation for coercive Tikhonov regularization](../../../../../../../normal-equation-for-coercive-tikhonov-regularization.md) gives

$$
\|Kv\|^2+\alpha\|Bv\|^2=\langle g,Kv\rangle\leq\|g\|\|Kv\|.
$$

Completing the square shows $\alpha\beta^2\|v\|^2\leq\|g\|^2/4$, hence $\|R_\alpha\|\leq1/(2\beta\sqrt\alpha)$. The [noise-bias decomposition for linear regularization](../../../../../../../noise-bias-decomposition-for-linear-regularization.md) now gives

$$
\|R_\alpha f^\delta-K^\dagger f\|\leq\frac{\delta}{2\beta\sqrt\alpha}+\|R_\alpha f-K^\dagger f\|.
$$

Therefore the sufficient [regularization parameter choice](../../../../../../../regularization-parameter-choice.md) is

$$
\boxed{\alpha(\delta)\to0,\qquad\delta^2/\alpha(\delta)\to0.}
$$

For example $\alpha(\delta)=\delta^q$ with $0<q<2$ works. Coercivity makes $K^*K+\alpha B^*B$ boundedly invertible for each positive $\alpha$, so these are continuous linear reconstruction operators and form a [convergent regularization of an inverse problem](../../../../../../../convergent-regularization-of-an-inverse-problem.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2](../../../2.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
