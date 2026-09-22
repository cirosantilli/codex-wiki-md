<h1 id="3/2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For the stated [mollifier](../../../../../../../mollifier.md), $(\partial_t+\partial_s)\chi_\varepsilon=(\partial_x+\partial_y)\chi_\varepsilon=0$. Thus the interior doubled integral is

$$
\int\chi_\varepsilon(t-s,x-y)\bigl[H(u(t,x),v(s,y))\varphi_t(t,x)+Q(u(t,x),v(s,y))\varphi_x(t,x)\bigr].
$$

On a bounded state range, $H$ is Lipschitz in each argument, and so is $Q$: away from the diagonal each partial [derivative](../../../../../../../derivative.md) has modulus at most $\sup|f'|$, and the function is continuous across the diagonal. Local $L^1$ translation continuity therefore makes this converge to the corresponding single-time, single-space integral. The compact time support is chosen below $T$, with a margin for $s\le t+2\varepsilon$.

The initial terms need a separate argument. Since the time kernel is supported at $t-s\in[-2\varepsilon,-\varepsilon]$, $B_v$ is identically zero for $t\ge0$, whereas $B_u$ samples $v(s,\cdot)$ at $\varepsilon\le s\le2\varepsilon$.

The [averaged initial trace of an entropy solution](../../../../../../../averaged-initial-trace-of-an-entropy-solution.md) follows directly from its inequalities. Test the constant-level entropy for $v$ with $(1-s/\delta)_+\rho(y)$, using smooth approximations of that temporal cutoff. Boundedness of $v$ and its entropy flux gives

$$
\frac1\delta\int_0^\delta\!\int\rho|v(s)-k|\le\int\rho|v_0-k|+O(\delta).
$$

Approximate $v_0$ locally in $L^1$ by finitely many constants with a smooth nonnegative partition of unity. Applying this estimate on each partition member and using the triangle inequality makes the limsup of $\delta^{-1}\int_0^\delta\|v(s)-v_0\|_{L^1(K)}ds$ arbitrarily small. This proves its convergence to zero for each compact $K$.

The time kernel has size $O(\varepsilon^{-1})$ and the spatial kernel is a normalized [approximate identity](../../../../../../../approximate-identity.md). The averaged trace, followed by spatial $L^1$ translation continuity of $v_0$, therefore gives $B_u\to\int|u_0-v_0|\varphi(0)$. Its time mass is one, not one-half, because its whole support lies on the positive $s$ side. Consequently

$$
\boxed{\int_0^T\!\int\bigl[|u-v|\varphi_t+Q(u,v)\varphi_x\bigr]+\int|u_0-v_0|\varphi(0)\ge0.}
$$

This is the [Kato inequality for scalar conservation laws](../../../../../../../kato-inequality-for-scalar-conservation-laws.md) with its initial contribution. Assuming an initial trace solely from interior translation continuity would leave a gap; the entropy argument above supplies it.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [3](../../../3.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
