<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Linearize about water at rest with uniform surface elevation $h_0$. Write $h=h_0+\eta$, $u=v$, $S_0=S(x,h_0)$ and $T_0=S_h(x,h_0)$. To first order the [shallow water equations](../../../../../../shallow-water-equations.md) become

$$
T_0\eta_t+(S_0v)_x=0,\qquad v_t+g\eta_x=0.
$$

Differentiate continuity in time and eliminate $v_t$:

$$
T_0\eta_{tt}-g(S_0\eta_x)_x=0.
$$

For a time-harmonic standing disturbance, use $\eta(x,t)=\operatorname{Re}[\eta(x)e^{-i\omega t}]$. Then

$$
(S_0\eta')'+\frac{\omega^2T_0}{g}\eta=0.
$$

Dividing by $S_0$ proves

$$
\boxed{\eta''+\frac{S_0'}{S_0}\eta'+k^2\eta=0,\qquad
k^2(x)=\frac{\omega^2}{c_0^2(x)},\quad c_0^2=\frac{gS_0}{T_0}.}
$$

This identifies the coefficient as the local long-wave wavenumber. It is constant under the fixed-shape geometry used in part (a), when $c_0$ is independent of $x$; that assumption is needed for the constant-coefficient mode calculation in part (c).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
