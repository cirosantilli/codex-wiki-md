<h1 id="section-b/b6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let the middle segment occupy $0<x<l$. Normalize the incident displacement [complex amplitude](../../../../../../complex-amplitude.md) to one, suppress the common time factor $e^{-i\omega t}$, and choose

$$
\begin{aligned}
y_L(x)&=e^{ik_Lx}+r e^{-ik_Lx},&&x<0,\\
y_M(x)&=a e^{ik_Mx}+b e^{-ik_Mx},&&0<x<l,\\
y_R(x)&=t e^{ik_R(x-l)},&&x>l.
\end{aligned}
$$

Here $r$ is the reflected [complex amplitude](../../../../../../complex-amplitude.md) at $0$, $a$ and $b$ are the rightgoing and leftgoing middle-segment [complex amplitudes](../../../../../../complex-amplitude.md) referenced to $0$, and $t$ is the outgoing [complex amplitude](../../../../../../complex-amplitude.md) referenced to $l$. The middle [wavenumber](../../../../../../wavenumber.md) is $k_M=\omega/c_M$, and

$$
\gamma=e^{ik_Ml},\qquad |\gamma|=1
$$

is the propagation [phase factor](../../../../../../phase-factor.md) across the lossless middle segment.

At each junction, continuity of displacement and transverse [force](../../../../../../force-split.md) means continuity of $y$ and $Ty_x$. Using $Tk_j=\omega Z_j$ gives

$$
\boxed{\begin{aligned}
1+r&=a+b,\\
Z_L(1-r)&=Z_M(a-b),\\
\gamma a+\gamma^{-1}b&=t,\\
Z_M(\gamma a-\gamma^{-1}b)&=Z_Rt.
\end{aligned}}
$$

These [boundary conditions](../../../../../../boundary-condition.md) also include all multiple reflections inside the middle segment: $a$ and $b$ are the total travelling components, not just the first waves to cross a junction.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
