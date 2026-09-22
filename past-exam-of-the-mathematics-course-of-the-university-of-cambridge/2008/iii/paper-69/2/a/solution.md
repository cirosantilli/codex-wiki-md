<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $e$ be the specific internal energy, $s$ the [specific entropy](../../../../../../specific-entropy.md), $T$ the absolute [temperature](../../../../../../temperature.md), and $w=e+p/\rho$ the [specific enthalpy](../../../../../../specific-enthalpy.md). The [first law of thermodynamics](../../../../../../first-law-of-thermodynamics.md) for a simple fluid of fixed composition is $de=Tds-p\,d(1/\rho)$, so

$$
\boxed{dw=T\,ds+dp/\rho,\qquad \nabla p/\rho=\nabla w-T\nabla s.}
$$

The unmagnetized [Euler equations for an inviscid fluid](../../../../../../euler-equations-for-an-inviscid-fluid.md) are $\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u=-\nabla\Phi-\nabla p/\rho$. Define the [vorticity](../../../../../../vorticity.md) $\boldsymbol\omega=\nabla\times\mathbf u$ and use the [vorticity cross-product identity](../../../../../../vorticity-cross-product-identity.md) $(\mathbf u\cdot\nabla)\mathbf u=\boldsymbol\omega\times\mathbf u+\nabla(u^2/2)$. Substitution gives the [Crocco form of the unsteady Euler equation](../../../../../../crocco-form-of-the-unsteady-euler-equation.md):

$$
\boxed{\partial_t\mathbf u+\boldsymbol\omega\times\mathbf u
+\nabla\left(u^2/2+\Phi+w\right)=T\nabla s.}
$$

Adiabaticity means $Ds/Dt=0$ for smooth flow without dissipative heating. It does not require $s$ to be uniform between different fluid elements, so the entropy-gradient term generally remains. For a [perfect gas](../../../../../../ideal-gas.md) with constant [adiabatic exponent](../../../../../../heat-capacity-ratio.md) $\gamma$, one may write $w=\gamma p/[(\gamma-1)\rho]$, but the thermodynamic derivation does not require that particular [equation of state](../../../../../../equation-of-state.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
