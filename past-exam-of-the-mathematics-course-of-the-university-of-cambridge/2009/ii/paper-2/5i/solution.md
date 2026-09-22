<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

An [exponential dispersion family](../../../../../exponential-dispersion-model.md) has density or mass function

$$
p(y;\theta,\phi)=\exp\left\{\frac{y\theta-b(\theta)}{a(\phi)}+c(y,\phi)\right\},
$$

with support independent of the natural parameter $\theta$. Usually $a(\phi)=\phi/w$ for a known weight $w$. For the [Poisson distribution](../../../../../poisson-distribution.md), identify

$$
\theta=\log\lambda,\qquad b(\theta)=e^\theta,\qquad a(\phi)=1,\qquad c(y,\phi)=-\log(y!),\quad y\in\mathbb N_0.
$$

The dispersion is fixed at one. Differentiating the normalizing identity gives $\mathbb EY=b'(\theta)$; differentiating again gives $\operatorname{Var}Y=a(\phi)b''(\theta)$. Here both [derivatives](../../../../../derivative.md) equal $e^\theta=\lambda$, so

$$
\boxed{\mathbb EY=\lambda,\qquad\operatorname{Var}Y=\lambda,\qquad V(\mu)=\mu.}
$$

The [variance function](../../../../../variance-function.md) expresses $b''(\theta)$ in terms of the mean $\mu$. The [canonical link function](../../../../../canonical-link-function.md) maps the mean to the natural parameter, so **the Poisson canonical link is $g(\mu)=\log\mu$**.

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
