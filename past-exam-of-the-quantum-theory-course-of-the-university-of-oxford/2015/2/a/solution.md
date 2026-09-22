<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [position operator](../../../../position-operator.md) $X$ and [momentum operator](../../../../momentum-operator.md) $P$ are [self-adjoint operators](../../../../self-adjoint-operator.md), so the [adjoint operator](../../../../adjoint-operator.md) is

$$
\boxed{a_+=P+im\omega X.}
$$

Use the [canonical commutation relation](../../../../canonical-commutation-relation.md) with the order of factors preserved:

$$
\begin{aligned}
a_+a_-&=(P+im\omega X)(P-im\omega X)\\
&=P^2+m^2\omega^2X^2+im\omega(XP-PX)\\
&=P^2+m^2\omega^2X^2-m\hbar\omega
=\boxed{2m\left(H-\frac12\hbar\omega\right)},\\
a_-a_+&=P^2+m^2\omega^2X^2-im\omega(XP-PX)\\
&=P^2+m^2\omega^2X^2+m\hbar\omega
=\boxed{2m\left(H+\frac12\hbar\omega\right)}.
\end{aligned}
$$

Subtracting the first product from the second proves

$$
\boxed{[a_-,a_+]=2m\hbar\omega I.}
$$

These [creation and annihilation operators](../../../../creation-and-annihilation-operators.md) are unscaled and carry the paper's phase convention; their [commutator](../../../../commutator.md) is not the unit-normalized oscillator commutator.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the quantum theory course of the University of Oxford](../../../split.md)
5. [Quantum theory course of the University of Oxford](../../../../quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
