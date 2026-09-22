<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Identify the nonrelativistic [mass](../../../mass.md) with the [rest mass](../../../invariant-mass.md), $m=m_0$. Expanding the [relativistic kinetic energy](../../../relativistic-kinetic-energy.md) in $p^2/(m^2c^2)$ gives

$$
T=\frac{p^2}{2m}-\frac{p^4}{8m^3c^2}+O(c^{-4}),\qquad H'=-\frac{p^4}{8m^3c^2}.
$$

First-order [perturbation theory](../../../perturbation-theory.md) requires $\Delta E_0=\langle0|H'|0\rangle$. Put $\alpha=\sqrt{m\hbar\omega/2}$, so $p=i\alpha(a^\dagger-a)$. The annihilation relations are $a|0\rangle=0$ and $\langle0|a^\dagger=0$. In particular, $a^\dagger|0\rangle$ does **not** vanish. A short calculation retaining the operator ordering gives

$$
p^2|0\rangle=\alpha^2\bigl(|0\rangle-\sqrt2|2\rangle\bigr),\qquad
\langle0|p^4|0\rangle=\|p^2|0\rangle\|^2=3\alpha^4.
$$

Equivalently, of the ordered words in $(a^\dagger-a)^4$, only $aa^\dagger aa^\dagger$ and $aa a^\dagger a^\dagger$ have nonzero ground-state expectation values, respectively $1$ and $2$. Words with a [creation operator](../../../creation-operator.md) on the far left or an [annihilation operator](../../../annihilation-operator.md) on the far right vanish; the remaining unbalanced words also vanish. Thus

$$
\boxed{\Delta E_0=-\frac{3\hbar^2\omega^2}{32mc^2},\qquad E_0=\frac12\hbar\omega-\frac{3\hbar^2\omega^2}{32mc^2}+O(c^{-4}).}
$$

The correction is negative because the [relativistic kinetic energy](../../../relativistic-kinetic-energy.md) is smaller than $p^2/(2m)$ at fixed nonzero [momentum](../../../momentum-split.md). This [relativistic oscillator ground-state kinetic correction](../../../relativistic-oscillator-ground-state-kinetic-correction.md) requires $\hbar\omega\ll mc^2$.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2016](../../2016-split.md)
3. [Past exam of the quantum physics course of the University of Oxford](../../split.md)
4. [Quantum physics course of the University of Oxford](../../../quantum-physics-course-of-the-university-of-oxford.md)
5. [Year 2 of the physics course of the University of Oxford](../../../year-2-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
