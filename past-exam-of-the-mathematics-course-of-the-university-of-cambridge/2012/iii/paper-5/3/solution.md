<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Construct the densities using the [Riesz representation theorem](../../../../../riesz-representation-theorem.md) for a [Hilbert space](../../../../../hilbert-space-split.md), rather than assuming the [measure](../../../../../measure.md)-decomposition conclusion. Put $\rho=\mu+\nu$, a finite [dominating measure](../../../../../dominating-measure.md), and work in the real [L2 space](../../../../../l2-space-is-a-hilbert-space.md) $L^2(\rho)$. The [linear functional](../../../../../linear-functional.md)

$$
L(g)=\int_\Omega g\,d\nu
$$

is well-defined on its equivalence classes because $\nu\le\rho$. By the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md),

$$
|L(g)|\le\nu(\Omega)^{1/2}
\left(\int_\Omega |g|^2\,d\nu\right)^{1/2}
\le\nu(\Omega)^{1/2}\|g\|_{L^2(\rho)}.
$$

Thus the [Riesz representation theorem](../../../../../riesz-representation-theorem.md) supplies $h\in L^2(\rho)$ such that $L(g)=\int gh\,d\rho$. Since $\rho$ is finite, $h$ is also [integrable](../../../../../integrability.md). Testing $g=1_A$ gives

$$
\nu(A)=\int_Ah\,d\rho,\qquad
\mu(A)=\int_A(1-h)\,d\rho\qquad(A\in\Sigma).
$$

The first identity and nonnegativity of $\nu$ rule out a positive-[measure](../../../../../measure.md) set where $h<0$; for example, test $\{h\le-1/n\}$. The second identity and nonnegativity of $\mu$ similarly rule out $\{h\ge1+1/n\}$. Modify a measurable representative on a $\rho$-[null set](../../../../../null-set.md) so that $0\le h\le1$ everywhere. This is the [Hilbert-space construction of dominated measure densities](../../../../../hilbert-space-construction-of-dominated-measure-densities.md).

Set

$$
B=\{h=1\},\qquad
f=
\begin{cases}
h/(1-h),&h<1,\\
0,&h=1.
\end{cases}
$$

Then $B\in\Sigma$ and $\mu(B)=0$. The indicator identities for $\mu$ extend to integrals of nonnegative [measurable functions](../../../../../measurable-function.md) by approximation with [simple functions](../../../../../simple-function.md) and the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md). Consequently,

$$
\int_\Omega f\,d\mu
=\int_{B^c}h\,d\rho=\nu(B^c)\le\nu(\Omega)<\infty,
$$

and, for every $A$,

$$
\int_A f\,d\mu=\nu(A\setminus B).
$$

Hence

$$
\boxed{\nu(A)=\int_Af\,d\mu+\nu(A\cap B),\qquad f\ge0,\quad f\in L^1(\mu),\quad\mu(B)=0.}
$$

This proves [Lebesgue decomposition from a sum-measure density](../../../../../lebesgue-decomposition-from-a-sum-measure-density.md). The argument includes the cases of zero [measures](../../../../../measure.md); there is no division on $B$, where the denominator vanishes.

[Absolute continuity of measures](../../../../../absolute-continuity-of-measures.md), written $\nu\ll\mu$, means that $\mu(A)=0$ implies $\nu(A)=0$ for every $A\in\Sigma$. If $\nu\ll\mu$, then $\nu(B)=0$ in the construction above, so the singular term vanishes. Conversely, if $\nu(A)=\int_Af\,d\mu$ with a nonnegative [integrable](../../../../../integrability.md) $f$, that integral is zero on every $\mu$-[null set](../../../../../null-set.md). Thus

$$
\boxed{\nu\ll\mu\iff \nu(A)=\int_Af\,d\mu
\text{ for some nonnegative }f\in L^1(\mu).}
$$

This is the finite-[measure](../../../../../measure.md) [Radon-Nikodym theorem](../../../../../radon-nikodym-theorem.md) as a consequence of the proved construction.

Finally restrict the base [measure](../../../../../measure.md) to the sub-[sigma-algebra](../../../../../sigma-algebra.md) $\Sigma_0$. For a real $f\in L^1(\mu)$, write $f=f^+-f^-$, with both parts nonnegative and [integrable](../../../../../integrability.md). On $\Sigma_0$ define finite [positive measures](../../../../../positive-measure.md)

$$
\nu_\pm(A)=\int_A f^\pm\,d\mu.
$$

They are [absolutely continuous with respect to](../../../../../absolute-continuity-of-measures.md) $\mu|_{\Sigma_0}$. The result just proved gives nonnegative, $\Sigma_0$-measurable densities $g_\pm$ satisfying

$$
\int_Ag_\pm\,d\mu=\int_Af^\pm\,d\mu\qquad(A\in\Sigma_0).
$$

Set $f_0=g_+-g_-$. Since $\int(g_++g_-)\,d\mu=\int|f|\,d\mu<\infty$, this is in $L^1(\Omega,\Sigma_0,\mu)$, and subtraction gives

$$
\boxed{\int_Af_0\,d\mu=\int_Af\,d\mu\qquad(A\in\Sigma_0).}
$$

For complex $f$, apply the real construction separately to its real and imaginary parts and combine the two results. This is [conditional expectation from finite-measure densities](../../../../../conditional-expectation-from-finite-measure-densities.md). The resulting [conditional expectation](../../../../../conditional-expectation.md) is unique almost everywhere: for two real versions, their difference has integral zero on its positive and negative level sets in $\Sigma_0$, forcing it to vanish; apply this to both components in the complex case. No probability normalization of $\mu$ is required.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
