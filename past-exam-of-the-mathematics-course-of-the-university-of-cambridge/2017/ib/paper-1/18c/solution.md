<h1 id="18c/solution">Solution</h1>

↑ **Parent:** [18C](../18c.md)

Assume $f$ is sufficiently smooth, for example $C^3$ near the exact trajectory. Write $f,f',f''$ at the current value, with $f'$ a [linear map](../../../../../linear-map.md) and $f''$ a bilinear map when the [ordinary differential equation](../../../../../ordinary-differential-equation.md) is vector valued. [Taylor expansion](../../../../../taylor-expansion.md) of the stages gives

$$
\begin{aligned}
k_2&=f+ha_1f'f+\tfrac12h^2a_1^2f''[f,f]+O(h^3),\\
k_3&=f+h(a_2+a_3)f'f+h^2\left(a_1a_3(f')^2f+\tfrac12(a_2+a_3)^2f''[f,f]\right)+O(h^3).
\end{aligned}
$$

The exact flow has [Taylor expansion](../../../../../taylor-expansion.md)

$$
y(t+h)=y+hf+\frac{h^2}{2}f'f+\frac{h^3}{6}\left(f''[f,f]+(f')^2f\right)+O(h^4).
$$

Matching the terms through $h^3$ in the [Runge-Kutta method](../../../../../runge-kutta-method.md) gives the sufficient [third-order conditions for an explicit Runge-Kutta method](../../../../../third-order-conditions-for-an-explicit-runge-kutta-method.md)

$$
\boxed{\begin{aligned}b_1+b_2+b_3&=1,\\b_2a_1+b_3(a_2+a_3)&=\tfrac12,\\b_2a_1^2+b_3(a_2+a_3)^2&=\tfrac13,\\b_3a_1a_3&=\tfrac16.\end{aligned}}
$$

For scalar $f$, replace $f''[f,f]$ by $f''f^2$ and $(f')^2f$ by $(f')^2f$ in the scalar sense. The resulting local error is $O(h^4)$; under a local [Lipschitz continuity](../../../../../lipschitz-continuity.md) assumption and bounded derivatives on a finite time interval, the standard one-step error recurrence gives global error $O(h^3)$, hence third order.

On the linear test equation $y'=\lambda y$, putting $z=h\lambda$ gives the [stability function](../../../../../stability-function.md)

$$
R(z)=1+z+\frac{z^2}{2}+\frac{z^3}{6},\qquad R(-5/2)=-\frac{47}{48}.
$$

Thus $\boxed{|R(-5/2)|=47/48<1}$, so $-5/2$ lies inside the [linear stability domain](../../../../../linear-stability-domain.md). The four order conditions are compatible, for example $a_1=1/2,a_2=-1,a_3=2$ and $(b_1,b_2,b_3)=(1/6,2/3,1/6)$.

## ↑ Ancestors (10)

1. [18C](../18c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
