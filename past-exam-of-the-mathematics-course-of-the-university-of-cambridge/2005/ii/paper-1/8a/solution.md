<h1 id="8a/solution">Solution</h1>

↑ **Parent:** [8A](../8a.md)

A [Papperitz symbol](../../../../../papperitz-symbol.md) records the three regular singular points of a second-order [Fuchsian differential equation](../../../../../fuchsian-differential-equation.md) and the two local exponents at each. Exponents at infinity refer to solutions behaving as $z^{-\gamma}$, that is, to powers of the local coordinate $1/z$. Their sum satisfies the Fuchs relation: the six exponents add to one. The symbol represents the two-dimensional solution space, not one normalized solution by itself.

The specified exponents give the [Gauss hypergeometric equation](../../../../../gauss-hypergeometric-equation.md)

$$
z(1-z)u''+[c-(a+b+1)z]u'-ab\,u=0.
$$

Set $d=c-a-b$ and let $v=F(c-a,c-b;c;z)$. Its equation is

$$
z(1-z)v''+[c-(2c-a-b+1)z]v'-(c-a)(c-b)v=0.
$$

For $u=(1-z)^dv$, differentiation gives $u'=(1-z)^d[v'-dv/(1-z)]$ and $u''=(1-z)^d[v''-2dv'/(1-z)+d(d-1)v/(1-z)^2]$. Substitution into the first equation leaves $(1-z)^d$ times exactly the second equation: its $v'$ coefficient is $c-(a+b+1+2d)z$, and its $v$ coefficient simplifies to $-(c-a)(c-b)$. Hence $u$ solves the same equation as $F(a,b;c;z)$.

The symbol gives the same check geometrically: multiplication by $(1-z)^d$ shifts the exponents at one from $\{0,-d\}$ to $\{d,0\}$ and those at infinity from $\{c-a,c-b\}$ to $\{b,a\}$; it does not change the exponents at zero. Choose the branch with $(1-0)^d=1$. Then $u$ is analytic at zero and $u(0)=1$. For $c\notin\{0,-1,-2,\ldots\}$ the analytic recurrence uniquely determines this normalized solution, proving

$$
\boxed{F(a,b;c;z)=(1-z)^{c-a-b}F(c-a,c-b;c;z).}
$$

The identity continues wherever both sides are defined with compatible branches. At exceptional parameters where the stated normalization does not uniquely define an analytic function, a parameter-continuation convention is needed; the generic proof does not silently assume uniqueness there. This is [Euler's hypergeometric transformation](../../../../../euler-s-hypergeometric-transformation.md).

## ↑ Ancestors (10)

1. [8A](../8a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
