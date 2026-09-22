<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a high-[Reynolds number](../../../../../../reynolds-number.md) thermal, buoyancy force scales as $\rho_0g'a^3$ and inertial resistance scales as $\rho_0W^2a^2$. Their balance gives $W^2\propto g'a$. It is therefore natural to write a diameter-based [Froude number](../../../../../../froude-number.md) closure

$$
\boxed{W=F\sqrt{2ag'}.}
$$

The order-one coefficient $F$ accounts for the thermal's shape, entrainment and flow structure. The main resistance is inertial pressure or form drag and the momentum needed to entrain and accelerate surrounding water, rather than molecular skin friction. Added mass matters when the thermal accelerates, so the Froude closure is a quasi-steady approximation.

In a homogeneous ocean all of the leading [buoyancy](../../../../../../buoyancy.md) comes from the bubbles. Parts (a) and (b) give

$$
g'=g\phi=\frac{g\phi_0a_0^3}{(1-z/H_p)a^3}.
$$

Substituting into the speed law yields

$$
W=F\left[\frac{2g\phi_0a_0^3}{(1-z/H_p)(a_0+\alpha z)^2}\right]^{1/2}.
$$

For $z\gg a_0/\alpha$, this becomes

$$
\boxed{W\sim F\left[\frac{2\phi_0a_0^3g}{(1-\rho_0gz/p_0)\alpha^2z^2}\right]^{1/2}.}
$$

The square root is essential both physically and dimensionally. This approximation still requires dilute bubbles and retained gas; it is not a valid prediction of infinite speed where the pressure approximation approaches zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
