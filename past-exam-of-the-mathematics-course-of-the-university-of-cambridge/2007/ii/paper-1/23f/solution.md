<h1 id="23f/solution">Solution</h1>

↑ **Parent:** [23F](../23f.md)

Use [stereographic projection](../../../../../stereographic-projection.md) charts $\varphi(X,Y,Z)=(X+iY)/(1-Z)$ away from the north pole and $\psi(X,Y,Z)=(X-iY)/(1+Z)$ away from the south pole. On their overlap $\psi=1/\varphi$, a [holomorphic](../../../../../complex-differentiability-at-a-point.md) transition function, defining the [Riemann sphere](../../../../../riemann-sphere.md).

Where $F$ avoids the north pole, $\varphi\circ F$ is an ordinary holomorphic function exactly when $F$ is holomorphic. Near a north-pole value, the other chart gives $\psi\circ F=1/(\varphi\circ F)$; a zero of this holomorphic coordinate becomes a pole of $\varphi\circ F$. This proves the correspondence with [meromorphic functions](../../../../../meromorphic-function.md). On a disconnected domain one must also allow components mapped constantly to infinity, or state the correspondence on each nonconstant component. Applying the same reciprocal charts at source and target infinity shows that every nonconstant [rational function](../../../../../rational-function.md) defines a holomorphic sphere map.

The multiplicity of the value $a$ at infinity is the zero order at $w=0$ of $f(1/w)-a$ when $a$ is finite, and of $1/f(1/w)$ when $a=\infty$. For coprime polynomials $P,Q$, the [degree of a rational map of the Riemann sphere](../../../../../degree-of-a-rational-map-of-the-riemann-sphere.md) is $n=\max(\deg P,\deg Q)$, also its total number of poles with multiplicities.

The quotient rule $f'=(P'Q-PQ')/Q^2$ gives the upper bound $\deg f'\le2n$. Each finite pole of order $m$ contributes order $m+1$ to $f'$. If $\deg P>\deg Q$, infinity contributes an additional order $\deg P-\deg Q-1$ when this is positive. Counting gives the [degree bounds for the derivative of a rational function](../../../../../degree-bounds-for-the-derivative-of-a-rational-function.md)

$$
\boxed{n-1\le\deg f'\le2n.}
$$

The lower bound is attained by $f=z^n$; the upper by $f=1/(z^n-1)$, whose $n$ simple finite poles become double poles. Product degrees are **not additive**: $f=z$ and $g=(z+1)/z$ both have degree one, but $fg=z+1$ also has degree one because the zero and pole cancel.

## ↑ Ancestors (10)

1. [23F](../23f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
