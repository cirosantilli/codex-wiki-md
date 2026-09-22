<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The expression $d\phi(X)$ is in general a [vector field along a map](../../../../../../vector-field-along-a-map.md), rather than a [vector field](../../../../../../vector-field.md) on $M$. Its intended meaning in the required formula is pointwise evaluation of the [vector-bundle-valued differential form](../../../../../../vector-bundle-valued-differential-form.md) $\nabla s$:

$$
\bigl(\nabla'_{X}(\phi^*s)\bigr)_p
=(\nabla s)_{\phi(p)}(d\phi_pX_p),
$$

using the canonical identification $(\phi^*E)_p=E_{\phi(p)}$. This interpretation works for every [smooth map](../../../../../../smooth-map-between-manifolds.md), including a constant map or a map with self-intersections.

Choose a [frame of a vector bundle](../../../../../../frame-of-a-vector-bundle.md) over $U$, written as a row $e=(e_1,\ldots,e_r)$. Define its [connection one-form](../../../../../../connection-one-form.md) $\Omega$ by

$$
\nabla(eu)=e(du+\Omega u)
$$

for component columns $u$. The pulled-back frame $e^\phi=(\phi^*e_1,\ldots,\phi^*e_r)$ is a [frame of a vector bundle](../../../../../../frame-of-a-vector-bundle.md) over $\phi^{-1}U$. For any component column $v$ of [smooth functions](../../../../../../smooth-function.md) on that open set, define

$$
\boxed{\nabla'(e^\phi v)=e^\phi\bigl(dv+(\phi^*\Omega)v\bigr).}
$$

Here the matrix entries of $\phi^*\Omega$ are ordinary [pullbacks of a differential form](../../../../../../pullback-of-a-differential-form.md). The displayed operator is linear and satisfies the [Leibniz rule](../../../../../../leibniz-rule.md), hence is locally a [connection on a vector bundle](../../../../../../connection-vector-bundle.md).

To prove these local operators glue, change the original [frame of a vector bundle](../../../../../../frame-of-a-vector-bundle.md) to $\widetilde e=eh$. Expanding $\nabla(eh u)$ gives the [change of frame of a vector-bundle connection](../../../../../../change-of-frame-of-a-vector-bundle-connection.md)

$$
\widetilde\Omega=h^{-1}\Omega h+h^{-1}dh.
$$

The [pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) and the [chain rule](../../../../../../chain-rule.md) give

$$
\phi^*\widetilde\Omega
=(h\circ\phi)^{-1}(\phi^*\Omega)(h\circ\phi)
+(h\circ\phi)^{-1}d(h\circ\phi).
$$

This is precisely the required transformation law for the pulled-back frame $\widetilde e^\phi=e^\phi(h\circ\phi)$. Thus the definitions agree and give a global [pullback connection](../../../../../../pullback-connection.md).

For $s=eu$, substitute $v=u\circ\phi$ in the defining formula and use $d(u\circ\phi)(X)=du(d\phi(X))$. This proves the required identity. Conversely that identity fixes $\nabla'_X(\phi^*e_a)$; the [Leibniz rule](../../../../../../leibniz-rule.md) then fixes the derivative of every $\sum_a v^a\phi^*e_a$, proving uniqueness. If the identity is initially imposed only on global [sections of a vector bundle](../../../../../../section-of-a-vector-bundle.md), multiply each local frame section by a [smooth bump function](../../../../../../smooth-bump-function.md) equal to one near the point in question and supported in $U$, and extend by zero. These global sections agree with the frame locally, so the same uniqueness argument applies. **The pullback connection exists and is unique.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
