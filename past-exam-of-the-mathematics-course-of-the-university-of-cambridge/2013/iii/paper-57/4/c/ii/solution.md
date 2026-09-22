<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $g_*>0$ for the upper endpoint called $a$ in the question, to distinguish it from the device amplitude. For a single realization of a finite bath,

$$
z_N(t)=\prod_{k=1}^N\cos(2g_kt).
$$

**The literal claim of convergence to zero as time tends to infinity is false for every fixed finite $N$.** [Random-coupling spin-bath decoherence](../../../../../../../random-coupling-spin-bath-decoherence.md) must distinguish individual realizations, ensemble averages and the large-bath limit.

First establish [finite spin-bath coherence recurrence](../../../../../../../finite-spin-bath-coherence-recurrence.md) without assuming commensurate couplings. Fix a reference time $t_0>0$ and consider $Q^N+1$ points with coordinates $j g_k t_0/\pi$ modulo $1$, for $0\leq j\leq Q^N$. Partition the unit cube into $Q^N$ smaller cubes of side $1/Q$. Two points share a cube, so their difference provides an integer $1\leq q\leq Q^N$ with

$$
\operatorname{dist}(q g_k t_0/\pi,\mathbb Z)<1/Q\quad\text{for all }k.
$$

At time $q t_0$ every cosine is arbitrarily close to $1$. As $Q$ increases, either these $q$ have an unbounded subsequence, or a bounded subsequence supplies a fixed $q$ with all distances exactly zero; its arbitrarily large multiples are then exact recurrences. In both cases there are unbounded times $t_j$ such that $z_N(t_j)\to1$. This is the simultaneous [Dirichlet approximation theorem](../../../../../../../dirichlet-s-approximation-theorem.md) argument; it applies equally to typical irrational random couplings. Part (i) supplies a particularly simple exact periodic counterexample.

The intended suppression is valid after ensemble averaging. Independence and the uniform density give the [ensemble spin-bath coherence](../../../../../../../ensemble-spin-bath-coherence.md)

$$
\boxed{\mathbb E z_N(t)=\left[\frac1{g_*}\int_0^{g_*}\cos(2gt)\,dg\right]^N
=\left[\frac{\sin(2g_*t)}{2g_*t}\right]^N}.
$$

The continuous value at $t=0$ is $1$. For $t\ne0$ its magnitude is strictly below $1$ to the power $N$, and for fixed $N$ it has an envelope of order $(2g_*t)^{-N}$ as $t\to\infty$. Thus **the ensemble mean tends to zero with time**.

The mean square distinguishes actual loss of coherence from cancellation of signs in that mean:

$$
\boxed{\mathbb E|z_N(t)|^2=\left[\frac12+\frac{\sin(4g_*t)}{8g_*t}\right]^N}.
$$

At long times this tends to $2^{-N}$, exponentially small for $N\gg1$, rather than exactly zero for a finite bath. At any fixed $t\ne0$, the bracket $q(t)$ is strictly less than $1$, since $\cos^2(2gt)<1$ on a set of positive measure. The [Markov inequality](../../../../../../../markov-inequality.md) then gives

$$
P(|z_N(t)|>\varepsilon)\leq\varepsilon^{-2}q(t)^N\longrightarrow0\quad(N\to\infty).
$$

This proves small coherence for typical large baths at a fixed nonzero time. An even stronger fixed-time formulation uses the [strong law of large numbers](../../../../../../../strong-law-of-large-numbers.md):

$$
\frac1N\log|z_N(t)|\longrightarrow\frac1{g_*}\int_0^{g_*}\log|\cos(2gt)|\,dg<0
\quad\text{almost surely}.
$$

The logarithmic singularities at isolated cosine zeros are integrable, and an exact zero has probability zero, so the law applies. Typical coherence consequently decreases exponentially with bath size.

The initial time scale is also explicit. When $g_*|t|\ll1$, $\log\cos(2g_kt)=-2g_k^2t^2+O(g_k^4t^4)$, so the [short-time Gaussian spin-bath decoherence](../../../../../../../short-time-gaussian-spin-bath-decoherence.md) approximation is

$$
z_N(t)=\exp\left[-2t^2\sum_k g_k^2+O(Ng_*^4t^4)\right]
\simeq\boxed{\exp\left[-\frac23Ng_*^2t^2\right]}.
$$

Here $N^{-1}\sum g_k^2\to g_*^2/3$; on the scale $t\sim(g_*\sqrt N)^{-1}$ the displayed remainder tends to zero. The coherence is therefore rapidly suppressed for a large bath and is usually tiny at later fixed times, while rare recurrences still prevent a finite-realization long-time zero limit. **Ensemble decay or a specified large-$N$ limit is the correct qualification of the printed assertion**, consistent with reversible global [unitary time evolution](../../../../../../../unitary-time-evolution.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 57](../../../../paper-57-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
