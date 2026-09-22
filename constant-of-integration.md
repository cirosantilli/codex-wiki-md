# Constant of integration

↑ **Parent:** [Antiderivative](antiderivative.md)

On a connected open [interval](interval-mathematics.md), if $F'=g$, every [antiderivative](antiderivative.md) of $g$ has the form $F+C$, where $C$ is a [constant function](constant-function.md). Indeed, two solutions satisfy $(G-F)'=0$: the [zero derivative on a connected open set](zero-derivative-on-a-connected-open-set.md) principle makes their difference constant. In one dimension, the [mean value theorem](mean-value-theorem.md) proves this on any closed subinterval. [Lebl, Basic Analysis I, Proposition 4.2.6: zero derivative on an interval](https://www.jirka.org/ra/html/sec_mvt.html)

An [initial condition](initial-condition.md) or [boundary condition](boundary-condition.md) can determine $C$. If a particular [antiderivative](antiderivative.md) is $F_0$ and $F(x_0)=y_0$, then

$$
\boxed{C=y_0-F_0(x_0).}
$$

For $g(x)=x^2$, $F_0(x)=x^3/3$ and $F(1)=2$, this gives $C=5/3$. Without that reference value, choosing $C=0$ simply selects one member of the family.

The freedom has a physical meaning in a simple kinematic model. A [velocity](velocity.md) $v(t)=at$, with constant [acceleration](acceleration.md) $a$, determines [position](position.md) only as $x(t)=at^2/2+C$. The [initial condition](initial-condition.md) $x(0)=x_0$ selects $C=x_0$; changing the starting [position](position.md) does not change the prescribed [velocity](velocity.md).

For the [differential equation](differential-equation-split.md) $T'=-B/r^2$ on $r>0$, the [antiderivative](antiderivative.md) is $T=B/r+C$. The [boundary condition](boundary-condition.md) $T(R_s)=T_s$ gives $C=T_s-B/R_s$. Discarding the [constant of integration](constant-of-integration.md) therefore needs a specified condition or an approximation that quantifies its effect. On a domain with several [connected components](connected-component.md), the freedom is larger: [antiderivatives on disconnected domains](antiderivatives-on-disconnected-domains.md) require a separate constant on each component.

**Table of contents**

- [Antiderivatives on disconnected domains](antiderivatives-on-disconnected-domains.md)

## ↑ Ancestors (8)

1. [Antiderivative](antiderivative.md)
2. [Integral](integral.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Additive constant](additive-constant.md)
- [Antiderivative](antiderivative.md)
- [Constant of integration](constant-of-integration.md)
- [Definite integral](definite-integral.md)
- [Integration by parts](integration-by-parts.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-8/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-8/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-74/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-72/1/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-71/3/b/solution.md)
