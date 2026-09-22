<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In a steady state the [heat equation](../../../../../../heat-equation.md) says $(kT_s')'=0$, so the positive-$x$ [heat flux](../../../../../../heat-flux-density.md) $q=-kT_s'$ is the same constant $Q$ in both materials. Assume perfect thermal contact: temperature is continuous at $x=\ell$, and [conservation of energy](../../../../../../conservation-of-energy.md) requires continuous [heat flux](../../../../../../heat-flux-density.md) there. Integrating from the right endpoint gives

$$
\boxed{T_s(x)=\begin{cases}
\displaystyle\frac{Q\ell}{k_2}+\frac Q{k_1}(\ell-x),&0\leq x\leq\ell,\\[6pt]
\displaystyle\frac Q{k_2}(2\ell-x),&\ell\leq x\leq2\ell.
\end{cases}}
$$

The two formulas agree at the interface. Their slopes differ, but $-k_1T_s'(\ell^-)=-k_2T_s'(\ell^+)=Q$. The total temperature drop is $Q\ell(1/k_1+1/k_2)$, the sum of the two layers' contributions in [steady heat conduction through layers](../../../../../../steady-heat-conduction-through-layers.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
