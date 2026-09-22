<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a real [potential energy](../../../../potential-energy.md) and a [stationary state](../../../../stationary-state.md), the [probability current](../../../../probability-current.md) is

$$
j(x)=\frac{\hbar}{2mi}\bigl(\psi^*\psi'-\psi\psi'^*\bigr)=\frac\hbar m\operatorname{Im}(\psi^*\psi').
$$

The time-independent [Schrödinger equation](../../../../schrodinger-equation.md) gives $\psi''=2m(V-E)\psi/\hbar^2$, so $j'=\hbar\operatorname{Im}(\psi^*\psi'')/m=0$. In an exterior [plane wave](../../../../plane-wave.md) superposition, interference terms contribute no current and

$$
j_{\rm left}=\frac{k}{m}(|A|^2-|B|^2),\qquad j_{\rm right}=\frac{k}{m}(|C|^2-|D|^2).
$$

Consequently $|A|^2+|D|^2=|B|^2+|C|^2$ for every choice of incoming amplitudes. If $u=(A,D)^T$, this says $u^\dagger(I-S^\dagger S)u=0$ for every complex [vector](../../../../vector.md) $u$. Since $I-S^\dagger S$ is [Hermitian](../../../../hermitian-operator.md), vanishing of its [quadratic form](../../../../quadratic-form-split.md) implies that the [matrix](../../../../matrix.md) itself vanishes. Therefore

$$
\boxed{S^\dagger S=I,\qquad R+T=1.}
$$

The second identity follows by choosing $u=(1,0)^T$. Since $S$ is a square [matrix](../../../../matrix.md), the first also implies $SS^\dagger=I$, proving [unitarity](../../../../unitary-operator.md). A real [delta potential](../../../../delta-potential.md) preserves this proof: continuity of $\psi$ and the real derivative jump make the current continuous across the interaction point.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further quantum theory course of the University of Oxford](../../../split.md)
5. [Further quantum theory course of the University of Oxford](../../../../further-quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
