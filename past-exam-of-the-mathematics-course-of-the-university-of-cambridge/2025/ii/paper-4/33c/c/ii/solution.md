<h1 id="33c/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Part (a) gives

$$
[L_3,X_3]=[L_3,P_3]=0.
$$

Hence both operators preserve the magnetic quantum number $m$. They are also odd under parity, while $|n,\ell,m\rangle$ has parity $(-1)^\ell$. Their matrix elements between states of equal parity vanish. The [position-momentum selection rules in the first excited hydrogen eigenspace](../../../../../../../position-momentum-selection-rules-in-the-first-excited-hydrogen-eigenspace.md) therefore leave only the coupling between

$$
|s\rangle:=|2,0,0\rangle,
\qquad
|p\rangle:=|2,1,0\rangle.
$$

The $m=\pm1$ states decouple, and all diagonal matrix elements vanish.

In the ordered basis $(|s\rangle,|p\rangle)$, remove the common energy $E_2$ and write

$$
\Delta H(t)=
\begin{pmatrix}
0&z(t)\\
z(t)^*&0
\end{pmatrix}
=
\begin{pmatrix}
0&ce^{i\omega t/\hbar}\\
ce^{-i\omega t/\hbar}&0
\end{pmatrix}.
$$

Let

$$
U(t)=
\begin{pmatrix}
e^{i\omega t/(2\hbar)}&0\\
0&e^{-i\omega t/(2\hbar)}
\end{pmatrix},
\qquad
\binom{a_0}{a_1}=U(t)\binom{b_0}{b_1}.
$$

The rotating-frame amplitudes obey a constant Schrödinger equation

$$
i\hbar\frac d{dt}\binom{b_0}{b_1}
=H_{\mathrm{eff}}\binom{b_0}{b_1},
\qquad
H_{\mathrm{eff}}=
\begin{pmatrix}
\omega/2&c\\
c&-\omega/2
\end{pmatrix}.
$$

Put

$$
q=\sqrt{c^2+\frac{\omega^2}{4}},
\qquad
\theta=\frac{qt}{\hbar}.
$$

Since $H_{\mathrm{eff}}^2=q^2I$,

$$
e^{-itH_{\mathrm{eff}}/\hbar}
=\cos\theta\,I-i\frac{\sin\theta}{q}H_{\mathrm{eff}}.
$$

For the initial amplitudes $(A_0,A_1)$, the exact coefficients are therefore

$$
\boxed{
a_0(t)=e^{i\omega t/(2\hbar)}
\left[
\left(\cos\theta-i\frac{\omega}{2q}\sin\theta\right)A_0
-i\frac cq\sin\theta\,A_1
\right]}
$$

and

$$
\boxed{
a_1(t)=e^{-i\omega t/(2\hbar)}
\left[
-i\frac cq\sin\theta\,A_0
+\left(\cos\theta+i\frac{\omega}{2q}\sin\theta\right)A_1
\right]}.
$$

Restoring the common unperturbed phase, the solution is

$$
\boxed{
|\psi(t)\rangle
=e^{-iE_2t/\hbar}
\bigl(a_0(t)|2,0,0\rangle+a_1(t)|2,1,0\rangle\bigr)}.
$$

This is the [rotating-frame solution for a harmonically driven two-level system](../../../../../../../rotating-frame-solution-for-a-harmonically-driven-two-level-system.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [33C](../../../33c.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
