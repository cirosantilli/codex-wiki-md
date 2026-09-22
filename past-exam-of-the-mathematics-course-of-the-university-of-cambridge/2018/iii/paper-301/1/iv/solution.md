<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

First derive the needed [gamma-matrix traces](../../../../../../gamma-matrix-trace.md) directly from the [Clifford algebra](../../../../../../clifford-algebra.md). The [cyclic property of the trace](../../../../../../cyclic-property-of-the-trace.md) gives

$$
2\operatorname{tr}(\gamma^\mu\gamma^\nu)
=\operatorname{tr}\{\gamma^\mu,\gamma^\nu\}
=2\eta^{\mu\nu}\operatorname{tr}I_4,
$$

so $\operatorname{tr}(\gamma^\mu\gamma^\nu)=4\eta^{\mu\nu}$. For $T=\operatorname{tr}(\gamma^\mu\gamma^\nu\gamma^\rho\gamma^\sigma)$, move $\gamma^\mu$ successively through the other three matrices and cycle the final term back to the front:

$$
2T=2\eta^{\mu\nu}\operatorname{tr}(\gamma^\rho\gamma^\sigma)
-2\eta^{\mu\rho}\operatorname{tr}(\gamma^\nu\gamma^\sigma)
+2\eta^{\mu\sigma}\operatorname{tr}(\gamma^\nu\gamma^\rho).
$$

Therefore

$$
\operatorname{tr}(\gamma^\mu\gamma^\nu\gamma^\rho\gamma^\sigma)
=4(\eta^{\mu\nu}\eta^{\rho\sigma}-\eta^{\mu\rho}\eta^{\nu\sigma}+\eta^{\mu\sigma}\eta^{\nu\rho}).
$$

These are all the trace identities required.

For massless external [Dirac spinors](../../../../../../dirac-spinor.md), the [fermion spin sums](../../../../../../fermion-spin-sum.md) are $\sum_su_s(p)\bar u_s(p)=\not p$ and $\sum_rv_r(q)\bar v_r(q)=\not q$. With the initial [spin average](../../../../../../spin-average.md), part (iii) becomes a contraction of

$$
L^{\mu\nu}=4(q^\mu p^\nu+q^\nu p^\mu-\eta^{\mu\nu}p\cdot q),\qquad
H_{\mu\nu}=4(p'_\mu q'_\nu+p'_\nu q'_\mu-\eta_{\mu\nu}p'\cdot q').
$$

Their contraction is

$$
L^{\mu\nu}H_{\mu\nu}
=32\bigl[(q\cdot p')(p\cdot q')+(q\cdot q')(p\cdot p')\bigr].
$$

The massless [Mandelstam variables](../../../../../../mandelstam-variables.md) give $p\cdot p'=q\cdot q'=-t/2$ and $p\cdot q'=q\cdot p'=-u/2$, hence

$$
\overline{|\mathcal M|^2}=\frac{2e^4}{s^2}(t^2+u^2).
$$

In the [center of mass](../../../../../../center-of-mass.md) frame each particle has energy $\sqrt s/2$, and

$$
t=-\frac s2(1-\cos\theta),\qquad u=-\frac s2(1+\cos\theta).
$$

Substitution gives the concise angular answer:

$$
\boxed{\overline{|\mathcal M|^2}=e^4(1+\cos^2\theta).}
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
