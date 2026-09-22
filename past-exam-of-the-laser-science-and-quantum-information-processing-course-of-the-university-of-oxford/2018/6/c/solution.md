<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a deterministic local hidden variable, write the four possible measurement results as $q,r,s,t\in\{\pm1\}$. Its Bell combination is

$$
b=q(s-t)-r(s+t).
$$

If $s=t$, the first bracket vanishes and the second is $\pm2$; if $s=-t$, the second vanishes and the first is $\pm2$. Thus $b=\pm2$ for every hidden variable. Averaging over any local hidden-variable distribution gives $|\mathcal B|\leq2$, and in particular the requested upper bound.

For the specified settings, the correlation formula in part b gives

$$
\langle QS\rangle=\frac1{\sqrt2},\quad
\langle RS\rangle=\langle RT\rangle=-\frac{\cos\varphi}{\sqrt2},\quad
\langle QT\rangle=-\frac1{\sqrt2}.
$$

Consequently

$$
\boxed{\mathcal B=\sqrt2(1+\cos\varphi).}
$$

This violates the local bound precisely when

$$
\boxed{\cos\varphi>\sqrt2-1,\qquad
|\varphi-2\pi m|<\arccos(\sqrt2-1)\simeq1.14372\ \text{rad},\quad m\in\mathbb Z.}
$$

The maximum is $2\sqrt2$ at $\varphi=0$ modulo $2\pi$. The state remains maximally entangled at other [phases](../../../../phase-waves.md), even when this fixed choice of real-plane analyser settings gives no violation. Local [phase](../../../../phase-waves.md) compensation or adapted measurement settings can recover the optimum.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
