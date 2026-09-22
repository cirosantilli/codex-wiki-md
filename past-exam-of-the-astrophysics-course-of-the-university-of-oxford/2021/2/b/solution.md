<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $r=A(1-\cos\theta)$ and $t+T=B(\theta-\sin\theta)$, differentiation gives

$$
\dot r=\frac AB\frac{\sin\theta}{1-\cos\theta},\qquad
\ddot r=-\frac A{B^2(1-\cos\theta)^2}.
$$

Comparison with $-GM/[A^2(1-\cos\theta)^2]$ proves $A^3=GMB^2$. Substitution into the conserved [specific orbital energy](../../../../specific-orbital-energy.md) gives $\epsilon=-GM/(2A)$. Therefore

$$
\boxed{A=\frac{r_i(1+\delta_i)}{2\delta_i},\qquad
B=\frac{1+\delta_i}{2H_i\delta_i^{3/2}}.}
$$

These constants exactly reproduce both the initial radius and expanding [velocity](../../../../velocity.md). The initial parameter obeys

$$
\cos\theta_i=\frac{1-\delta_i}{1+\delta_i},\qquad
\theta_i=2\arctan\sqrt{\delta_i}.
$$

In an [Einstein-de Sitter universe](../../../../einstein-de-sitter-universe.md) whose background big bang is $t=0$, $t_i=2/(3H_i)$. Thus the exact required offset is

$$
\boxed{T=B(\theta_i-\sin\theta_i)-t_i.}
$$

Expanding $\theta_i-\sin\theta_i=\frac43\delta_i^{3/2}-\frac85\delta_i^{5/2}+O(\delta_i^{7/2})$ gives

$$
T=-\frac15t_i\delta_i+O(t_i\delta_i^2).
$$

**One cannot set $T=0$ exactly at finite $\delta_i$ while retaining the stated initial Hubble velocity and background time origin.** For example $\delta_i=0.01$, $t_i=1$ gives $T=-0.00199148$. Shifting to $t'=t+T$ removes the offset from the local orbit, but the background then scales as $a\propto(t'-T)^{2/3}$, not $t'^{2/3}$. Setting $T\simeq0$ is justified in the early-initial-time limit for subsequent evolution; the following standard growing-mode formulae use that approximation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
