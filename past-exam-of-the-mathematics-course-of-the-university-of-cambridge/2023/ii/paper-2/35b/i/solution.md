<h1 id="35b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\Delta=E_+-E_->0$. Hermiticity gives

$$
\langle-|\Delta H|+\rangle=-i\lambda,
$$

so in the ordered basis $(| -\rangle,|+\rangle)$,

$$
H_0+\Delta H=
\begin{pmatrix}
E_-&-i\lambda\\
i\lambda&E_+
\end{pmatrix}.
$$

For a [nondegenerate unperturbed level](../../../../../../nondegenerate-energy-eigenvalue.md), the [first-order nondegenerate perturbation theory](../../../../../../first-order-nondegenerate-perturbation-theory.md) formulas are

$$
E_n^{(1)}=\langle n|\Delta H|n\rangle,
\qquad
|n^{(1)}\rangle
=\sum_{m\ne n}|m\rangle
\frac{\langle m|\Delta H|n\rangle}{E_n-E_m}.
$$

The diagonal matrix elements vanish, so both linear energy corrections are zero. The state corrections are

$$
| -^{(1)}\rangle
=|+\rangle\frac{i\lambda}{E_--E_+}
=-\frac{i\lambda}{\Delta}|+\rangle,
$$



$$
|+^{(1)}\rangle
=|-\rangle\frac{-i\lambda}{E_+-E_-}
=-\frac{i\lambda}{\Delta}|-\rangle.
$$

Thus, through linear order,

$$
\boxed{
\begin{aligned}
E_-^{\rm pert}&=E_-+O(\lambda^2),&
|-\rangle_{\rm pert}&=|-\rangle-\frac{i\lambda}{\Delta}|+\rangle+O(\lambda^2),\\
E_+^{\rm pert}&=E_++O(\lambda^2),&
|+\rangle_{\rm pert}&=|+\rangle-\frac{i\lambda}{\Delta}|-\rangle+O(\lambda^2).
\end{aligned}}
$$

Normalization changes only at quadratic order.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [35B](../../35b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
