<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take [parity symmetry in quantum field theory](../../../../parity-symmetry-in-quantum-field-theory.md) to preserve free time evolution, so the conjugate initial data reflect along with the field. Substitute the [mode expansion of a free field](../../../../mode-expansion-of-a-free-field.md) into the defining [parity operator](../../../../parity-operator.md) relation and change the integration variable $\mathbf p\mapsto-\mathbf p$. Since $E_{-\mathbf p}=E_{\mathbf p}$, coefficient comparison, or comparison of both the field and its conjugate initial data, gives the intrinsic-even convention

$$
\boxed{\begin{aligned}
\mathcal P a_{\mathbf p}\mathcal P^\dagger&=a_{-\mathbf p},&
\mathcal P b_{\mathbf p}\mathcal P^\dagger&=b_{-\mathbf p},\\
\mathcal P a_{\mathbf p}^\dagger\mathcal P^\dagger&=a_{-\mathbf p}^\dagger,&
\mathcal P b_{\mathbf p}^\dagger\mathcal P^\dagger&=b_{-\mathbf p}^\dagger.
\end{aligned}}
$$

Here [parity symmetry in quantum field theory](../../../../parity-symmetry-in-quantum-field-theory.md) reverses spatial [momentum](../../../../momentum-split.md) and preserves time. The [creation operator](../../../../creation-operator.md) formulas follow by taking [Hermitian adjoints](../../../../adjoint-operator.md). The given field relation has fixed the intrinsic phase to $+1$.

For one [real scalar field](../../../../real-scalar-field.md), let $R$ act on one-particle [wave functions](../../../../wave-function-split.md) by $(Rf)(\mathbf p)=f(-\mathbf p)$. It is a [Hermitian operator](../../../../hermitian-operator.md) with $R^2=1$, so $P_-=(1-R)/2$ is the [orthogonal projector](../../../../orthogonal-projection.md) onto odd [wave functions](../../../../wave-function-split.md). Its [second quantization](../../../../second-quantization.md) is the odd-mode [number operator](../../../../number-operator.md)

$$
N_{\rm odd}=\frac12\int_{\mathbf p}a_{\mathbf p}^\dagger(a_{\mathbf p}-a_{-\mathbf p})
=\frac14\int_{\mathbf p}(a_{\mathbf p}^\dagger-a_{-\mathbf p}^\dagger)(a_{\mathbf p}-a_{-\mathbf p}).
$$

The full [momentum space](../../../../momentum-space.md) is integrated in both expressions; the factors prevent double counting the pairs $\{\mathbf p,-\mathbf p\}$. A suitable [parity operator](../../../../parity-operator.md) is

$$
\boxed{\mathcal P=\exp(i\pi N_{\rm odd})
=\exp\left[\frac{i\pi}{2}\int_{\mathbf p}a_{\mathbf p}^\dagger(a_{\mathbf p}-a_{-\mathbf p})\right].}
$$

For verification, $[N_{\rm odd},a_{\mathbf p}]=-(a_{\mathbf p}-a_{-\mathbf p})/2$. Thus the even combination $a_{\mathbf p}+a_{-\mathbf p}$ is unchanged, and the odd combination $a_{\mathbf p}-a_{-\mathbf p}$ changes sign under conjugation by $e^{i\pi N_{\rm odd}}$, exactly reproducing $a_{\mathbf p}\mapsto a_{-\mathbf p}$. The same holds for [creation operators](../../../../creation-operator.md). The odd-mode [number operator](../../../../number-operator.md) has integer [eigenvalues](../../../../eigenvalue.md), so $\mathcal P^2=1$, and $\mathcal P|0\rangle=|0\rangle$. Multiplying by an overall constant phase would not change its conjugation action. This is [parity as odd-mode number parity](../../../../parity-as-odd-mode-number-parity.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
