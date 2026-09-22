<h1 id="34a/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $\Delta=\Omega-\omega$. Using

$$
e^{iH_0t/\hbar}
\bigl(|e\rangle\langle g|\otimes A\bigr)
e^{-iH_0t/\hbar}
=e^{i\Delta t}|e\rangle\langle g|\otimes A,
$$

the interaction-picture perturbation is

$$
\delta H_I(t)
=\frac{\hbar\Delta}{2}
\left(
e^{i\Delta t}|e\rangle\langle g|\otimes A
+e^{-i\Delta t}|g\rangle\langle e|\otimes A^\dagger
\right).
$$

The initial field is the [coherent state](../../../../../../../coherent-state.md) with amplitude $-1$:

$$
e^{-1/2}e^{-A^\dagger}|0\rangle
=e^{-1/2}\sum_{m=0}^\infty
\frac{(-1)^m}{\sqrt{m!}}|m\rangle.
$$

Hence the initial amplitudes of both $|e,n\rangle$ and $|g,n\rangle$ are

$$
c_{e,n}(0)=c_{g,n}(0)
=\frac{e^{-1/2}(-1)^n}{\sqrt{2n!}}.
$$

Only $|g,n+1\rangle$ contributes at first order to the amplitude of $|e,n\rangle$. Since $A|n+1\rangle=\sqrt{n+1}|n\rangle$,

$$
\begin{aligned}
c_{e,n}^{I}(t)
&=c_{e,n}(0)
-\frac{i\Delta}{2}\sqrt{n+1}\,c_{g,n+1}(0)
\int_0^t e^{i\Delta t'}\,dt'\\
&=c_{e,n}(0)
-\frac12\sqrt{n+1}\,c_{g,n+1}(0)
\bigl(e^{i\Delta t}-1\bigr).
\end{aligned}
$$

But $\sqrt{n+1}\,c_{g,n+1}(0)=-c_{e,n}(0)$, so

$$
c_{e,n}^{I}(t)
=\frac{c_{e,n}(0)}2
\bigl(1+e^{i\Delta t}\bigr).
$$

The free Schrödinger-picture phase does not change the probability. Within this first-order perturbative approximation,

$$
\boxed{
\mathbb P\{\text{atom }e,\text{ field }n\}
=\frac{e^{-1}}{2n!}
\cos^2\!\left(\frac{(\Omega-\omega)t}{2}\right)
}.
$$

At $t=\pi/(\Omega-\omega)$ the cosine is zero, so this probability vanishes to the stated perturbative order.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [34A](../../../34a.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
