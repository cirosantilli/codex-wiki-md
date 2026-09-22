<h1 id="jensen-s-inequality">Jensen's inequality</h1>

↑ **Parent:** [Convex function](convex-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jensen's_inequality)

[Jensen's inequality](jensen-s-inequality.md) says that applying a [convex function](convex-function.md) to a [weighted mean](weighted-arithmetic-mean.md) cannot exceed the same [weighted mean](weighted-arithmetic-mean.md) of its outputs. For nonnegative weights $w_i$ with $\sum_{i=1}^n w_i=1$ and inputs $x_i$ in a [convex set](convex-set.md),

$$
f\left(\sum_{i=1}^n w_i x_i\right)\leq\sum_{i=1}^n w_i f(x_i).
$$

Nonnegative weights are essential: this is a [convex combination](convex-combination.md), rather than an arbitrary [affine combination](affine-combination.md). For two inputs it is precisely the defining [inequality](inequality-mathematics.md) for a [convex function](convex-function.md); repeatedly grouping inputs gives the finite weighted version.

Take $f(x)=x^2$, weights $1/4$ and $3/4$, and inputs $1$ and $3$. Their [weighted mean](weighted-arithmetic-mean.md) is $2.5$, so the two sides are

$$
f(2.5)=6.25\leq\tfrac14 f(1)+\tfrac34 f(3)=7.
$$

**The Jensen gap is $0.75$.** The [inequality](inequality-mathematics.md) measures the effect of replacing distinct inputs by one representative input before applying a nonlinear [function](function-split.md).

The probabilistic form uses an [integrable random variable](integrable-random-variable.md) $X$ taking values in an [interval](interval-mathematics.md) where $f$ is a [convex function](convex-function.md). If $f(X)$ is also an [integrable random variable](integrable-random-variable.md) and $\mathbb E X$ belongs to that [interval](interval-mathematics.md), then

$$
f(\mathbb E X)\leq\mathbb E[f(X)].
$$

The direction reverses for a [concave function](concave-function.md). For a [strictly convex function](strictly-convex-function.md), equality in the finite weighted form requires all inputs having positive weight to be equal; in the probabilistic form it requires $X$ to be constant [almost surely](almost-sure-convergence.md). An [affine function](affine-function.md) gives equality for any admissible distribution. [Boyd and Vandenberghe's slides, section 3.14, state the expectation form](https://stanford.edu/~boyd/cvxbook/bv_cvxslides.pdf).

For the [quadratic function](quadratic-function.md) $f(x)=x^2$ and a [random variable](random-variable-split.md) with a finite [second moment](second-moment.md), the difference between the two sides is exactly its [variance](variance-split.md):

$$
\mathbb E[X^2]-(\mathbb E X)^2=\operatorname{Var}(X)\geq0.
$$

Consider two equally likely values $2-d$ and $2+d$. Their [expected value](expected-value.md) stays at $2$ as $d$ increases, but their [variance](variance-split.md) is $d^2$. Thus the [expected value](expected-value.md) of the square grows from $4$ to $4+d^2$. For the [exponential function](exponential-function.md), the same two-point distribution gives $\mathbb E[e^X]=e^2\cosh d$, while $e^{\mathbb E X}=e^2$. Both are examples of [Jensen's inequality](jensen-s-inequality.md), but their [Jensen gaps](jensen-gap.md) depend differently on the spread of the inputs.

<a id="image-keeping-the-mean-fixed-while-spreading-the-inputs-increases-the-average-of-these-convex-functions"></a>
![](jensen-mean-and-spread.png)

**[Figure 36](#image-keeping-the-mean-fixed-while-spreading-the-inputs-increases-the-average-of-these-convex-functions). Keeping the mean fixed while spreading the inputs increases the average of these convex functions**. The [random variable](random-variable-split.md) takes $2-d$ and $2+d$ with equal [probability](probability.md). The [quadratic function](quadratic-function.md) produces a [Jensen gap](jensen-gap.md) of $d^2$, exactly the [variance](variance-split.md). The [exponential function](exponential-function.md) produces a [Jensen gap](jensen-gap.md) of $e^2(\cosh d-1)$, involving the [hyperbolic cosine](hyperbolic-cosine.md). The horizontal reference in each panel applies the [function](function-split.md) directly to the unchanged [expected value](expected-value.md) $2$.

Another useful choice is the [concave function](concave-function.md) $\log x$ on positive inputs. Its version of [Jensen's inequality](jensen-s-inequality.md) gives $\sum_iw_i\log x_i\leq\log(\sum_iw_ix_i)$. Applying the increasing [exponential function](exponential-function.md) shows that the weighted [geometric mean](geometric-mean.md) cannot exceed the weighted [arithmetic mean](arithmetic-mean.md). For the equally weighted inputs $1$ and $9$, these are $3$ and $5$. This recovers the [arithmetic-geometric mean inequality](arithmetic-geometric-mean-inequality.md) and illustrates how choosing one [function](function-split.md) can generate an entire family of bounds.

A short proof idea explains the probabilistic form. If $f$ has a [subgradient](subgradient.md) $g$ at $\mu=\mathbb E X$, the supporting [affine function](affine-function.md) gives $f(X)\geq f(\mu)+g(X-\mu)$. Taking the [expected value](expected-value.md) cancels the linear term because $\mathbb E[X-\mu]=0$. This argument applies, for example, to finite [convex functions](convex-function.md) on $\mathbb R$; more general [domains of a function](domain-of-a-function.md) need attention to endpoints and the existence of a [subgradient](subgradient.md).

[Johan Jensen](johan-jensen.md)'s 1906 paper “Sur les fonctions convexes et les inégalités entre les valeurs moyennes” is an early source for the connection between [convex functions](convex-function.md) and inequalities for [means](expected-value.md). [Jensen's original article and publication record, DOI 10.1007/BF02418571](https://zenodo.org/records/2371297).

**Table of contents**

- [Jensen gap](jensen-gap.md)
- [Sharp two-term convex power bound](sharp-two-term-convex-power-bound.md)

## ↑ Ancestors (6)

1. [Convex function](convex-function.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (21)

- [Finite-sample bias in a negative multinomial probability estimator](finite-sample-bias-in-a-negative-multinomial-probability-estimator.md)
- [Independent-set bound for biregular graphs](independent-set-bound-for-biregular-graphs.md)
- [Integral fluctuation theorem](integral-fluctuation-theorem.md)
- [Jarzynski equality](jarzynski-equality.md)
- [Jensen gap](jensen-gap.md)
- [Jensen's inequality](jensen-s-inequality.md)
- [L2-compatible initialization of grid data](l2-compatible-initialization-of-grid-data.md)
- [Lyapunov moment inequality](lyapunov-moment-inequality.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-9/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-57/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-1/21h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-2/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-2/19h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2/3f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-12/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-32/4/solution.md)
- [Sharp two-term convex power bound](sharp-two-term-convex-power-bound.md)
- [Weighted arithmetic-geometric mean inequality](weighted-arithmetic-geometric-mean-inequality.md)
- [Weighted geometric mean](weighted-geometric-mean.md)
