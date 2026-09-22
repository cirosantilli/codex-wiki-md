<h1 id="11/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take $x\in[-s/2,s/2]$ along the tilt, with local separation $h(x)=a+2\delta x/s$. Since $s\gg a$ and the tilt is small, each narrow strip is a local [parallel-plate capacitor](../../../../parallel-plate-capacitor.md) at the same voltage $V$. Its surface charge densities are approximately

$$
\boxed{\sigma_\pm(x)=\pm\frac{\epsilon_0V}{a+2\delta x/s}.}
$$

Parallel strip capacitances add, so for $|\delta|<a$,

$$
C(\delta)=\epsilon_0s\int_{-s/2}^{s/2}\frac{dx}{a+2\delta x/s}
=\frac{\epsilon_0s^2}{2\delta}\log\frac{a+\delta}{a-\delta}.
$$

Using $\log[(1+z)/(1-z)]=2(z+z^3/3+z^5/5+\cdots)$ gives

$$
\boxed{C(\delta)=\frac{\epsilon_0s^2}{a}\left[1+\frac{\delta^2}{3a^2}+O\left(\frac{\delta^4}{a^4}\right)\right].}
$$

The denser charge at the smaller gap explains why tilting increases the capacitance. The local-strip approximation neglects fringing and slope corrections of order $(\delta/s)^2$, smaller than the retained $(\delta/a)^2$ term.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [11](../../11.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
