<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use an [independent](../../../../independent-random-variables.md) copy $(x',y')$ of $(x,y)$ under the [product measure](../../../../product-measure.md) $\Pi\otimes\Pi$. Write $q=y-x$, $q'=y'-x'$, and

$$
r_t=z_t-z'_t=(1-t)(x-x')+t(y-y'),\qquad a=q-q'.
$$

Since the [pushforward measure](../../../../pushforward-measure.md) of $\Pi\otimes\Pi$ under $(z_t,z'_t)$ is $\mu_t\otimes\mu_t$, the [interaction energy](../../../../interaction-energy.md) is

$$
\mathcal W[\mu_t]=\frac12\iint W(r_t)\,d\Pi(x,y)\,d\Pi(x',y').
$$

Two applications of the [chain rule](../../../../chain-rule.md) give

$$
\boxed{\frac{d^2}{dt^2}\mathcal W[\mu_t]=\frac12\iint (q-q')^TD^2W(z_t-z'_t)(q-q')\,d\Pi\,d\Pi'.}
$$

The factor $1/2$ is retained. This classical identity requires [differentiation under the integral sign](../../../../differentiation-under-the-integral-sign.md) to be justified, just as in part (b). Bounded [Hessian matrix](../../../../hessian-matrix.md) of $W$ is sufficient, since $|q-q'|^2\leq2|q|^2+2|q'|^2$ is integrable; compactly supported endpoints are another sufficient case. The printed quadratic-growth condition alone does not provide this domination.

The failure can occur for the [interaction energy](../../../../interaction-energy.md) too. Take the even [interaction potential](../../../../interaction-potential.md) $W(x)=1-\cos(2\pi x^3)$ and replace the endpoint [probability measures](../../../../probability-measure.md) in part (b) by $\frac12\delta_0+\frac12\mu$ and $\frac12\delta_0+\frac12\nu$. Keep the origin fixed and translate every other atom by one. This coupling is increasing on the line, hence is optimal: its assigned values extend to a nondecreasing [transport map](../../../../transport-map.md), which is the [gradient](../../../../gradient.md) of a [convex function](../../../../convex-function.md). Differences between translated atoms remain integers, so their mutual interaction vanishes. Only interactions with the origin contribute, giving $\mathcal W[\mu_t]=F(t)/4$, with $F$ from part (b). It therefore also lacks a finite classical [second derivative](../../../../second-derivative.md) at $t=1/2$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the optimal transport and partial differential equations course of the University of Oxford](../../../split.md)
5. [Optimal transport and partial differential equations course of the University of Oxford](../../../../optimal-transport-and-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
