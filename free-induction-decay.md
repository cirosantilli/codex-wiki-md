# Free induction decay

↑ **Parent:** [Nuclear magnetic resonance](nuclear-magnetic-resonance-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Free_induction_decay)

[Free induction decay](free-induction-decay.md) is a receiving [signal](signal.md) from freely precessing transverse [magnetization](magnetization.md) after excitation ends. [Faraday's law of induction](faraday-s-law-of-induction.md) gives coil voltage proportional to the time derivative of linked [magnetic flux](magnetic-flux.md), with sign set by the winding. At $\omega_0T_2\gg1$ its envelope follows the transverse [magnetization](magnetization.md); a fixed receiver phase can absorb the derivative's near-quadrature shift. We define the calibrated complex [signal](signal.md) below to represent [magnetization](magnetization.md), not raw coil voltage.

For an original teaching model, take positive $\gamma$, a circular drive $B_1(\cos\omega t\,\hat{\mathbf x}-\sin\omega t\,\hat{\mathbf y})$, and axes rotating at $-\omega$ about $z$. Define $u+iv=e^{i\omega t}(M_x+iM_y)$, $w=M_z$, $\Delta=\omega_0-\omega$ and $\omega_1=\gamma B_1$. The [Bloch equations](bloch-equations.md) become

$$
\dot u=-u/T_2+\Delta v,\qquad
\dot v=-\Delta u-v/T_2+\omega_1w,\qquad
\dot w=-\omega_1v-(w-M_0)/T_1.
$$

A linearly oscillating field of peak amplitude $2B_1$ has a co-rotating component of amplitude $B_1$; neglecting its counter-rotating component requires $\omega_1\ll\omega_0$ near resonance.

At resonance, a short pulse starting from $(0,0,M_0)$ gives $(u,v,w)=(0,M_0\sin\theta,M_0\cos\theta)$ with $\theta=\gamma B_1\tau$, neglecting relaxation during duration $\tau$. A receiver phase rotation can make a $\pi/2$ pulse's initial transverse [signal](signal.md) real. After the pulse, direct integration gives

$$
S(t)=S_0e^{-t/T_2}e^{-i\Delta t},\qquad
I(t)=\operatorname{Re}S(t),\qquad Q(t)=\operatorname{Im}S(t).
$$

These are the two components extracted by [quadrature demodulation](quadrature-demodulation.md). Differentiating verifies $\dot S=-(T_2^{-1}+i\Delta)S$; taking its magnitude separates decay from detuning.

Choose rounded illustrative $\gamma/(2\pi)=42.58\,\mathrm{MHz/T}$, $B_0=0.200\,\mathrm T$, $B_1=10\,\mathrm{\mu T}$, $T_1=0.800\,\mathrm s$ and $T_2=0.120\,\mathrm s$. Then $f_0=8.516\,\mathrm{MHz}$ and the $\pi/2$ duration is $\tau=1/(4(\gamma/(2\pi))B_1)=0.587\,\mathrm{ms}$, short relative to both relaxation times. For receiver detuning $\Delta/(2\pi)=5\,\mathrm{Hz}$ and $S_0=1$, $S(0.050\,\mathrm s)=-0.65924i$ and $S(0.100\,\mathrm s)=-0.43460$. These are calculated examples, not 1946 measurements.

<a id="image-a-pulse-rotating-frame-quadratures-and-the-corresponding-resonance-width"></a>
![](nuclear-magnetic-resonance-rotating-frame-decay-and-linewidth.png)

**[Figure 2](#image-a-pulse-rotating-frame-quadratures-and-the-corresponding-resonance-width). A pulse, rotating-frame quadratures and the corresponding resonance width**. Original calculated [Bloch equations](bloch-equations.md) example with the parameters above. The resonant pulse rotates [magnetization](magnetization.md) towards $+v$; a receiver phase makes $S(0)=1$. The later free [signal](signal.md) has 5 Hz detuning. The final panel shows the normalized weak-drive homogeneous absorption profile, centered on resonance. None of these curves is a historical trace.

## ↑ Ancestors (3)

1. [Nuclear magnetic resonance](nuclear-magnetic-resonance-split.md)
2. [Chemistry](chemistry-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Free induction decay](free-induction-decay.md)
- [Hahn spin echo experiment](hahn-spin-echo-experiment.md)
- [Spin echo](spin-echo.md)
- [Static inhomogeneity refocusing](static-inhomogeneity-refocusing.md)
