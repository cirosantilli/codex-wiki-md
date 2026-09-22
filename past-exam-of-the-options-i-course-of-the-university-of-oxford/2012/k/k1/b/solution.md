<h1 id="k/k1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

This is a [Rankine vortex](../../../../../rankine-vortex.md). Write $r=\sqrt{x^2+y^2}$. Inside the core the [velocity](../../../../../velocity.md) is $u=(\Gamma y/a^2,-\Gamma x/a^2,0)$, so

$$
\boxed{\omega=\nabla\times u=-\frac{2\Gamma}{a^2}k\quad(r<a).}
$$

This is the core value obtained from the inner formula; outside, the given irrotationality makes the [vorticity](../../../../../vorticity-split.md) zero. For nonzero $\Gamma$, the sharp boundary $r=a$ has different one-sided velocity gradients, so a single classical [vorticity](../../../../../vorticity-split.md) is not defined exactly on that edge; the inner trace is the boxed value and the outer trace is zero.

Inside the core, direct differentiation gives $(u\cdot\nabla)u=-\Gamma^2(x,y,0)/a^4$. The steady [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid-split.md) therefore give $p_r=\rho\Gamma^2r/a^4$ and $p_z=-\rho g$. Integrating,

$$
p_{\rm in}=A+\frac{\rho\Gamma^2r^2}{2a^4}-\rho gz.
$$

Outside, $|u|^2=\Gamma^2/r^2$, so part (a) gives

$$
p_{\rm out}=B-\frac{\rho\Gamma^2}{2r^2}-\rho gz.
$$

Matching [pressure](../../../../../pressure-split.md) at the core edge $r=a$ yields $A=B-\rho\Gamma^2/a^2$. Hence the complete [pressure](../../../../../pressure-split.md) field, up to one additive constant $B$, is

$$
\boxed{p(r,z)=\begin{cases}
B-\rho gz-\dfrac{\rho\Gamma^2(2a^2-r^2)}{2a^4},&r\leq a,\\
B-\rho gz-\dfrac{\rho\Gamma^2}{2r^2},&r>a.
\end{cases}}
$$

Both the [velocity](../../../../../velocity.md) and [pressure](../../../../../pressure-split.md) are continuous at $r=a$. The inside expression has been derived from the momentum equation because the core is rotational.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [K1](../../k1.md)
3. [K](../../../k.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
