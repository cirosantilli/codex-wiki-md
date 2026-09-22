<h1 id="k/k3/solution">Solution</h1>

↑ **Parent:** [K3](../k3.md)

On $\zeta=ae^{i\theta}$, the [Joukowski map](../../../../joukowski-map.md) gives $z=2a\cos\theta$, so the image is the segment $S=[-2a,2a]$. Solving the resulting quadratic gives the inverse candidates

$$
\zeta=\frac12\left(z\pm\sqrt{z^2-4a^2}\right).
$$

On $D=\mathbb C\setminus[-2a,2a]$, choose the analytic square [root](../../../../root-of-a-root-system.md) $s(z)$ of $z^2-4a^2$ characterized by $s(z)/z\to1$ at infinity. One explicit definition is

$$
s(z)=(z+2a)\sqrt{\frac{z-2a}{z+2a}},
$$

where the square [root](../../../../root-of-a-root-system.md) on the right is the [principal square root](../../../../principal-square-root-of-a-complex-number.md). Its argument never lies on the nonpositive real axis for $z\in D$, so this defines the required [holomorphic function](../../../../holomorphic-function-split.md). Then $g(z)=(z+s(z))/2\sim z$.

The two quadratic roots have product $a^2$. For $z\notin S$, neither [root](../../../../root-of-a-root-system.md) lies on $|\zeta|=a$, since that circle maps into $S$. Consequently exactly one [root](../../../../root-of-a-root-system.md) lies outside the circle, and it is the branch $g$ chosen at infinity. Also, if two exterior points have the same image, then

$$
(\zeta_1-\zeta_2)\left(1-\frac{a^2}{\zeta_1\zeta_2}\right)=0,
$$

whose second factor cannot vanish. Thus the [Joukowski map](../../../../joukowski-map.md) is a [conformal map](../../../../conformal-map.md) from $|\zeta|>a$ onto $D$, and $g$ is [conformal](../../../../conformal-map.md) throughout $D$. The two endpoints are branch points and are excluded.

The [complex potential](../../../../complex-potential-of-a-two-dimensional-potential-flow.md) in the circle plane is the sum of the [uniform flow](../../../../uniform-flow.md) term $Ue^{-i\alpha}\zeta$, its circle-image term $Ua^2e^{i\alpha}/\zeta$, and the [point vortex](../../../../line-vortex.md) term $-i\Gamma\log\zeta/(2\pi)$. On $\zeta=ae^{i\theta}$, the first two sum to $2Ua\cos(\theta-\alpha)$, which is real, while the imaginary part of the vortex term is the constant $-\Gamma\log a/(2\pi)$. Hence the circle is a streamline, giving no normal flow. At infinity the first term gives the required [uniform flow](../../../../uniform-flow.md); the logarithmic term supplies circulation $\Gamma$. The potential may be multivalued by a real constant, but its velocity is single-valued.

Conformal transport therefore gives

$$
\boxed{w(z)=U\left(g(z)e^{-i\alpha}+\frac{a^2e^{i\alpha}}{g(z)}\right)
-\frac{i\Gamma}{2\pi}\log g(z).}
$$

In the frame where the plate is horizontal, its length is $4a$ and the stream has angle $\alpha$; rotating the frame gives the equivalent incidence description. The [complex velocity](../../../../complex-velocity.md) is

$$
\frac{dw}{dz}=\frac{W'(\zeta)}{1-a^2/\zeta^2}.
$$

At the trailing edge $z=2a$, corresponding to $\zeta=a$, the denominator has a simple zero. Finite velocity requires

$$
0=W'(a)=-2iU\sin\alpha-\frac{i\Gamma}{2\pi a},
$$

so the [Kutta condition](../../../../kutta-condition.md) is

$$
\boxed{\Gamma=-4\pi Ua\sin\alpha.}
$$

With this choice, cancellation of the common zero gives

$$
\left.\frac{dw}{dz}\right|_{z=2a}
=\frac{W''(a)}{2/a}
=Ue^{i\alpha}+\frac{i\Gamma}{4\pi a}
=\boxed{U\cos\alpha}.
$$

Thus the limiting velocity has zero transverse component and is tangent to the plate.

## ↑ Ancestors (12)

1. [K3](../k3.md)
2. [K](../../k.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
