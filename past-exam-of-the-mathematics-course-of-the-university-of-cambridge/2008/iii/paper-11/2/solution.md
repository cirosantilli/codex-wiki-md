<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We construct the density and singular part, rather than assuming the desired [Lebesgue decomposition theorem](../../../../../lebesgue-decomposition-theorem.md). Put $\rho=\mu+\nu$, a finite [dominating measure](../../../../../dominating-measure.md), and use the real [Hilbert space](../../../../../hilbert-space-split.md) $L^2(\rho)$. The [linear functional](../../../../../linear-functional.md)

$$
T(g)=\int_\Omega g\,d\nu
$$

is well defined on its equivalence classes, since a $\rho$-null set is $\nu$-null. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and $\nu\leq\rho$ give

$$
|T(g)|\leq\nu(\Omega)^{1/2}\left(\int g^2\,d\nu\right)^{1/2}\leq\nu(\Omega)^{1/2}\|g\|_{L^2(\rho)}.
$$

By the [Riesz representation theorem](../../../../../riesz-representation-theorem.md), there is $h\in L^2(\rho)$ with $T(g)=\int gh\,d\rho$. Indicators of all measurable sets belong to this Hilbert space, so

$$
\nu(A)=\int_Ah\,d\rho,\qquad \mu(A)=\int_A(1-h)\,d\rho\quad(A\in\Sigma).
$$

The nonnegativity of these two [measures](../../../../../measure.md) forces $0\leq h\leq1$ almost everywhere. For instance, if $\rho(\{h\leq-1/n\})>0$, its $\nu$-[measure](../../../../../measure.md) would be negative; the analogous sets $\{h\geq1+1/n\}$ contradict positivity of $\mu$. Their countable union excludes every violation. Modify $h$ on its measurable $\rho$-null exceptional set so that these inequalities hold everywhere. This is the [Hilbert-space construction of dominated measure densities](../../../../../hilbert-space-construction-of-dominated-measure-densities.md).

Define

$$
B=\{h=1\},\qquad f=\begin{cases}h/(1-h),&h<1,\\0,&h=1.\end{cases}
$$

Then $B\in\Sigma$, $f$ is a nonnegative [measurable function](../../../../../measurable-function.md), and $\mu(B)=\int_B(1-h)\,d\rho=0$. The identity for integration against $\mu$ follows first for indicators, then for nonnegative simple functions and finally for all nonnegative functions by the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md). Applying it to $f\mathbf1_A$ gives

$$
\int_Af\,d\mu=\int_{A\setminus B}h\,d\rho=\nu(A\setminus B).
$$

In particular $\int_\Omega f\,d\mu=\nu(\Omega\setminus B)<\infty$, so $f\in L^1(\mu)$. Additivity on the disjoint measurable sets $A\setminus B$ and $A\cap B$ now gives

$$
\boxed{\nu(A)=\int_A f\,d\mu+\nu(A\cap B),\qquad \mu(B)=0.}
$$

This is the [Lebesgue decomposition from a sum-measure density](../../../../../lebesgue-decomposition-from-a-sum-measure-density.md): the first [measure](../../../../../measure.md) has a density, and the second is concentrated on a $\mu$-[null set](../../../../../null-set.md), so is [mutually singular](../../../../../mutually-singular-measures.md) with $\mu$.

The [absolute continuity of measures](../../../../../absolute-continuity-of-measures.md) condition $\nu\ll\mu$ means that $\mu(A)=0$ implies $\nu(A)=0$ for every $A\in\Sigma$. If this holds, then $\nu(B)=0$, eliminating the singular part above. Conversely, a [measure](../../../../../measure.md) of the form $\nu(A)=\int_Af\,d\mu$ vanishes on every $\mu$-null set. Therefore

$$
\boxed{\nu\ll\mu\iff\nu(A)=\int_Af\,d\mu\text{ for some nonnegative }f\in L^1(\mu).}
$$

Thus absolute continuity is exactly the absence of the singular part in this construction.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
