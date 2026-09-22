<h1 id="k/k3/solution">Solution</h1>

↑ **Parent:** [K3](../k3.md)

The [circle theorem](../../../../milne-thomson-circle-theorem.md) says that if a [complex potential](../../../../complex-potential-of-a-two-dimensional-potential-flow.md) $f$ has no singularities on or inside $|z|=a$ (and has the required analytic continuation there), then

$$
w(z)=f(z)+\overline{f(a^2/\bar z)}
$$

adds image singularities inside the circle and makes it a [streamline](../../../../streamline.md). On the circle $a^2/\bar z=z$, so $w=f(z)+\overline{f(z)}$ is real and its imaginary part is constant. This gives zero normal velocity. The reflected term is holomorphic where defined, as follows from its [power](../../../../power-function-of-a-statistical-test.md) series in $1/z$, and its singularities are precisely the reflected ones; the external original singularities are retained. This proves the construction, with an additive constant and any independently prescribed [circulation](../../../../circulation-physics.md) handled separately.

For the [fluid vortex](../../../../vortex-fluid-mechanics.md) use $f(z)=-i\Gamma\log(z-b)/(2\pi)$. Reflecting gives an opposite image at $d=a^2/b$ and also a term $-i\Gamma\log z/(2\pi)$, up to constants. The zero-[circulation](../../../../circulation-physics.md) circle-theorem construction has both these terms. To impose the specified [circulation](../../../../circulation-physics.md) $-\Gamma$ about the obstacle, add $+i\Gamma\log z/(2\pi)$, canceling the central term. Thus

$$
\boxed{w(z)=\frac{i\Gamma}{2\pi}\bigl(\log(z-d)-\log(z-b)\bigr)+\text{constant}.}
$$

It has the stated [circulation](../../../../circulation-physics.md) and the same impermeable boundary, since the added central-[fluid vortex](../../../../vortex-fluid-mechanics.md) [streamfunction](../../../../stream-function.md) is constant on the circle.

For the given [Blasius integral](../../../../blasius-force-theorem.md) take the obstacle contour counterclockwise. Inside it the sole singularity of

$$
w'(z)^2=-\frac{\Gamma^2}{4\pi^2}\left(\frac1{z-d}-\frac1{z-b}\right)^2
$$

is at $d$. Its [residue](../../../../residue.md) is $\Gamma^2/[2\pi^2(d-b)]$, from the cross term. The [residue theorem](../../../../residue-theorem.md) then gives

$$
F_x-iF_y=-\rho\pi\operatorname{Res}_{z=d}w'^2=\frac{\rho\Gamma^2}{2\pi(b-d)}.
$$

Therefore $\boxed{F_x=\rho\Gamma^2b/[2\pi(b^2-a^2)],\quad F_y=0}$. The force on the obstacle points toward the external [fluid vortex](../../../../vortex-fluid-mechanics.md).

## ↑ Ancestors (12)

1. [K3](../k3.md)
2. [K](../../k.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
