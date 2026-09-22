<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Each light-string round trip combines wall reflection $-1$ with junction reflection $-1/3$, multiplying the remaining pulse amplitude by $1/3$. The initial directly reflected heavy-string pulse has amplitude $A_i/3$. The subsequent outgoing heavy pulses have amplitudes

$$
A_n=-\frac89\left(\frac13\right)^{n-1}A_i,\qquad n=1,2,\ldots.
$$

They all have width $w$ in the same heavy medium. For nonoverlapping pulses their [energy](../../../../energy-split.md) fractions therefore sum to

$$
\boxed{\frac{E_{\rm out}}{E_i}
=\frac19+\frac{64}{81}\sum_{n=0}^\infty\left(\frac19\right)^n
=\frac19+\frac89=1.}
$$

The first transmission leaves energy fraction $8/9$ in the light segment; each return encounter leaves only $1/9$ of the previous stored energy there, so this residual tends to zero.

For [reflection from a finite string segment with a fixed far end](../../../../reflection-from-a-finite-string-segment-with-a-fixed-far-end.md), if pulses overlap, squared amplitudes cannot simply be added because of [interference](../../../../interference-wave-propagation.md). The same result follows frequency by frequency: with round-trip phase $q=e^{2ik_lL_l}$, $L_l=2\,\mathrm m$, the total amplitude coefficient is

$$
R(q)=\frac13-\frac{8q/9}{1-q/3}=\frac{1/3-q}{1-q/3}.
$$

For real frequencies $|q|=1$, so $|1/3-q|=|1-q/3|$ and $|R|=1$. Thus the ideal lossless fixed-ended segment returns all incident finite-pulse energy even when individual echoes overlap; their relative phases must be retained.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [10](../../10.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
