<h1 id="39c/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The Fourier modes evolve according to the dispersion relation found in part (a), so

$$
\phi(Vt,t)=\int_{-\infty}^{\infty}
A(k)e^{it\psi(k)}\,dk,
\qquad
\psi(k)=(V-U)k-\frac{k^9}{9}.
$$

For $V>U$, the stationary-point equation is

$$
\psi'(k)=V-U-k^8=0.
$$

It has the two real solutions

$$
k=\pm k_0,
\qquad
k_0=(V-U)^{1/8}.
$$

Define

$$
\Omega=\psi(k_0)=\frac89k_0^9,
\qquad
|\psi''(\pm k_0)|=8k_0^7.
$$

The [one-dimensional stationary-phase formula](../../../../../../../one-dimensional-stationary-phase-formula.md) gives one contribution from each stationary point:

$$
\boxed{
\phi(Vt,t)\sim
\sqrt{\frac{\pi}{4tk_0^7}}
\left[
A(k_0)e^{i(\Omega t-\pi/4)}
+A(-k_0)e^{-i(\Omega t-\pi/4)}
\right].}
$$

Because the initial field is [real](../../../../../../../real-valued-function.md), its [Fourier transform](../../../../../../../fourier-transform.md) has the conjugate symmetry $A(-k)=A(k)^*$. Hence the same result can be written

$$
\boxed{
\phi(Vt,t)\sim
\sqrt{\frac{\pi}{tk_0^7}}\,
\operatorname{Re}\!\left[
A(k_0)e^{i(\Omega t-\pi/4)}
\right].}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [39C](../../../39c.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
