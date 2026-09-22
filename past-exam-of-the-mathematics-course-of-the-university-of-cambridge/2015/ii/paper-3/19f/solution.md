<h1 id="19f/solution">Solution</h1>

↑ **Parent:** [19F](../19f.md)

On the [complex torus](../../../../../complex-torus.md) $\mathbb C/\Lambda$, the [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) $\wp$ is a degree-two map to the [Riemann sphere](../../../../../riemann-sphere.md), and its fibres are the pairs $\{z,-z\}$, with coalescence at the four branch points. An even [elliptic function](../../../../../elliptic-function.md) is constant on every fibre, so away from those branch points it descends to a meromorphic function $Q$ of $\wp$.

The descent also holds at a branch point. At a half-period $h$, evenness and periodicity give $f(h+u)=f(h-u)$, so its local [Laurent series](../../../../../laurent-series.md) uses only even powers of $u$. Also $\wp(h+u)-\wp(h)$ is a local coordinate proportional to $u^2$. At $0$, use $1/\wp(z)\sim z^2$ instead. Thus $Q$ extends meromorphically across every branch point and infinity. Every [meromorphic function](../../../../../meromorphic-function.md) on the [Riemann sphere](../../../../../riemann-sphere.md) is a [rational function](../../../../../rational-function.md), proving $f=Q\circ\wp$.

For a nonconstant rational function $Q=p/q$ in coprime form, $\deg Q=\max(\deg p,\deg q)$: a generic equation $p-wq=0$ has that many roots on the sphere. Degrees of holomorphic maps multiply under composition. Hence **the degree is**

$$
\boxed{\deg f=2\max(\deg p,\deg q).}
$$

Constant functions have degree zero. Degree two therefore occurs exactly when $Q$ is a [Möbius transformation](../../../../../mobius-transformation.md):

$$
\boxed{f(z)=\frac{a\wp(z)+b}{c\wp(z)+d},\qquad ad-bc\ne0.}
$$

Conversely every such function is even, elliptic and of degree two.

## ↑ Ancestors (10)

1. [19F](../19f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
