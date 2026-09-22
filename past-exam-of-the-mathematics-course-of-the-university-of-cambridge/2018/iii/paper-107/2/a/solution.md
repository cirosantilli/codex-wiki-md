<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume uniform ellipticity $a^{ij}\xi_i\xi_j\geq\lambda|\xi|^2$ with $\lambda>0$, bounded coefficients, and $c\leq0$. The [weak maximum principle for elliptic operators](../../../../../../weak-maximum-principle-for-elliptic-operators.md) is

$$
\boxed{\sup_\Omega u\leq\max\{0,\sup_{\partial\Omega}u\}.}
$$

When $c=0$, zero can be omitted. The sign restriction is necessary, as shown by the [failure of the weak maximum principle with a positive zeroth-order coefficient](../../../../../../failure-of-the-weak-maximum-principle-with-a-positive-zeroth-order-coefficient.md).

Let $M=\max(0,\sup_{\partial\Omega}u)$ and $w=u-M$, so $Lw=Lu-cM\geq0$ and $w\leq0$ on the boundary. For sufficiently large $k$, $q=e^{kx_1}$ satisfies

$$
Lq=q(k^2a^{11}+kb^1+c)>0.
$$

If $w$ is positive somewhere, $w+\varepsilon q$ retains a positive interior maximum above all its boundary values for small $\varepsilon>0$. At that point its [gradient](../../../../../../gradient.md) is zero and its [Hessian matrix](../../../../../../hessian-matrix.md) is negative semidefinite; ellipticity and $c\leq0$ give $L(w+\varepsilon q)\leq0$, contradicting its strict positivity. This [exponential perturbation proof of the weak maximum principle with drift](../../../../../../exponential-perturbation-proof-of-the-weak-maximum-principle-with-drift.md) also works with $M=\sup_{\partial\Omega}u$ of either sign when $c=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
