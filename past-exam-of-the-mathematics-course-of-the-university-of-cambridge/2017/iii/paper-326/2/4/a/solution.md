<h1 id="2/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $u^\dagger=K^\dagger f$, $e=R_\alpha f-u^\dagger$, and $z=\beta^{-2}B^*Bu^\dagger$, with $\beta>0$ as required by coercivity and by the printed inverse power. The [Tikhonov regularization with a coercive penalty operator](../../../../../../../tikhonov-regularization-with-a-coercive-penalty-operator.md) normal equation gives

$$
(K^*K+\alpha B^*B)e=-\alpha B^*Bu^\dagger.
$$

This also holds for inconsistent data in $\mathcal D(K^\dagger)$, because $f-Ku^\dagger\perp\mathcal R(K)$ and therefore $K^*f=K^*Ku^\dagger$. Taking the inner product with $e$ gives

$$
\|Ke\|^2+\alpha\|Be\|^2=-\alpha\beta^2\langle z,e\rangle.
$$

For any $w$ with $\|w\|\leq r$, put $d=\|z-K^*w\|$ and use [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) to bound the right-hand side by $\alpha\beta^2(d\|e\|+r\|Ke\|)$. Since $\|Be\|\geq\beta\|e\|$, completing the square in $\|Ke\|$ yields

$$
\alpha\beta^2\|e\|^2\leq\alpha\beta^2d\|e\|+\frac{\alpha^2\beta^4r^2}{4}.
$$

The positive root of this quadratic inequality is at most $d+\sqrt\alpha\beta r/2$. Infimizing over $w$ proves the [approximate source bound for coercive Tikhonov regularization](../../../../../../../approximate-source-bound-for-coercive-tikhonov-regularization.md), in fact slightly more strongly:

$$
\boxed{\|R_\alpha f-K^\dagger f\|\leq\eta_r+\tfrac12\sqrt\alpha\beta r\leq\eta_r+\sqrt\alpha\beta r.}
$$

Injectivity gives $\overline{\mathcal R(K^*)}=\mathcal N(K)^\perp=U$. Given any positive tolerance, approximate $z$ by $K^*w$ for some finite-norm $w$; for all sufficiently large $r$ it is admissible in the infimum. Thus

$$
\boxed{\eta_r\downarrow0\quad(r\to\infty).}
$$

No attainment of that infimum is needed.

## ↑ Ancestors (12)

1. [A](../a.md)
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
