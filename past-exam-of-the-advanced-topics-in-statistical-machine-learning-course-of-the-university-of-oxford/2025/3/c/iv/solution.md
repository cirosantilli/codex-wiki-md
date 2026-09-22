<h1 id="3/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $x_n=x_*$, the notation of part (i) gives $b=a$, $d=k_{**}$, and $c=k_{**}+\sigma^2$. Write $v=\operatorname{Var}_{n-1}(f_*)=k_{**}-a^TA^{-1}a$. The remaining [covariance](../../../../../covariance.md) is then $v$ and the new observation's remaining [variance](../../../../../variance-split.md) is $v+\sigma^2$. Thus

$$
\boxed{\operatorname{Var}_{n-1}(f_*)-\operatorname{Var}_n(f_*)=\frac{v^2}{v+\sigma^2}=\frac{\operatorname{Var}_{n-1}(f_*)^2}{\operatorname{Var}_{n-1}(f_*)+\sigma^2}}.
$$

Equivalently,

$$
\boxed{\operatorname{Var}_n(f_*)=\frac{v\sigma^2}{v+\sigma^2}}.
$$

The expression is valid also when $v=0$ and $\sigma^2>0$. For $v>0$, a noiseless observation, interpreted as the limit $\sigma^2\downarrow0$, removes all remaining [variance](../../../../../variance-split.md) at the observed target.

**The source's assertion that the target input always gives the greatest reduction needs an additional hypothesis.** The reduction formula above does not require that assertion. For a counterexample, use the [linear kernel](../../../../../linear-kernel.md) $k(x,x')=xx'$ with $\sigma^2=1$ and target $x_*=1$. With no informative previous observations, $v=1$. This can also be arranged with $n-1=1$ by observing first at $x_1=0$, which has zero [covariance](../../../../../covariance.md) with all latent values. Observing at the target gives reduction $1/2$, whereas observing at $x_n=2$ gives

$$
\frac{k(2,1)^2}{k(2,2)+1}=\frac45>\frac12.
$$

Indeed this [Gaussian process](../../../../../gaussian-process-split.md) is $f(x)=xZ$ for a standard [normal random variable](../../../../../gaussian-random-variable.md) $Z$, so the measurement at $2$ observes the same unknown coefficient with a larger signal relative to its noise.

One sufficient extra condition is that the existing latent [posterior variance](../../../../../posterior-variance.md) be maximal at $x_*$ among all candidate inputs. To prove it, let $w=v_{n-1}(x)$ and $r=\operatorname{Cov}(f(x),f_*\mid\mathbf y_{1:n-1},\theta)$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $r^2\leq vw$. If $w\leq v$, then

$$
\Delta(x)=\frac{r^2}{w+\sigma^2}\leq\frac{vw}{w+\sigma^2}\leq\frac{v^2}{v+\sigma^2}=\Delta(x_*),
$$

because $w\mapsto w/(w+\sigma^2)$ is increasing. Thus target sampling is optimal under this extra condition, but it is not implied by the paper's arbitrary-[covariance function](../../../../../covariance-function.md) assumptions.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the advanced topics in statistical machine learning course of the University of Oxford](../../../../split.md)
6. [Advanced topics in statistical machine learning course of the University of Oxford](../../../../../advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics and statistics course of the University of Oxford](../../../../../year-4-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
