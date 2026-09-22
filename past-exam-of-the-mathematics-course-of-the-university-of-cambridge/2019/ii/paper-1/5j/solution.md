<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

An [exponential dispersion family](../../../../../exponential-dispersion-model.md) has densities of the form

$$
f(y;\theta,\phi)
=a(y,\phi)\exp\left\{\frac{y\theta-b(\theta)}{\phi}\right\},
$$

where $\theta$ is the [canonical parameter](../../../../../natural-parameter-of-an-exponential-family.md), $\phi>0$ is the [dispersion parameter](../../../../../dispersion-parameter.md), and the support does not depend on $\theta$. Its mean and variance are

$$
\mathbb E Y=b'(\theta),
\qquad
\operatorname{var}(Y)=\phi b''(\theta).
$$

For the given [Gamma distribution](../../../../../gamma-distribution.md), set

$$
\phi=\frac1\alpha,
\qquad
\theta=-\frac\lambda\alpha<0,
\qquad
b(\theta)=-\log(-\theta).
$$

Then

$$
a(y,\phi)
=\frac{y^{1/\phi-1}}{\Gamma(1/\phi)\phi^{1/\phi}}
$$

gives

$$
a(y,\phi)
\exp\left\{\frac{y\theta-b(\theta)}\phi\right\}
=\frac{\lambda^\alpha}{\Gamma(\alpha)}y^{\alpha-1}e^{-\lambda y}.
$$

Thus the gamma laws form the [Gamma exponential dispersion family](../../../../../gamma-exponential-dispersion-family.md).

Directly integrating, or using the [cumulant-generating function of a gamma distribution](../../../../../cumulant-generating-function-of-a-gamma-distribution.md),

$$
M_Y(t)=\left(\frac\lambda{\lambda-t}\right)^\alpha,
\qquad t<\lambda,
$$

so

$$
K_Y(t)=\log M_Y(t)
=-\alpha\log\left(1-\frac t\lambda\right).
$$

Differentiation at zero yields

$$
\boxed{\mathbb E Y=K_Y'(0)=\frac\alpha\lambda},
\qquad
\boxed{\operatorname{var}(Y)=K_Y''(0)=\frac\alpha{\lambda^2}}.
$$

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
