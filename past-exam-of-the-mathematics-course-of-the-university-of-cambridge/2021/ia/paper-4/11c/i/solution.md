<h1 id="11c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $e_i'(t)$ be a [Cartesian basis](../../../../../../cartesian-basis.md) fixed in the rotating frame. A vector $A=A_i'e_i'$ then satisfies

$$
\left(\frac{dA}{dt}\right)_S
=\dot A_i'e_i'+A_i'\dot e_i'
=\left(\frac{dA}{dt}\right)_{S'}+\omega\times A,
$$

because a [derivative of a body-fixed basis vector](../../../../../../derivative-of-a-body-fixed-basis-vector.md) is $\dot e_i'=\omega\times e_i'$. Applying this transport formula twice to $r$ gives, for constant $\omega$,

$$
a_S=a_{S'}+2\omega\times v_{S'}+\omega\times(\omega\times r).
$$

The second and third terms correspond to [Coriolis acceleration](../../../../../../coriolis-acceleration.md) and [centrifugal acceleration](../../../../../../centrifugal-acceleration.md) in the rotating description.

For the bead, use cylindrical unit vectors $(e_r,e_\phi,e_z)$ with $e_z$ upward and

$$
r=R(\sin\theta\,e_r-\cos\theta\,e_z),
\qquad \dot e_r=\omega e_\phi.
$$

Projection of $m\ddot r=-mg e_z+N$ along the wire tangent $\cos\theta\,e_r+\sin\theta\,e_z$ eliminates the smooth-wire [normal force](../../../../../../normal-force.md) $N$ and gives

$$
\boxed{\ddot\theta=(\omega^2\cos\theta-g/R)\sin\theta}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11C](../../11c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
