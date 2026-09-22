<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a slowly varying envelope $E=\psi e^{-ikx}$, the [paraxial approximation](../../../../../../paraxial-approximation.md) to the [Helmholtz equation](../../../../../../helmholtz-equation.md) is

$$
E_x=\frac{i}{2k}E_{zz}
+\frac{ik}{2}(n^2-1)E.
$$

Because $n=1+\mu W$ and $\mu^2\ll1$, passage through a sufficiently thin [phase screen](../../../../../../phase-screen.md) produces

$$
E(0,z)=e^{i\phi(z)},
\qquad
\phi(z)=\frac{k}{2}\int_{-\xi}^{0}(n^2-1)\,dx
\simeq k\mu\xi W(z).
$$

Its [modulus](../../../../../../modulus.md) is one at the screen exit. Beyond the screen, $n=1$, so the [parabolic wave equation](../../../../../../parabolic-wave-equation.md) is $E_x=iE_{zz}/(2k)$. A [Taylor expansion](../../../../../../taylor-expansion.md) in propagation distance gives

$$
E(x,z)=E(0,z)+\frac{ix}{2k}E_{zz}(0,z)+O(x^2).
$$

Since

$$
\frac{(e^{i\phi})_{zz}}{e^{i\phi}}
=i\phi''-(\phi')^2,
$$

we find

$$
E(x,z)=e^{i\phi(z)}
\left[1-\frac{x}{2k}\phi''(z)
-\frac{ix}{2k}(\phi'(z))^2\right]+O(x^2).
$$

It follows that

$$
\boxed{|E(x,z)|=1-\frac{x}{2k}\phi''(z)+O(x^2)},
$$

or, equivalently, $|E|^2=1-x\phi''/k+O(x^2)$. Thus random [phase curvature](../../../../../../phase-curvature.md) produces local focusing and defocusing: [free-space diffraction](../../../../../../free-space-diffraction.md) converts phase fluctuations into amplitude fluctuations immediately after the screen.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
