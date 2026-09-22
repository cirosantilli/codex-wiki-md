# Noise amplification by differentiation of a linear interpolant

↑ **Parent:** [Ill-posedness of numerical differentiation](ill-posedness-of-numerical-differentiation.md)

For [linear interpolation](linear-interpolation.md) at zero and $h>0$, an error $\delta$ in the second sampled value, with the first exact, changes the [linear interpolant](linear-interpolant.md) by $\Delta p(x)=\delta x/h$. On $[0,h]$, its [uniform norm](supremum-norm.md) is exactly $|\delta|$, whereas the [derivative](derivative.md) change is the constant $\delta/h$. With independent absolute bounds $|\delta_0|,|\delta_1|\leq\delta$ on both samples, the value change remains at most $\delta$ and the [derivative](derivative.md) change is at most $2\delta/h$, attained for opposite endpoint errors.

Thus bounded absolute sample noise can remain bounded under value [interpolation](interpolation-split.md) while becoming unbounded under [numerical differentiation](numerical-differentiation.md) as $h\to0$. Fixed nonzero sample noise also prevents exact convergence of the value approximation; stability against perturbations and convergence to exact data are different assertions. For a second-sample error $a\epsilon(h)$ with fixed $a>0$, value convergence requires $\epsilon(h)\to0$, while [derivative](derivative.md) convergence requires $\epsilon(h)=o(h)$ in [little o notation](little-o-notation.md), in addition to vanishing [truncation error](truncation-error.md).

## ↑ Ancestors (7)

1. [Ill-posedness of numerical differentiation](ill-posedness-of-numerical-differentiation.md)
2. [Numerical differentiation](numerical-differentiation.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Ill-posedness of numerical differentiation](ill-posedness-of-numerical-differentiation.md)
- [Linear interpolant](linear-interpolant.md)
- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2015/2/c/iii/solution.md)
