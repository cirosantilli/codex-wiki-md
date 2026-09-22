<h1 id="a/3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Write $A(x)=x-x^2$, $q=1/(n+2)$ and $p=(n+1)/(n+2)$. Integrating the steady [mass conservation](../../../../../mass-conservation.md) equation from the head gives

$$
\boxed{H_0(x)=[(n+2)A(x)]^q,\qquad0<x<1.}
$$

For the time-dependent first-order equation $H_t+H^{n+1}H_x=1-2x$, [method of characteristics](../../../../../method-of-characteristics.md) gives $\dot x=H^{n+1}$ and $\dot H=1-2x$. Consequently $d[H^{n+2}/(n+2)-A(x)]/dt=0$. On a [characteristic](../../../../../characteristic-of-a-field.md) starting at $(\xi,0)$ with zero thickness,

$$
H^{n+2}=(n+2)[A(x)-A(\xi)],\qquad t=\int_\xi^x\frac{dx'}{[(n+2)(A(x')-A(\xi))]^p}.
$$

On a [characteristic](../../../../../characteristic-of-a-field.md) emitted by the boundary $x=0$, the invariant is zero and $H=H_0(x)$. The travel time of the one emitted at time zero is

$$
\boxed{f(x)=(n+2)^{-p}\int_0^x[z(1-z)]^{-p}\,dz=(n+2)^{-p}B_x(q,q).}
$$

The [incomplete beta function](../../../../../incomplete-beta-function.md) is finite at both endpoints because $0<p<1$ for the physical exponents $n>0$. Before [characteristic](../../../../../characteristic-of-a-field.md) crossings, the initial-data branch and boundary-data branch have the displayed forms in the source, with the appropriate emission time $t-f(x)$ for the latter.

[Glacier characteristic admissibility](../../../../../glacier-characteristic-admissibility.md) gives a substantive domain restriction. Factoring the invariant gives $A(x)-A(\xi)=(x-\xi)(1-x-\xi)$. A positive forward branch requires

$$
\boxed{0\leq\xi<x<1-\xi,\qquad0\leq\xi<1/2.}
$$

Equivalently it is the image of this parameter domain under $(\xi,x)\mapsto(x,t(\xi,x))$, restricted further to regions where that map is single-valued. [Characteristics](../../../../../characteristic-of-a-field.md) cannot start with positive thickness growth at $\xi>1/2$, where the prescribed initial rate $H_t=1-2\xi$ is negative. This is why **the printed piecewise expression is a formal [characteristic](../../../../../characteristic-of-a-field.md) construction, not a global nonnegative solution from a bare bed**. For example for $x>1/2$, putting $L_\xi=1-2\xi$ gives

$$
t(\xi,x)=(n+2)^{-p}L_\xi^{-n/(n+2)}B_{(x-\xi)/L_\xi}(q,q)\geq f(x).
$$

Both factors increase with $\xi$ there, so no positive initial-data branch exists at that $x$ for $0<t<f(x)$, contrary to a literal global reading of the first case. Compression can also make [characteristics](../../../../../characteristic-of-a-field.md) intersect; [entropy solutions](../../../../../entropy-solution.md) then require [shock waves](../../../../../shock-wave.md).

One can nevertheless give the exact zero-thickness endpoint locus of these formal [characteristics](../../../../../characteristic-of-a-field.md). Let $K=f(1)=(n+2)^{-p}B(q,q)$. At $x=1-\xi$ the change of variable $z=\xi+(1-2\xi)y$ gives

$$
t_{\rm end}(\xi)=K(1-2\xi)^{-n/(n+2)},\qquad\boxed{x_{\rm end}(t)=\frac12\left[1+\left(\frac Kt\right)^{(n+2)/n}\right],\quad t\geq K.}
$$

This is the formal snout locus inferred from the given [characteristic](../../../../../characteristic-of-a-field.md) family; it retreats from $1$ towards $1/2$. It is not justified as the physical terminus of an accumulating glacier formed from zero initial [ice](../../../../../ice.md). In particular it says nothing about a positive advancing snout at $t<K$. A physical [free boundary problem](../../../../../free-boundary-problem.md) must specify no ablation on a bare bed, maintain $H\geq0$, and select an [entropy solution](../../../../../entropy-solution.md) or retain the small slope regularization. Those additional conditions are absent from the printed first-order construction. Thus a unique global physical snout trajectory cannot be claimed from that construction alone. The steady endpoint remains $x=1$. The degenerate $n=0$ limit would instead have the same endpoint time $K$ for every initial [characteristic](../../../../../characteristic-of-a-field.md), so the inverted formula presumes $n>0$.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
