<h1 id="14d/solution">Solution</h1>

↑ **Parent:** [14D](../14d.md)

A fixed point is locally attracting when its multiplier satisfies $|F'(x_*)|<1$ and repelling when $|F'(x_*)|>1$. A multiplier crossing $+1$ can create or destroy fixed points in a fold bifurcation, or exchange their stability when branches cross, as in a transcritical bifurcation. A multiplier crossing $-1$ gives a flip, or period-doubling bifurcation, in which a two-cycle can emerge. These are the two multiplier mechanisms; additional [symmetry](../../../../../symmetry-physics.md) can distinguish special cases at $+1$.

For the [logistic map](../../../../../logistic-map.md), the fixed points are

$$
x=0,\qquad x_*=1-\frac1\mu.
$$

The second lies in $[0,1]$ only for $\mu\ge1$. Their multipliers are $\mu$ and $2-\mu$. Thus zero attracts for $0<\mu<1$; the branches meet at $\mu=1$ and exchange stability, with the nonzero branch attracting for $1<\mu<3$. At $\mu=1$, positive orbits decrease to zero since $F(x)=x-x^2$. At $\mu=3$, put $x=2/3+z$. Then $z\mapsto-z-3z^2$ and its second iterate is

$$
z\mapsto z-18z^3-27z^4,
$$

so the fixed point is still weakly attracting at the bifurcation, although linear attraction has disappeared.

The supplied factorization gives the nonfixed two-cycle points for $\mu>3$:

$$
\boxed{x_\pm=\frac{\mu+1\pm\sqrt{(\mu-3)(\mu+1)}}{2\mu}.}
$$

They are interchanged by $F$. Using their sum and product in $F'(x_+)F'(x_-)$ gives

$$
(F^2)'(x_\pm)=4+2\mu-\mu^2.
$$

The two-cycle is attracting exactly for

$$
\boxed{3<\mu<1+\sqrt6.}
$$

It is born from the fixed point at multiplier $+1$ for the second iterate, and at $\mu=1+\sqrt6$ its multiplier reaches $-1$, giving the next period doubling. The boundary cycles are nonhyperbolic; the strict multiplier test is not a proof of attraction there.

Beyond this threshold the [logistic map](../../../../../logistic-map.md) undergoes further period doublings, with attracting cycles of periods $4,8,16,\ldots$ and then chaotic parameter ranges, interspersed with periodic windows. It is not correct to say that every parameter above this threshold is chaotic. At $\mu=4$, the substitution $x=\sin^2(\pi\theta)$ gives $F(x)=\sin^2(2\pi\theta)$, illustrating its chaotic doubling-map behavior.

## ↑ Ancestors (10)

1. [14D](../14d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
