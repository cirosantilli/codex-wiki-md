<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Positivity means $u>0$ almost everywhere, since the real [logarithm](../../../../../logarithm.md) must belong to $L^1$. A [positivity-preserving operator](../../../../../positivity-preserving-linear-operator-on-l1.md) gives $s=Tu\ge0$. For fixed $x$, the scalar [shifted Poisson data fidelity](../../../../../shifted-poisson-data-fidelity.md) is $f_x(s)=s-g(x)\log(1+s)$, with

$$
f_x'(s)=1-\frac{g(x)}{1+s},\qquad f_x''(s)=\frac{g(x)}{(1+s)^2}>0.
$$

Composition with the [linear operator](../../../../../linear-operator.md) $T$ proves [convexity](../../../../../convex-function.md) in $u$, and strict [convexity](../../../../../convex-function.md) holds along pairs whose forward images differ on a set of positive measure. The admissible class itself is [convex](../../../../../convex-function.md): the [concavity of the logarithm](../../../../../concavity-of-the-logarithm.md) gives $\log(\theta u+(1-\theta)v)\ge\theta\log u+(1-\theta)\log v$, controlling its negative part, while $\log^+w\le w$ controls its positive part.

Because $|\Omega|=1$ and $\log(1+s)\ge0$, the [Jensen inequality](../../../../../jensen-s-inequality.md) gives the requested bound:

$$
\begin{aligned}
\int_\Omega[s-g\log(1+s)]\,dx
&\ge\|s\|_1-\|g\|_\infty\int_\Omega\log(1+s)\,dx\\
&\ge\|s\|_1-\|g\|_\infty\log(1+\|s\|_1)\\
&=\|Tu\|_1-\|g\|_\infty\log\|Tu+1\|_1.
\end{aligned}
$$

The final equality uses nonnegativity and the unit area. Since $t-G\log(1+t)\to\infty$, this controls the forward-image [norm](../../../../../norm.md) on energy sublevels.

**The printed strictly positive problem has no [minimizer](../../../../../global-minimizer.md).** This is [nonattainment under strict positivity for shifted Poisson fidelity](../../../../../nonattainment-under-strict-positivity-for-shifted-poisson-fidelity.md), rather than a failure of the coercivity calculation. Indeed, with $0<g<1$ and $s>0$, $\log(1+s)<s$ implies $f_x(s)>0$. Also $Tu$ cannot vanish identically for a strictly positive $u$. To see this, let $E_n=\{u\ge1/n\}$. If $Tu=0$, positivity and $0\le\chi_{E_n}\le nu$ give $T\chi_{E_n}=0$. But $\chi_{E_n}\to\chi_\Omega$ in $L^1$ and [continuity](../../../../../continuous-function.md) of $T$ would imply $T\chi_\Omega=0$, contradicting the hypothesis. Thus every admissible $u$ has positive fidelity and hence positive total energy.

Conversely, the constants $u_\varepsilon=\varepsilon\chi_\Omega$ are admissible, have zero [total variation](../../../../../total-variation.md), and satisfy

$$
0<E(u_\varepsilon)\le\varepsilon\|T\chi_\Omega\|_1\longrightarrow0.
$$

Their logarithms are integrable for each $\varepsilon>0$, but the [limit](../../../../../limit-of-a-function.md) is excluded. Therefore

$$
\boxed{\inf E=0,\qquad\operatorname{argmin}E=\varnothing\quad\text{in the printed domain}.}
$$

A bounded minimizing sequence and [bounded-variation compactness](../../../../../bounded-variation-compactness.md) do not repair a nonclosed positivity/[logarithm](../../../../../logarithm.md) constraint. In particular, a literal existence or uniqueness proof for that domain is impossible.

The natural correction is to minimize over $BV(\Omega)$ with $u\ge0$, omitting the unnecessary $\log u\in L^1$ condition: the fidelity only contains $\log(1+Tu)$, which is already integrable. Here is the full [existence for nonnegative shifted Poisson regularization](../../../../../existence-for-nonnegative-shifted-poisson-regularization.md) argument, also valid for any bounded nonnegative data $g$. Let $G=\|g\|_\infty$, $m_G=\inf_{t\ge0}\{t-G\log(1+t)\}>-\infty$, and take a minimizing sequence of energy at most $C$. The displayed bound gives $\|Tu_n\|_1\le C_1$ and $\alpha\operatorname{TV}(u_n)\le C-m_G$. Write $c_n=\int_\Omega u_n\ge0$. The [Poincaré inequality for total variation](../../../../../poincare-inequality-for-total-variation.md) and [mean control for positive imaging operators](../../../../../mean-control-for-positive-imaging-operators.md) yield

$$
c_n\|T\chi_\Omega\|_1\le\|Tu_n\|_1+\|T\|\|u_n-c_n\|_1
\le C_1+C_P\|T\|\operatorname{TV}(u_n).
$$

The denominator is nonzero, so the full $BV$ [norm](../../../../../norm.md) is bounded. [Bounded-variation compactness](../../../../../bounded-variation-compactness.md) gives $u_n\to u$ in $L^1$ along a subsequence, with $u\ge0$. [Continuity](../../../../../continuous-function.md) gives $Tu_n\to Tu$ in $L^1$. On $s\ge0$, $|f_x'(s)|\le1+G$, so the fidelity converges in the integral; [lower semicontinuity](../../../../../lower-semicontinuity.md) of variation completes the [direct method in the calculus of variations](../../../../../direct-method-in-the-calculus-of-variations.md).

For the actual printed data $0<g<1$, the corrected problem has the **unique [minimizer](../../../../../global-minimizer.md) $u=0$**, even if $T$ is not [injective](../../../../../injective-function.md). Zero attains energy zero. Any other zero-energy candidate would have both $Tu=0$ and $\operatorname{TV}(u)=0$; on the connected square, zero variation makes $u$ a nonnegative constant, and $T\chi_\Omega\ne0$ forces that constant to vanish. For general positive bounded data, an [injective](../../../../../injective-function.md) $T$ is a sufficient uniqueness condition, because its fidelity is [strictly convex](../../../../../strictly-convex-function.md); injectivity is not a necessary condition in every instance.

In the finite-dimensional interpretation, let $\lambda_{ij}=1+(Tu)_{ij}$. Independent [Poisson observations](../../../../../poisson-observation.md) with these intensities have negative [log-likelihood](../../../../../log-likelihood.md) $\sum_{ij}[\lambda_{ij}-g_{ij}\log\lambda_{ij}]+C(g)$. Removing the constant $\sum1$ gives precisely the stated fidelity. Thus the model is **Poisson counting noise with a unit background intensity**, or an approximate version of it for rescaled/[continuous](../../../../../continuous-function.md) grey values. Literal Poisson counts are integers; the constraint $0<g<1$ is a grey-value normalization, not a literal unscaled count sample.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
