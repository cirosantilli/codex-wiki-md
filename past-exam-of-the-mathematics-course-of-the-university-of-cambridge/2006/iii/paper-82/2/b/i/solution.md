<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take a cut-on mode with $k>0$, put $\lambda=n\pi/h$ and $\alpha=\tan^{-1}(\lambda/k)$, so $k=k_0\cos\alpha$, $\lambda=k_0\sin\alpha$, and initially take $n>0$. The [acoustic waveguide](../../../../../../../acoustic-waveguide.md) mode splits into two [acoustic plane waves](../../../../../../../acoustic-plane-wave.md):

$$
\cos(\lambda y)e^{-ikx}=\frac12e^{-ikx-i\lambda y}+\frac12e^{-ikx+i\lambda y}.
$$

At the upper edge $y=h$, the upward-going constituent is incident from below. Use the reflected local coordinate $Y_+=h-y$; its incident potential becomes $(-1)^n e^{-ikx+i\lambda Y_+}/2$, with local incidence angle $\theta_0=\pi-\alpha$. At the lower edge use $Y_-=y+h$ and the downward-going constituent; it has the same local incident amplitude and incidence angle. At each wall the other constituent is the [geometrical optics](../../../../../../../geometrical-optics.md) reflection of this incident half-amplitude, so it must not be counted again as an independent incident wave at the same edge.

Let $D(r)=\sqrt{2/(\pi k_0r)}e^{-ik_0r-i\pi/4}$. For a far observer, the upper and lower local observation angles are $-\theta$ and $\theta$, and their distances are $r_+=r-h\sin\theta+O(h^2/r)$ and $r_-=r+h\sin\theta+O(h^2/r)$. Applying the [Wiener-Hopf solution of rigid half-plane diffraction](../../../../../../../wiener-hopf-solution-of-rigid-half-plane-diffraction.md) separately gives

$$
\begin{aligned}
\phi_{d,+}&\sim-\frac{(-1)^n}{2}D(r)\frac{\cos(\alpha/2)\sin(\theta/2)}{\cos\theta-\cos\alpha}e^{+ik_0h\sin\theta},\\
\phi_{d,-}&\sim+\frac{(-1)^n}{2}D(r)\frac{\cos(\alpha/2)\sin(\theta/2)}{\cos\theta-\cos\alpha}e^{-ik_0h\sin\theta}.
\end{aligned}
$$

The sign difference is the reversal of the upper-edge transverse coordinate. Their sum is the leading [independent-edge radiation from an open planar duct](../../../../../../../independent-edge-radiation-from-an-open-planar-duct.md):

$$
\boxed{\phi_d\sim-i(-1)^nD(r)\cos(\alpha/2)\sin(\theta/2)\frac{\sin(k_0h\sin\theta)}{\cos\theta-\cos\alpha}.}
$$

Restore $e^{i\omega t}$ if a time-dependent potential is desired. This is the leading large-$k_0h$ approximation, neglecting further diffraction between edges, and assumes a far-field distance $r\gg k_0h^2$ as well as $r\gg h$. It is not a uniform approximation for a mode approaching cutoff. The zero mode follows as the grazing-incidence limit $\alpha=0$; its beam-direction limit is treated separately below.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 82](../../../../paper-82-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
