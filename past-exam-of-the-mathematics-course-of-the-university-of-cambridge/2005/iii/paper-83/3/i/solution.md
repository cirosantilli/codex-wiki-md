<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $\mathbf x'=\mathbf x-\mathbf u t$, with the same time coordinate in both frames. The [normal fluid](../../../../../../normal-component-of-a-superfluid.md) transforms as $\mathbf v_n'(\mathbf x',t)=\mathbf v_n(\mathbf x,t)-\mathbf u$. The field transformation is the unit-modulus Schrödinger boost

$$
\boxed{\psi'(\mathbf x',t)=e^{-i\mathbf u\cdot\mathbf x+i|\mathbf u|^2t/2}\psi(\mathbf x,t),
\qquad\mathbf A=-i\mathbf u,\quad B=-\frac i2|\mathbf u|^2.}
$$

Writing the phase as $F=-i\mathbf u\cdot\mathbf x'-i|\mathbf u|^2t/2$ makes differentiation at fixed primed position transparent:

$$
\nabla'\psi'=e^F(\nabla\psi-i\mathbf u\psi),\qquad
\partial_t'\psi'=e^F\left(\psi_t+\mathbf u\cdot\nabla\psi-\frac i2u^2\psi\right).
$$

It follows that both $-i\partial_t'\psi'$ and $\nabla'^2\psi'/2$ gain the same terms $e^F[-i\mathbf u\cdot\nabla\psi-u^2\psi/2]$. The density is unchanged, $\rho'=|\psi'|^2=\rho$, so the nonlinear local term has the same form.

The remaining [material derivative](../../../../../../material-derivative.md) transforms as

$$
(\partial_t'+\mathbf v_n'\cdot\nabla')\rho'
=[\partial_t+\mathbf u\cdot\nabla+(\mathbf v_n-\mathbf u)\cdot\nabla]\rho
=(\partial_t+\mathbf v_n\cdot\nabla)\rho.
$$

Thus the density-damping term acquires only the common phase factor, proving invariance of the complete equation under a [Galilean boost](../../../../../../galilean-transformation.md). Keeping the normal [velocity](../../../../../../velocity.md) unchanged in both frames would fail this check; the reference flow must transform along with the condensate.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
