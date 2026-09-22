<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

To prove (a) implies (c), shrink to a contractible coordinate neighborhood. The real [Poincaré lemma](../../../../../../poincare-lemma.md) gives a real one-form $\eta$ with $\omega=d\eta$. Write $\eta=\eta^{1,0}+\eta^{0,1}$. Because $\omega$ has type $(1,1)$, $\bar\partial\eta^{0,1}=0$ and $\partial\eta^{1,0}=0$. The [Dolbeault-Poincaré lemma](../../../../../../dolbeault-poincare-lemma.md) supplies a [smooth function](../../../../../../smooth-function.md) $\psi$ with $\eta^{0,1}=\bar\partial\psi$. Reality of $\eta$ gives $\eta^{1,0}=\partial\overline\psi$. Thus

$$
 \omega=\partial\bar\partial\psi+\bar\partial\partial\overline\psi
 =\partial\bar\partial(\psi-\overline\psi)
 =i\partial\bar\partial(2\operatorname{Im}\psi).
$$

Taking the real function $f=2\operatorname{Im}\psi$ gives the [local real potential for a closed (1,1)-form](../../../../../../local-real-potential-for-a-closed-1-1-form.md). Conversely, $d(i\partial\bar\partial f)=0$, by $\partial^2=\bar\partial^2=0$ and anticommutation. Hence (a) and (c) are equivalent, completing all three conditions.

For the unheaded radial continuation, take the real potential $f$ as in (c). Rotation invariance makes $f$ constant on every circle of radius $r>0$, so

$$
 \boxed{u(t)=f(e^{t/2}),\qquad t\in\mathbb R,}
$$

is well defined and smooth by composition. This avoids treating a [smooth function](../../../../../../smooth-function.md) as if it had a convergent Taylor series. At nonzero $z$, put $t=\log|z|^2$. The identities $\partial_z t=1/z$ and $\partial_{\bar z}t=1/\bar z$ give

$$
 f_{z\bar z}(z)=\frac{u''(t)}{|z|^2}=e^{-t}u''(t).
$$

Let $q(z)=f_{z\bar z}(z)$, which is smooth on the whole plane. Then

$$
 \omega=iq(z)\,dz\wedge d\bar z,
 \qquad g=2q(z)(dx^2+dy^2).
$$

At the origin, rotation invariance gives the finite [Taylor expansion](../../../../../../taylor-expansion.md) $f(z)=f(0)+b|z|^2+O(|z|^4)$, with $b=q(0)$. Alternatively continuity of $q$ directly gives

$$
 \lim_{t\to-\infty}e^{-t}u''(t)=q(0).
$$

The metric is positive away from the origin exactly when $u''(t)>0$ for all finite $t$, and it is positive at the origin exactly when this limit is positive. Smoothness at the origin is already supplied by the original smooth potential. Consequently the [positivity criterion for a radial Kähler potential](../../../../../../positivity-criterion-for-a-radial-kahler-potential.md) is

$$
 \boxed{u''(t)>0\ \text{for every }t\in\mathbb R,
 \qquad\lim_{t\to-\infty}e^{-t}u''(t)>0.}
$$

Closedness is automatic from the potential, and positivity completes the Kähler condition. No completeness of this metric is asserted. The [rotation-invariant Kähler potential on the complex plane](../../../../../../rotation-invariant-kahler-potential-on-the-complex-plane.md) is understood as real; if a complex radial potential is initially allowed with real $\omega$, its smooth radial imaginary part is harmonic and hence constant, so that constant can be removed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
