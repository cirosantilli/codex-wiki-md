<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On an outward-oriented sphere of radius $R>0$, the [electric field](../../../../../electric-field-split.md) is normal with constant magnitude $A/R^2$. Thus its [flux](../../../../../flux.md) is

$$
\boxed{\iint_{S_R}E\cdot d\boldsymbol S=\frac A{R^2}(4\pi R^2)=4\pi A=\frac Q{\epsilon_0}.}
$$

It is independent of $R$. There is no contradiction with [solution](../i/solution.md): the classical [divergence theorem](../../../../../divergence-theorem.md) cannot be applied to a full ball while pretending that $E$ is smooth at its center. On a punctured ball the outer flux and the inward-normal inner flux cancel, in agreement with zero ordinary [divergence](../../../../../divergence.md) there.

The three-dimensional [Dirac delta distribution](../../../../../dirac-delta-function.md) $\delta^{(3)}(r)$ is supported at the origin and satisfies the sampling identity

$$
\int_{\mathbb R^3}\delta^{(3)}(r)\varphi(r)\,dV=\varphi(0)
$$

for smooth compactly supported test functions $\varphi$. It is not an ordinary function with a finite value at zero; its total integral is one, and translating it moves the point at which the test function is sampled.

The globally valid source equation is

$$
\boxed{\nabla\cdot E=4\pi A\delta^{(3)}(r)=\frac Q{\epsilon_0}\delta^{(3)}(r).}
$$

For a direct weak verification, excise a ball of radius $\varepsilon$ and integrate $-E\cdot\nabla\varphi$ outside it. Since the ordinary [divergence](../../../../../divergence.md) vanishes there, the result is $A\int_{S^2}\varphi(\varepsilon\hat r)\,d\Omega\to4\pi A\varphi(0)$. This is precisely the displayed [distributional divergence](../../../../../distributional-divergence.md) and restores the [divergence theorem](../../../../../divergence-theorem.md) with the [point charge](../../../../../point-charge.md) included.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [2019 resit](../../../../2019-resit-split.md)
5. [Past exam of the mathematical methods II course of the University of Oxford](../../../../split.md)
6. [Mathematical methods II course of the University of Oxford](../../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

## ← Incoming links (1)

- [Solution](../i/solution.md)
