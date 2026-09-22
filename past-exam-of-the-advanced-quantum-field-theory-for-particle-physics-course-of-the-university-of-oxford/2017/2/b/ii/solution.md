<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Continue with $\eta=-g$ and dot products in that auxiliary [metric](../../../../../minkowski-metric.md). Odd [gamma traces](../../../../../gamma-matrix-trace.md) vanish. The two current [tensors](../../../../../tensor.md) are

$$
\begin{aligned}
H_{\mu\alpha}&=4[p_{2\mu}p_{1\alpha}+p_{2\alpha}p_{1\mu}-\eta_{\mu\alpha}(p_1\cdot p_2+M^2)],\\
L^{\mu\alpha}&=4[k_1^\mu k_2^\alpha+k_1^\alpha k_2^\mu-\eta^{\mu\alpha}(k_1\cdot k_2)].
\end{aligned}
$$

Contracting gives

$$
H_{\mu\alpha}L^{\mu\alpha}=32[(p_1\cdot k_1)(p_2\cdot k_2)+(p_1\cdot k_2)(p_2\cdot k_1)+M^2(k_1\cdot k_2)].
$$

Let $u=2M^2-s-t$. The [on-shell products](../../../../../mass-shell.md) are $p_1\cdot k_1=p_2\cdot k_2=(M^2-t)/2$, $p_1\cdot k_2=p_2\cdot k_1=(M^2-u)/2$, and $k_1\cdot k_2=s/2$. Substitution yields

$$
\boxed{\overline{|T|^2}=\frac{4g_s^4}{9s^2}[(M^2-t)^2+(M^2-u)^2+2M^2s]
=\frac{64\pi^2\alpha_s^2}{9s^2}[(M^2-t)^2+(s+t-M^2)^2+2M^2s].}
$$

The result is already averaged over incoming [colours](../../../../../color-charge.md) and [spins](../../../../../spin.md) and summed over outgoing ones. For $M\to0$, it becomes $4g_s^4(t^2+u^2)/(9s^2)$.

An additional check uses the [centre-of-mass](../../../../../center-of-momentum-frame.md) angle and [velocity](../../../../../velocity.md) $\beta_t=\sqrt{1-4M^2/s}$:

$$
\overline{|T|^2}=\frac{2g_s^4}{9}\left[1+\cos^2\theta+\frac{4M^2}{s}\sin^2\theta\right].
$$

It tends to $4g_s^4/9$ at [threshold](../../../../../particle-production-threshold.md) and is positive throughout the physical region. Keeping both printed minus signs would instead give $4g_s^4[(M^2-t)^2+(M^2-u)^2-2M^2s]/(9s^2)$, displaying the incorrect [mass](../../../../../mass.md) contribution explicitly.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
