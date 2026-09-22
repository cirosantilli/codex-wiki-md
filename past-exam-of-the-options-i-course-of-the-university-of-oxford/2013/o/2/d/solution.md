<h1 id="o/2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The further observation is independent of the earlier observations conditional on $\theta$. Integrate its conditional success [probability](../../../../../probability.md) against the posterior:

$$
\mathbb P(X_{n+1}=1\mid x)=\int_0^1\theta\,\pi(\theta\mid x)d\theta=\frac{B(A+1,B)}{B(A,B)}.
$$

The given factorial formula for the [beta function](../../../../../beta-function.md) gives this ratio as $A/(A+B)$. Thus the [posterior predictive probability](../../../../../posterior-predictive-probability.md) is

$$
\boxed{\mathbb P(X_{n+1}=1\mid x)=\frac{a+s}{a+b+n}.}
$$

It is the posterior mean of the Bernoulli success parameter. Independence here is conditional: sharing the uncertain parameter generally makes past and future observations dependent before conditioning on it.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [2](../../2.md)
3. [O](../../../o.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
