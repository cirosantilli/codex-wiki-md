# Radial Fourier representation of the Helmholtz Green function

↑ **Parent:** [Outgoing Green function for the three-dimensional Helmholtz equation](outgoing-green-function-for-the-three-dimensional-helmholtz-equation.md)

For $k_0>0$, $l=|r-r'|>0$ and the convention $(\Delta+k_0^2)G=-\delta$, the spatial [Fourier transform](fourier-transform-split.md) gives the multiplier $(k^2-k_0^2)^{-1}$. Aligning the Fourier polar axis with $r-r'$ gives $\int_{S^2}e^{ikl\cos\theta}d\Omega=4\pi\sin(kl)/(kl)$ and hence the displayed radial integral.

The pole on the integration path requires a prescription. The [Cauchy principal value](cauchy-principal-value.md) gives $G_{\rm PV}(l)=\cos(k_0l)/(4\pi l)$. The outgoing prescription is $k^2-k_0^2-i0$, yielding $G_+(l)=e^{ik_0l}/(4\pi l)$; the opposite prescription gives the incoming exponential. The [Sokhotski–Plemelj formula](sokhotski-plemelj-theorem.md) $1/(q-i0)=\operatorname{PV}(1/q)+i\pi\delta(q)$ shows that the additional radial contribution is $i\sin(k_0l)/(4\pi l)$.

For the inverse-kernel convention $(\Delta+k_0^2)H=+\delta$, use $H=-G$. Thus a source equation $(\Delta+k_0^2)\Phi=V$ has $\Phi=H*V=-G*V$, with the same boundary or radiation convention throughout. Without a pole prescription or an equivalent condition at infinity, the real-frequency source problem does not specify a unique Green function.

## ↑ Ancestors (7)

1. [Outgoing Green function for the three-dimensional Helmholtz equation](outgoing-green-function-for-the-three-dimensional-helmholtz-equation.md)
2. [Helmholtz equation](helmholtz-equation.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/3/solution.md)
