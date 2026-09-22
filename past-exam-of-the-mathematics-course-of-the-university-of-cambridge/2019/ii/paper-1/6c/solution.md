<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

In this discrete [age-structured population model](../../../../../age-structured-population-model.md), individuals of age $a\geq1$ present during the breeding season each produce $b_a$ newborns, so the number entering age zero is

$$
n_{0,t}=\sum_{a=1}^{\infty}n_{a,t}b_a.
$$

An age-$a$ individual survives the following winter with probability $1-\mu_a$ and is then age $a+1$ in the next year, giving

$$
n_{a+1,t+1}=(1-\mu_a)n_{a,t}.
$$

Together with the initial age distribution, these equations determine every later cohort.

Substitute $n_{a,t}=r_a\gamma^t$ into the survival equation. Then

$$
r_{a+1}=\frac{1-\mu_a}{\gamma}r_a,
$$

and iteration gives

$$
r_a=r_0\gamma^{-a}\prod_{i=0}^{a-1}(1-\mu_i).
$$

The birth equation becomes

$$
r_0=\sum_{a=1}^{\infty}r_ab_a
=r_0\sum_{a=1}^{\infty}
\left[\prod_{i=0}^{a-1}(1-\mu_i)\right]\gamma^{-a}b_a.
$$

A nonzero population mode therefore requires the [Discrete Euler-Lotka equation](../../../../../discrete-euler-lotka-equation.md)

$$
\boxed{\phi(\gamma)=1},
\qquad
\phi(\gamma)=\sum_{a=1}^{\infty}
\left[\prod_{i=0}^{a-1}(1-\mu_i)\right]\gamma^{-a}b_a.
$$

For nonnegative vital rates with at least one surviving reproductive age and enough decay to make the series finite, $\phi$ is continuous and strictly decreasing on $\gamma>0$, tends to infinity as $\gamma\downarrow0$, and tends to zero as $\gamma\to\infty$. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) gives one positive solution, and strict monotonicity makes it unique.

The value $\phi(1)$ is the expected lifetime offspring count under these fixed rates. Since $\phi$ decreases, $\phi(1)>1$ places the root at $\gamma>1$ and the population grows geometrically; $\phi(1)<1$ places it at $\gamma<1$ and the population shrinks. Equality gives replacement, $\gamma=1$.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
