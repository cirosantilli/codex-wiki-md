<h1 id="9b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work in one fixed [inertial frame](../../../../../../inertial-frame.md), and take positive [velocity](../../../../../../velocity.md) in the rocket's direction. During $d\tau$, the rocket ejects the positive amount of [mass](../../../../../../mass.md) $-m'(\tau)d\tau$. Its exhaust has inertial velocity $v(\tau)-u$, by the [Galilean transformation](../../../../../../galilean-transformation.md) of velocities. Once expelled, that material retains its velocity because it experiences no external [force](../../../../../../force.md). The system's [momentum](../../../../../../momentum.md) is therefore the rocket momentum plus the sum of all these exhaust momenta:

$$
P(t)=m(t)v(t)-\int_0^t[v(\tau)-u]m'(\tau)\,d\tau.
$$

The minus sign comes from the positive expelled mass being $-m'(\tau)d\tau$.

Differentiate, applying the product rule to the rocket [momentum](../../../../../../momentum.md) and the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) to the integral:

$$
P'=m'v+mv'-(v-u)m'=mv'+um'.
$$

The [momentum conservation](../../../../../../momentum-conservation.md) law thus gives **the nonrelativistic [rocket equation](../../../../../../rocket-equation.md)**

$$
\boxed{mv'+um'=0}.
$$

The same bookkeeping for [kinetic energy](../../../../../../kinetic-energy.md) gives

$$
K(t)=\frac12m(t)v(t)^2-\frac12\int_0^t[v(\tau)-u]^2m'(\tau)\,d\tau.
$$

Its derivative is

$$
K'=mvv'+\frac12\bigl[v^2-(v-u)^2\bigr]m'
=mvv'+uvm'-\frac12u^2m'
=-\frac12u^2m',
$$

where the [rocket equation](../../../../../../rocket-equation.md) cancels the first two terms. Thus **kinetic energy increases during mass ejection**, with $\boxed{K'=-u^2m'/2>0}$ when $u>0$ and $m'<0$. This does not violate [conservation of energy](../../../../../../conservation-of-energy.md): the increase comes from stored [internal energy](../../../../../../internal-energy.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9B](../../9b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
