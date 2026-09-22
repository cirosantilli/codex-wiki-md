<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $\Delta_n=\sup_{\theta\in\Theta}|Q_n(\theta)-Q(\theta)|$. For any $\varepsilon>0$, the set

$$
F_\varepsilon=\{\theta\in\Theta:\|\theta-\theta_0\|\geq\varepsilon\}
$$

is [compact](../../../../../compact-space.md). If it is empty there is nothing to prove. Otherwise [continuity](../../../../../continuous-function.md) and the unique minimum give a strictly positive separation gap

$$
d_\varepsilon=\min_{\theta\in F_\varepsilon}\{Q(\theta)-Q(\theta_0)\}>0.
$$

Take any measurable attained [minimizer](../../../../../global-minimizer.md) of $Q_n$. Its defining inequality gives

$$
Q(\widehat\theta_n)\leq Q_n(\widehat\theta_n)+\Delta_n\leq Q_n(\theta_0)+\Delta_n\leq Q(\theta_0)+2\Delta_n.
$$

Consequently

$$
\boxed{\Pr(\|\widehat\theta_n-\theta_0\|\geq\varepsilon)\leq\Pr(\Delta_n\geq d_\varepsilon/2)\longrightarrow0.}
$$

This proves [argmin consistency under uniform convergence in probability](../../../../../argmin-consistency-under-uniform-convergence-in-probability.md). No [continuity](../../../../../continuous-function.md) of $Q_n$ is needed once the [minimizer](../../../../../global-minimizer.md) exists; compactness and [continuity](../../../../../continuous-function.md) concern the deterministic separation gap. The [uniform convergence in probability](../../../../../uniform-convergence-in-probability.md) assumption controls all candidate parameters, including the random [minimizer](../../../../../global-minimizer.md).

For the [estimating equation](../../../../../estimating-equation.md), fix $\varepsilon>0$ and put $a=\theta_0-\varepsilon$, $b=\theta_0+\varepsilon$. The prescribed signs make $\eta=\tfrac12\min\{-S(a),S(b)\}>0$. Pointwise [convergence in probability](../../../../../convergence-in-probability.md) at just these two points implies

$$
\Pr(S_n(a)\geq0)\leq\Pr(|S_n(a)-S(a)|\geq\eta)\longrightarrow0,
$$

and similarly $\Pr(S_n(b)\leq0)\to0$. With [probability](../../../../../probability.md) tending to one, $S_n(a)<0<S_n(b)$. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) then gives a zero inside $(a,b)$, and uniqueness identifies it with $\widehat\theta_n$. Hence

$$
\boxed{\Pr(|\widehat\theta_n-\theta_0|\geq\varepsilon)\leq\Pr(S_n(a)\geq0)+\Pr(S_n(b)\leq0)\longrightarrow0.}
$$

This is [consistency of a uniquely bracketed zero](../../../../../consistency-of-a-uniquely-bracketed-zero.md). It needs no monotonicity, no [continuity](../../../../../continuous-function.md) of the limit $S$, and no uniform convergence of the $S_n$. The bracket interval must lie in the domain of $S_n$: read literally, the printed sign condition for every positive $\varepsilon$ puts every real point into $\Theta$, so this requirement is satisfied. More generally it is enough to have an interval about $\theta_0$ and sign brackets arbitrarily close to it.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
