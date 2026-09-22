<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use constant component [masses](../../../../mass.md) and a circular [Keplerian orbit](../../../../kepler-orbit.md). Then $J=\mu\sqrt{GMA}$ gives $\dot J/J=\dot A/(2A)$, while $P=2\pi A^{3/2}/\sqrt{GM}$ gives $\dot P/P=3\dot A/(2A)=3\dot J/J$. Dividing the supplied loss law by $J$ therefore yields

$$
\boxed{\frac{\dot P}{P}=-\frac{96}{5}\frac{G^3\mu M^2}{c^5A^4}},\qquad
\dot A=-\frac{64}{5}\frac{G^3\mu M^2}{c^5A^3}.
$$

The positive instantaneous [orbital decay timescale](../../../../orbital-decay-timescale.md) is $\tau_P=P/|\dot P|$, since $\dot P<0$. For $t_G=10^{10}$ yr, the requested prescription gives

$$
A_{\max}=\left(\frac{96G^3\mu M^2t_G}{5c^5}\right)^{1/4},\qquad
P_{\max}=\frac{2\pi A_{\max}^{3/2}}{\sqrt{GM}}.
$$

It is important to distinguish this prescription from the integrated [gravitational-wave inspiral time](../../../../gravitational-wave-inspiral-time.md). Integrating $\dot A=-C/A^3$ gives

$$
\boxed{t_{\rm merge}=\frac{5c^5A^4}{256G^3\mu M^2}=\frac38\tau_P}.
$$

Finite contact radii supply a small lower-limit correction when the initial separation is much larger than the compact objects. Thus the periods below satisfy the printed instantaneous-timescale criterion and have a formal merger time $3.75$ Gyr. If instead the requirement is literally $t_{\rm merge}=10$ Gyr, every period limit is larger by $(8/3)^{3/8}=1.445$. Eccentric systems require a different decay calculation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
