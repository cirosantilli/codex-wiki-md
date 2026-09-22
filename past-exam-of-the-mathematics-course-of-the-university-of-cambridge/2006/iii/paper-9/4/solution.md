<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $n=km$, with positive integers $k,m$, and put $Q=P^m$. [Polynomial](../../../../../polynomial-split.md) substitution respects congruence, so $Q(z)\equiv z\pmod{Q(z)-z}$ implies inductively $Q^j(z)\equiv z$ for every $j\geq1$. Since $Q^k=P^n$,

$$
\boxed{P^m(z)-z\mid P^n(z)-z.}
$$

Equivalently one can factor each $Q^{j+1}(z)-Q^j(z)$ by $Q(z)-z$ and telescope. If $Q(z)-z$ is identically zero, then $Q$ is the identity and $P^n-z$ is also zero, so the assertion still holds in the sense that the latter is a [polynomial](../../../../../polynomial-split.md) multiple of the former.

For the [holomorphic cycle](../../../../../cycle-of-a-holomorphic-map.md), the [chain rule](../../../../../chain-rule.md) gives

$$
(P^n)'(w_j)=P'(w_j)P'(w_{j+1})\cdots P'(w_{j+n-1}),
$$

with indices cyclically understood. These are the same product at every point. If its modulus is less than one at one point, it is less than one at every point. [Taylor expansion](../../../../../taylor-expansion.md) of each return map gives a contracting neighborhood of its [fixed point](../../../../../fixed-point.md), exactly as in question 1. Hence **every point of the [holomorphic cycle](../../../../../cycle-of-a-holomorphic-map.md) is attracting for $P^n$ whenever one is**; a zero factor makes every return [periodic-orbit multiplier](../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) zero.

For the quadratic family, factor the second-iterate fixed-point equation:

$$
P^2(z)-z=(z^2-z+c)(z^2+z+c+1).
$$

The first factor gives [fixed points](../../../../../fixed-point.md). A root of the second is also fixed only if subtracting the two factors gives $2z+1=0$, so $z=-1/2$ and $c=-3/4$. If $c\ne-3/4$, the second factor has discriminant $-4c-3\ne0$ and has two distinct roots, neither fixed. They are exchanged by $P$, since each is fixed by $P^2$ but not by $P$, and form an exact two-cycle. Therefore the unique parameter with no exact two-cycle is

$$
\boxed{c=-\frac34.}
$$

At this parameter,

$$
\boxed{P^2(z)-z=(z-3/2)(z+1/2)^3.}
$$

Thus the four finite solutions counted with multiplicity are $3/2$ once and $-1/2$ three times: there are only two distinct finite solutions, both already fixed by $P$. The [periodic-orbit multiplier](../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) at $3/2$ is three (nine for $P^2$), so it is repelling. At $-1/2$ the [periodic-orbit multiplier](../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) for $P$ is minus one; for $P^2$ it is one. Indeed, with $u=z+1/2$, the local first-return expression for $P$ is $-u+u^2$, and its square is $u-2u^3+u^4$. This is a parabolic return with a triple fixed-point root. The two-cycle has merged into this [fixed point](../../../../../fixed-point.md); the triple root is not three distinct [periodic points](../../../../../periodic-point.md). In the [Mandelbrot set](../../../../../mandelbrot-set.md) picture this is the [period-two bulb](../../../../../period-two-bulb-of-the-mandelbrot-set.md)'s attachment to the [main cardioid](../../../../../main-cardioid-of-the-mandelbrot-set.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
