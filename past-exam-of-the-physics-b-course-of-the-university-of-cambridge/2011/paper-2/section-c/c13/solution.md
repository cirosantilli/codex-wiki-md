<h1 id="section-c/c13/solution">Solution</h1>

↑ **Parent:** [C13](../c13.md)

A [normal mode](../../../../../normal-mode.md) is a small-oscillation motion with every coordinate proportional to one common sinusoid, at a fixed amplitude ratio and relative phase. Expanding an arbitrary small motion in [normal mode coordinates](../../../../../normal-coordinate.md) decouples its linear equations into independent oscillators. With [mechanical mass matrix](../../../../../mechanical-mass-matrix.md) $\mathsf M$ and [mechanical stiffness matrix](../../../../../mechanical-stiffness-matrix.md) $\mathsf K$, the generalized [eigenvalue](../../../../../eigenvalue.md) equation is $\mathsf K\mathbf u=\omega^2\mathsf M\mathbf u$.

Horizontal gravitational restoring force on each bob is $-m_i(g/l)x_i$. The two springs add $k(x_2-x_1)$ on the first bob, $k(x_1-2x_2+x_3)$ on the middle bob, and $k(x_2-x_3)$ on the last. Dividing by the bob masses gives the stated equations with

$$
\boxed{\alpha=g/l,\qquad\beta=k.}
$$

[Reflection symmetry](../../../../../reflection-symmetry.md) separates an antisymmetric end motion from two symmetric motions. The [three coupled pendulums with equal end masses](../../../../../three-coupled-pendulums-with-equal-end-masses.md) have independent modes

$$
\begin{array}{c|c|l}
\text{amplitude vector}&\omega^2&\text{motion}\\\hline
(1,1,1)&g/l&\text{all bobs together; springs unstretched}\\
(1,0,-1)&g/l+k/m&\text{end bobs opposite; middle at rest}\\
(1,-2m/M,1)&g/l+k/m+2k/M&\text{ends together; middle opposite}.
\end{array}
$$

Call their positive frequencies $\omega_0,\omega_a,\omega_s$ respectively. The middle amplitude in the last mode ensures $m x_1+M x_2+m x_3=0$. The modes are orthogonal in the mass-weighted [inner product](../../../../../inner-product-split.md), rather than generally in the unweighted coordinate dot product.

The initially stationary displacement decomposes as

$$
(0,0,d)=\frac{md}{M+2m}(1,1,1)-\frac d2(1,0,-1)+\frac{Md}{2(M+2m)}(1,-2m/M,1).
$$

There are no [sine](../../../../../sine.md) terms because every initial velocity is zero. Therefore

$$
\boxed{\begin{aligned}
x_1(t)&=\frac{md}{M+2m}\cos\omega_0t-\frac d2\cos\omega_at+\frac{Md}{2(M+2m)}\cos\omega_st,\\
x_2(t)&=\frac{md}{M+2m}(\cos\omega_0t-\cos\omega_st),\\
x_3(t)&=\frac{md}{M+2m}\cos\omega_0t+\frac d2\cos\omega_at+\frac{Md}{2(M+2m)}\cos\omega_st.
\end{aligned}}
$$

These give $(0,0,d)$ at $t=0$ and solve all three coupled equations. The [spring constant](../../../../../spring-constant.md) is assumed positive; for $k=0$ the frequencies become degenerate and the same [superposition](../../../../../superposition-principle.md) reduces to uncoupled pendulum motion.

<a id="section-c/c13/image-three-pendulum-modes"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-2-pendulum-modes.png)

**[Figure 3](#section-c/c13/image-three-pendulum-modes). Three pendulum modes**.

The original example uses $M=2m$ and $k/m=g/l$ to display the mode [vectors](../../../../../vector.md) and resulting [superposition](../../../../../superposition-principle.md). Those illustrative parameter ratios are not additional supplied data.

## ↑ Ancestors (14)

1. [C13](../c13.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
