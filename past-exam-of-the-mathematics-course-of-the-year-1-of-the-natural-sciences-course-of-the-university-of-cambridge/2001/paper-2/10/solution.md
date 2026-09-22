<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

If $P\,dx+Q\,dy=dF$ for a twice continuously differentiable potential $F$, then $P=F_x$ and $Q=F_y$. Equality of [mixed partial derivatives](../../../../mixed-partial-derivative.md) gives the necessary condition for an [exact differential](../../../../exact-differential.md):

$$
\boxed{P_y=Q_x.}
$$

This condition alone does not ensure global exactness on a domain with holes.

For the [Helmholtz free energy](../../../../helmholtz-free-energy.md) $A=U-TS$, use the stated identity for [internal energy](../../../../internal-energy-split.md) and the [product rule](../../../../product-rule.md):

$$
dA=dU-T\,dS-S\,dT=-S\,dT-p\,dV.
$$

Thus $A_T|_V=-S$ and $A_V|_T=-p$. Equality of [mixed partial derivatives](../../../../mixed-partial-derivative.md) yields the [Maxwell relation](../../../../maxwell-relations.md)

$$
\boxed{\left(\frac{\partial S}{\partial V}\right)_T=\left(\frac{\partial p}{\partial T}\right)_V.}
$$

The [temperature](../../../../temperature-split.md) and [volume](../../../../volume-thermodynamics.md) are the independent variables here, with composition and amount of gas fixed.

Next express $S=S(T,V)$ and substitute its [total differential](../../../../total-differential.md) into $dU=T\,dS-p\,dV$:

$$
dU=T\left(\frac{\partial S}{\partial T}\right)_VdT+\left[T\left(\frac{\partial S}{\partial V}\right)_T-p\right]dV.
$$

Matching the coefficient of $dV$ gives

$$
\boxed{\left(\frac{\partial U}{\partial V}\right)_T=T\left(\frac{\partial S}{\partial V}\right)_T-p=T\left(\frac{\partial p}{\partial T}\right)_V-p.}
$$

This is the [thermodynamic internal pressure](../../../../thermodynamic-internal-pressure.md) identity: an [equation of state](../../../../equation-of-state.md) determines how [internal energy](../../../../internal-energy-split.md) changes under an isothermal change of [volume](../../../../volume-thermodynamics.md).

For the [Dieterici equation](../../../../dieterici-equation.md), set $c=an/(VR)$ while differentiating at fixed $V$. Then

$$
p=\frac{nR}{V-nb}Te^{-c/T},\qquad\left(\frac{\partial p}{\partial T}\right)_V=\frac{nR}{V-nb}e^{-c/T}\left(1+\frac cT\right).
$$

Substitute into the [thermodynamic internal pressure](../../../../thermodynamic-internal-pressure.md) identity. The term proportional to $T$ cancels $p$, leaving

$$
\boxed{\left(\frac{\partial U}{\partial V}\right)_T=\frac{an^2}{V(V-nb)}\exp\left(-\frac{an}{VRT}\right).}
$$

The physical gas domain has $T>0$ and $V>nb$.

For the [ideal gas](../../../../ideal-gas-split.md) instead, $p=nRT/V$ gives $T(\partial p/\partial T)_V-p=0$. Therefore $U$ is independent of [volume](../../../../volume-thermodynamics.md) at fixed amount of gas. Integrating the remaining condition $(\partial U/\partial T)_V=C_V$, with constant [heat capacity at constant volume](../../../../heat-capacity-at-constant-volume.md), gives

$$
\boxed{U(T,V)=C_VT+U_0,}
$$

where $U_0$ is independent of both $T$ and $V$ and fixes the reference for [internal energy](../../../../internal-energy-split.md).

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 2](../../paper-2-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
