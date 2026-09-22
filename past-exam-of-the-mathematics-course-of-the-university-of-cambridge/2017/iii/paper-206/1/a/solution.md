<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [exponential dispersion family](../../../../../../exponential-dispersion-model.md) in the convention

$$
f(z;\theta,\phi)=\exp\left\{\frac{z\theta-b(\theta)}{\phi}+c(z,\phi)\right\},\qquad \phi>0.
$$

Assume that the support does not depend on the parameters, that $\theta$ is in the interior of the [natural parameter space](../../../../../../natural-parameter-space.md), and that differentiation can pass under the normalizing integral or sum. Differentiating $\int f=1$ at fixed [dispersion parameter](../../../../../../dispersion-parameter.md) gives

$$
0=\int\frac{z-b'(\theta)}{\phi}f(z;\theta,\phi)\,dz,
$$

so the [expectation](../../../../../../expected-value.md) is $b'(\theta)$. A second differentiation gives

$$
0=\mathbb E\left[\frac{(Z-b'(\theta))^2}{\phi^2}-\frac{b''(\theta)}{\phi}\right].
$$

Consequently

$$
\boxed{\mathbb E Z=b'(\theta),\qquad \operatorname{Var}(Z)=\phi b''(\theta).}
$$

Here $b$ is the [cumulant function of an exponential family](../../../../../../cumulant-function-of-an-exponential-family.md); the same identities follow by differentiating $\log\mathbb E e^{tZ}=[b(\theta+\phi t)-b(\theta)]/\phi$. For a known observation weight $w$, replace $\phi$ by $\phi/w$. These regularity assumptions for [differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) matter: differentiation of a parameter-dependent support can introduce additional boundary terms.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
