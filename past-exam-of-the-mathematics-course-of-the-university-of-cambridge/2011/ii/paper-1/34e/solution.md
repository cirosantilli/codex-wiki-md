<h1 id="34e/solution">Solution</h1>

↑ **Parent:** [34E](../34e.md)

With outgoing-channel index first, the [scattering matrix](../../../../../s-matrix.md) convention is $\psi_b\sim I_b+\sum_{a=\pm}S_{ab}O_a$ as $|x|\to\infty$. An even potential commutes with [parity](../../../../../parity.md), so its incoming even and odd channels remain separate: $\boxed{S_{+-}=S_{-+}=0}$.

For the odd channel, on $0<x<a$ write $\psi_-(x)=C\sin(kx)$, while on $x>a$ its prescribed normalization is $e^{-ikx}-S_{--}e^{ikx}$. A [delta potential](../../../../../delta-potential.md) keeps the wavefunction continuous and imposes $\psi'(a+)-\psi'(a-)=U_0\psi(a)$, with $U_0=2mV_0/\hbar^2$. Thus the exterior logarithmic derivative is $k\cot(ka)+U_0$. Matching gives

$$
S_{--}=e^{-2ika}\frac{k\cot(ka)+U_0+ik}{k\cot(ka)+U_0-ik}.
$$

Multiplying numerator and denominator by $2\sin(ka)$ and using exponential forms yields

$$
\boxed{S_{--}(k)=e^{-2ika}\frac{(2k-iU_0)e^{ika}+iU_0e^{-ika}}{(2k+iU_0)e^{-ika}-iU_0e^{ika}}.}
$$

For real $k,U_0$, the numerator of the fraction is the complex conjugate of its denominator, and the prefactor has modulus one. Hence $\boxed{|S_{--}|^2=1}$, conservation of probability flux in this single elastic parity channel. In particular the minus sign built into $O_-$ makes the free odd-channel matrix element equal to one.

For an odd [bound state](../../../../../bound-state.md), continue to $k=i\kappa$, $\kappa>0$. A pole means the outgoing solution is exponentially decaying on both sides. Its denominator vanishes when

$$
\kappa[1+\coth(\kappa a)]+U_0=0,\qquad\boxed{2\kappa=-U_0(1-e^{-2\kappa a}).}
$$

The function $2\kappa/(1-e^{-2\kappa a})$ rises strictly from $1/a$ to infinity: differentiation reduces positivity to $e^{2\kappa a}>1+2\kappa a$. Thus there is exactly one positive solution if $-U_0>1/a$, and none otherwise. The numerator does not vanish at that solution, so the pole is genuine. Consequently

$$
\boxed{\text{exactly one odd bound state exists iff }U_0a<-1,\quad E=-\hbar^2\kappa^2/(2m).}
$$

At equality the zero-energy threshold solution is not square integrable.

For repulsive strong barriers put $u=U_0a\gg1$ and $z=ka=\pi+\delta$. The pole equation is $z\cot z+u-iz=0$. Since $\cot\delta=\delta^{-1}-\delta/3+O(\delta^3)$, multiplication by $\delta$ gives $\pi+(u+1-i\pi)\delta+O(\delta^2)=0$. Iterating in $u^{-1}$ yields

$$
\delta=-\frac\pi u+\frac{\pi-i\pi^2}{u^2}+O(u^{-3}),\qquad
\boxed{\alpha\sim-\frac\pi{U_0a},\qquad\gamma\sim\left(\frac\pi{U_0a}\right)^2.}
$$

This lower-half-plane [resonance pole](../../../../../resonance-pole.md) is an odd standing wave trapped between the barriers and slowly leaking by tunnelling. Its complex energy is $E_R-i\Gamma/2$, with $\Gamma\simeq2\hbar^2\pi\gamma/(ma^2)>0$. The factor $e^{-iEt/\hbar}$ then decays rather than grows; $\gamma>0$ encodes the positive escape rate.

## ↑ Ancestors (11)

1. [34E](../34e.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
