<h1 id="k/k3/solution">Solution</h1>

↑ **Parent:** [K3](../k3.md)

On the circle put $\zeta=ae^{i\theta}$. The [Joukowski map](../../../../joukowski-map.md) gives $z=2a\cos\theta$, so its image is the slit $S=[-2a,2a]$. Away from that circle, the inverse equation is $\zeta^2-z\zeta+a^2=0$. For $z\notin S$, neither root has modulus $a$, and their product is $a^2$, so exactly one root has modulus greater than $a$. Selecting that root defines the exterior inverse.

More explicitly, define $s(z)=\sqrt{z^2-4a^2}$ to be the branch analytic on $\mathbb C\setminus S$ normalized by $s(z)/z\to1$ at infinity. It is positive for real $z>2a$ and negative for real $z<-2a$. Then

$$
\boxed{g(z)=\frac{z+s(z)}2.}
$$

Existence and analyticity of this branch also follow from the exterior inverse: $J'(\zeta)=1-a^2/\zeta^2$ is nonzero for $|\zeta|>a$, so the selected simple root varies analytically; $s=2g-z$ has the stated normalization. The exterior map is injective because $J(\zeta_1)=J(\zeta_2)$ with distinct roots would imply $\zeta_1\zeta_2=a^2$, impossible for two exterior points. Thus $g$ is a conformal bijection throughout $\mathbb C\setminus S$.

The proposed potential is a uniform stream plus its cylinder doublet and the [circulation](../../../../circulation-physics.md) term. On $\zeta=ae^{i\theta}$, the first two terms sum to the real quantity $2Ua\cos(\theta-\alpha)$, while the imaginary part of the logarithmic term is the constant $-\Gamma\log a/(2\pi)$. Thus the cylinder is a [streamline](../../../../streamline.md). At infinity the [complex velocity](../../../../complex-velocity.md) tends to $Ue^{-i\alpha}$ and the [circulation](../../../../circulation-physics.md) is $\Gamma$, verifying both far-field conditions. Logarithms may be chosen locally; their derivative gives a single-valued velocity.

Composition therefore gives the plate potential

$$
\boxed{w(z)=U\left(g(z)e^{-i\alpha}+\frac{a^2e^{i\alpha}}{g(z)}\right)-\frac{i\Gamma}{2\pi}\log g(z).}
$$

At the [edge](../../../../edge-of-a-graph.md) $z=2a$, corresponding to $\zeta=a$, the physical [complex velocity](../../../../complex-velocity.md) is $W'(\zeta)/J'(\zeta)$. Since the denominator has a simple zero, finiteness requires

$$
W'(a)=-2iU\sin\alpha-\frac{i\Gamma}{2\pi a}=0,
$$

which is exactly

$$
\boxed{\Gamma+4\pi Ua\sin\alpha=0.}
$$

With this cancellation, the limiting ratio is $W''(a)/J''(a)$. The Kutta value of the [circulation](../../../../circulation-physics.md) gives $W''(a)=2U\cos\alpha/a$ and $J''(a)=2/a$. Hence the finite [edge](../../../../edge-of-a-graph.md) velocity is

$$
\boxed{u-iv=U\cos\alpha,\quad\text{or }(u,v)=(U\cos\alpha,0).}
$$

## ↑ Ancestors (12)

1. [K3](../k3.md)
2. [K](../../k.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
