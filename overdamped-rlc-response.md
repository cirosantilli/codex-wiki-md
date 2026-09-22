# Overdamped RLC response

↑ **Parent:** [Series RLC circuit](series-rlc-circuit.md)

An [overdamped RLC response](overdamped-rlc-response.md) is a free [series RLC circuit](series-rlc-circuit.md) response with $R>2\sqrt{L/C}$, equivalently $\alpha>\omega_0$. Put $\beta=\sqrt{\alpha^2-\omega_0^2}$. The distinct negative [characteristic roots](characteristic-root-of-a-constant-coefficient-differential-equation.md) are $r_\pm=-\alpha\pm\beta$, so the general [electric charge](electric-charge-split.md) is

$$
q(t)=Ae^{r_+t}+Be^{r_-t},\qquad i(t)=q'(t).
$$

For [initial conditions](initial-condition.md) $q(0)=q_0$, $i(0)=0$,

$$
q(t)=q_0e^{-\alpha t}\left(\cosh(\beta t)+\frac\alpha\beta\sinh(\beta t)\right),\qquad
i(t)=-\frac{q_0\omega_0^2}{\beta}e^{-\alpha t}\sinh(\beta t).
$$

For $q_0>0$, this [electric charge](electric-charge-split.md) decreases to zero without reversing sign. In the dimensionless example $\omega_0=1$, $\alpha=2$, the [characteristic roots](characteristic-root-of-a-constant-coefficient-differential-equation.md) are $-2\pm\sqrt3\approx-0.268,-3.732$. The slow term dominates late times. Stronger [damping](damping.md) can therefore make the final return slower: for $\alpha\gg\omega_0$, $r_+\sim-\omega_0^2/(2\alpha)=-1/(RC)$. Nonoscillation alone does not imply a fast response, and monotonicity here uses the specified [initial conditions](initial-condition.md).

## ↑ Ancestors (7)

1. [Series RLC circuit](series-rlc-circuit.md)
2. [RLC circuit](rlc-circuit.md)
3. [Electrical circuit](electrical-circuit-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Critically damped RLC response](critically-damped-rlc-response.md)
- [Overdamped RLC response](overdamped-rlc-response.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/5c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/5c/c/ii/solution.md)
- [Resonant series RLC response](resonant-series-rlc-response.md)
- [Series RLC circuit](series-rlc-circuit.md)
- [Underdamped RLC response](underdamped-rlc-response.md)
