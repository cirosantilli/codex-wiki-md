<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the model's normalization in which $K$ has velocity-squared units: it is kinetic energy per fixed reference mass, or a correspondingly normalized total energy. Let

$$
a=U_0^2\left(\frac1{L_f}-\frac1{L_\rho}\right),
\qquad \dot K=\sqrt K\left(a-\frac K{L_v}\right).
$$

For $K>0$, setting $s=\sqrt K$ reduces the equation to $2\dot s=a-s^2/L_v$. Suppose first that $L_f<L_\rho$, so $a>0$. Put $s_\infty=\sqrt{aL_v}$, $y=s/s_\infty$, $y_0=\sqrt{K_0/(aL_v)}$ and $\gamma=s_\infty/(2L_v)$. Separating variables gives $\dot y=\gamma(1-y^2)$ and therefore the [forced stratified mixing with square-root power input](../../../../../../forced-stratified-mixing-with-square-root-power-input.md) solution

$$
\boxed{K(t)=K_\infty\left[
\frac{y_0+\tanh(\gamma t)}{1+y_0\tanh(\gamma t)}\right]^2,
\qquad K_\infty=aL_v
=\frac{L_v(L_\rho-L_f)}{L_fL_\rho}U_0^2.}
$$

This expression satisfies $K(0)=K_0$ and the differential equation directly.

For $0<K_0<K_\infty$, one may equivalently write $y=\tanh[\gamma t+\operatorname{artanh}y_0]$; the energy increases monotonically to $K_\infty$. For $K_0>K_\infty$, $y=\coth[\gamma t+\operatorname{arccoth}y_0]$, and the energy decreases monotonically to the same value. $K_0=K_\infty$ is stationary. For a very large initial energy, the initial evolution is approximately $s=s_0/[1+s_0t/(2L_v)]$, until forcing becomes comparable with dissipation. For a very small positive seed, $s$ initially grows approximately linearly, before leveling off. Thus both paragraphs labelled (c) in the PDF are answered by the solution and its two branches.

The positive-seed condition is material. If $K_0=0$, the original equation also admits $K\equiv0$, and its square-root right-hand side is not Lipschitz at zero. It admits delayed-start solutions $K=0$ for $t\le t_d$ followed by $K=K_\infty\tanh^2[\gamma(t-t_d)]$. Therefore convergence to the positive steady state is not guaranteed from exactly zero turbulence without a startup prescription. For completeness, if $a=0$ a positive seed decays as $K=K_0/[1+\sqrt{K_0}t/(2L_v)]^2$. If $a<0$, it reaches zero in finite time, $t_*=2\sqrt{L_v/|a|}\arctan\sqrt{K_0/(|a|L_v)}$, and the nonnegative continuation is at rest.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
