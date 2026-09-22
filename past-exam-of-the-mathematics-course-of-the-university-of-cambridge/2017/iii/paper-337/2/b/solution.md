<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a real steady amplitude, integrate the conserved-field equation twice. Periodicity forces the integration slope to vanish, and the zero mean fixes the remaining constant. Hence

$$
\boxed{B=\kappa(\langle A^2\rangle-A^2),\qquad\kappa=\mu/\sigma.}
$$

Substituting this into the steady [amplitude equation](../../../../../../amplitude-equation.md) gives the nonlocal [ordinary differential equation](../../../../../../ordinary-differential-equation.md)

$$
A''+(1-\kappa\langle A^2\rangle)A+(\kappa-1)A^3=0.
$$

For $A=R\operatorname{sech}(cX)$, use the [hyperbolic secant](../../../../../../hyperbolic-secant.md) identity $A''=c^2A-2c^2A^3/R^2$. Vanishing of the two independent coefficients gives

$$
\boxed{\kappa\langle A^2\rangle=1+c^2,\qquad \kappa=1+\frac{2c^2}{R^2}.}
$$

Choose $c>0$ and $R>0$; an overall negative sign is another solution. Thus $\kappa>1$. The exact average of the proposed profile over the finite interval is

$$
\langle A^2\rangle=\frac{2R^2}{cL}\tanh\frac{cL}{2}.
$$

For $cL\gg1$, the [hyperbolic tangent](../../../../../../hyperbolic-tangent.md) differs from one by $O(e^{-cL})$, so $cL\langle A^2\rangle\simeq2R^2$. Eliminating $R^2=2c^2/(\kappa-1)$ gives the requested leading relation

$$
\boxed{L(c^2+1)=\frac{4c\kappa}{\kappa-1}.}
$$

Equivalently $c+c^{-1}=K$, with $K=4\kappa/[L(\kappa-1)]$. Positive real roots exist precisely when $K\geq2$; they are $(K\pm\sqrt{K^2-4})/2$ and are reciprocal. Each candidate must additionally satisfy $cL\gg1$. For $L>2$, the leading necessary range is $1<\kappa\leq L/(L-2)$, with equality at the coalescence $c=1$. Away from this leading-order fold, the inequality is strict.

The strict finite-window condition can also be seen by retaining the average exactly. Its consistency relation is $c+c^{-1}=K\tanh(cL/2)$. Since $\tanh(cL/2)<1$, it implies $K>2$, and hence

$$
\boxed{1<\kappa<\frac L{L-2}\quad\text{provided }L>2.}
$$

The strict endpoint distinction is exponentially small in the large-$cL$ approximation; the leading polynomial alone permits its double root. When $0<L\leq2$, this algebra imposes no finite upper bound on $\kappa>1$. The printed interval therefore needs $L>2$: for example $L=1$, $\kappa=1.1$ gives a large positive root $c\simeq43.98$ of the leading equation and $cL\gg1$, despite the printed upper endpoint being negative.

Finally, the single [localized pulse of a conserved-field convection model](../../../../../../localized-pulse-of-a-conserved-field-convection-model.md) is an approximate periodic solution. Its values agree at the interval ends, but its derivatives have opposite signs there; their magnitude is exponentially small, $O(cR e^{-cL/2})$. Periodic-tail corrections are needed for an exact smooth [periodic boundary condition](../../../../../../periodic-boundary-conditions.md). The range derived from the truncated profile is a consistency condition, not a proof that every permitted parameter gives an exact stable periodic pulse.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
