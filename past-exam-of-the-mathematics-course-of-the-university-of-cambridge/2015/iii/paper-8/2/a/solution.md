<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix $t,x$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) in the integration variable $v_*$ gives

$$
|K_tg(x,v)|^2
\leq\left(\int_{\mathbb R^d}|k(t,x,v,v_*)|^2\,dv_*\right)
\left(\int_{\mathbb R^d}|g(x,v_*)|^2\,dv_*\right).
$$

Integrate first in $v$, then in $x$. The uniform kernel hypothesis bounds the first factor after velocity integration by $C^2$, independently of $t,x$. Hence

$$
\boxed{\|K_tg\|_{L^2_{x,v}}^2\leq C^2\|g\|_{L^2_{x,v}}^2,\qquad \|K_t\|\leq C.}
$$

The [linear Boltzmann collision operator](../../../../../../linear-boltzmann-collision-operator.md) is linear by its integral definition, so this proves it is a [bounded linear operator](../../../../../../continuous-linear-operator.md) on $L^2_{x,v}$. The estimate is the [Hilbert-Schmidt kernel bound](../../../../../../hilbert-schmidt-kernel-bound.md) applied at each spatial point. The printed real-kernel square is $|k|^2$ for a complex kernel. Measurability of the coefficients is understood so that the displayed integrals are defined.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
