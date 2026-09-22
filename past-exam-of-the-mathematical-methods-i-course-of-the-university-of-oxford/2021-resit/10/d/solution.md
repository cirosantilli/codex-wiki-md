<h1 id="10/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [homogeneous linear differential equation](../../../../homogeneous-linear-differential-equation.md) has roots $(-1\pm i\sqrt3)/2$, so its [complementary function](../../../../homogeneous-solution.md) decays:

$$
f_h=e^{-t/2}\left(C_1\cos\frac{\sqrt3t}{2}+C_2\sin\frac{\sqrt3t}{2}\right).
$$

For a [particular integral](../../../../particular-solution.md), set $f_p=B\cos2t+C\sin2t$. Substitution gives

$$
f_p''+f_p'+f_p=(-3B+2C)\cos2t+(-2B-3C)\sin2t.
$$

The two coefficient equations are $-3B+2C=A$ and $-2B-3C=0$, so $B=-3A/13$ and $C=2A/13$. Consequently every solution obeys

$$
\boxed{f(t)=\frac A{13}(-3\cos2t+2\sin2t)+O(e^{-t/2}),\qquad t\to\infty.}
$$

The limiting behaviour is a periodic steady oscillation with amplitude $|A|/\sqrt{13}$, the long-time response of a [forced harmonic oscillator](../../../../forced-harmonic-oscillator.md). Unless $A=0$, there is no finite numerical limit: at $t=n\pi$ and $t=n\pi+\pi/2$, the two limiting values are $-3A/13$ and $3A/13$. For $A=0$, $f(t)\to0$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [10](../../10.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
