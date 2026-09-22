<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For an invertible probability [measure-preserving system](../../../../../measure-preserving-system.md), an [almost periodic observable](../../../../../almost-periodic-observable.md) is an $f\in L^2(\mu)$ whose [Koopman operator](../../../../../koopman-operator.md) orbit is [totally bounded](../../../../../totally-bounded-space.md):

$$
\boxed{\{U_T^nf:n\in\mathbb Z\}\text{ is totally bounded in }L^2(\mu).}
$$

Equivalently, for every $\varepsilon>0$ it has a finite $\varepsilon$-net in $L^2$. For a noninvertible system use the forward orbit $n\geq0$.

A [factor map](../../../../../factor-map-between-measure-preserving-systems.md) $\varphi:X\to Y$ satisfies $\varphi_*\mu=\nu$ and $\varphi T=S\varphi$ [almost everywhere](../../../../../almost-everywhere.md). Disintegrate $\mu=\int_Y\mu_y\,d\nu(y)$ over this map and write

$$
\|h\|_y=\left(\int_X|h|^2\,d\mu_y\right)^{1/2}
$$

for the [conditional L2 norm](../../../../../conditional-l2-norm.md). A [relatively almost periodic observable](../../../../../relatively-almost-periodic-observable.md) is an $f\in L^2(\mu)$ such that, for every $\varepsilon>0$, there are finitely many $g_1,\ldots,g_r\in L^2(\mu)$ with

$$
\boxed{\min_{1\leq j\leq r}\|U_T^nf-g_j\|_y<\varepsilon
\quad\text{for all }n\in\mathbb Z,\text{ for }\nu\text{-almost every }y.}
$$

The center may depend on both $n$ and $y$; the finite list itself does not. Since $\mathbb Z$ is countable, the exceptional null sets can be combined. A [compact extension of a measure-preserving system](../../../../../compact-extension-of-a-measure-preserving-system.md) is a [factor map](../../../../../factor-map-between-measure-preserving-systems.md) for which these [relatively almost periodic observables](../../../../../relatively-almost-periodic-observable.md) are dense in $L^2(\mu)$. This density definition should not be replaced by a claim that every $L^2$ observable already satisfies the uniform fiberwise finite-net condition.

For a proper [factor map](../../../../../factor-map-between-measure-preserving-systems.md) example, let $Y=\{-1,1\}^{\mathbb Z}$ carry independent fair coordinates and the two-sided [Bernoulli shift](../../../../../bernoulli-shift.md) $S$, with $(Sy)_j=y_{j+1}$. Set

$$
X=Y\times\{0,1\},\qquad
T(y,i)=(Sy,i+1\pmod2),\qquad \varphi(y,i)=y,
$$

using the product of the Bernoulli measure and the equal two-point measure. These are invertible [measure-preserving systems](../../../../../measure-preserving-system.md), and the projection preserves measure and intertwines the transformations, so it is a two-to-one [factor map](../../../../../factor-map-between-measure-preserving-systems.md).

Take $f(y,i)=y_0$. Then $U_T^nf(y,i)=y_n$. Distinct coordinates are independent and have mean zero and variance one, hence

$$
\boxed{\|U_T^nf-U_T^mf\|_2^2
=\mathbb E[(y_n-y_m)^2]=2\qquad(n\ne m).}
$$

Its orbit has no finite sufficiently small net. Thus **the [Bernoulli coordinate observable is not almost periodic](../../../../../bernoulli-coordinate-observable-is-not-almost-periodic.md) in global $L^2$**. In contrast, the conditional measure over $y$ is the equal measure on $(y,0),(y,1)$, and $U_T^nf$ is constant on that fiber with value $y_n\in\{-1,1\}$. The two centers $g_1=1,g_2=-1$ give zero error on every fiber for every $n$. Therefore **$f$ is a [relatively almost periodic observable](../../../../../relatively-almost-periodic-observable.md) for this map**.

The example is also a [finite-fiber compact extension](../../../../../finite-fiber-compact-extension.md). For a bounded observable on $X$, each orbit value on a fiber is a pair in a fixed bounded subset of $\mathbb C^2$, which has a finite net. Its centers can be chosen as functions constant in $y$, with prescribed values on the two labels. Bounded observables are dense in $L^2$, so the extension is compact. The [Bernoulli shift](../../../../../bernoulli-shift.md) is mixing: cylinder events involving disjoint coordinate sets are independent for all sufficiently large shifts, and approximation by cylinder events extends this to arbitrary events. Thus $S$ and $S^2$ are [ergodic](../../../../../ergodicity.md). If an invariant function on $X$ is written $a(y)+(-1)^ib(y)$, invariance gives $a\circ S=a$ and $b\circ S=-b$. The first function is constant; the second is $S^2$-invariant and hence constant, and then its sign equation forces zero. This proves that the example's source is also [ergodic](../../../../../ergodicity.md).

For the positive-subset assertion, interpret the printed $X'$ as $X$, or as an invariant full-measure domain of the [factor map](../../../../../factor-map-between-measure-preserving-systems.md); the prime is otherwise undefined and does not change the measure-theoretic argument.

First establish [conditional norm covariance under a factor map](../../../../../conditional-norm-covariance-under-a-factor-map.md). Invariance of the measures and uniqueness in the [disintegration theorem for a probability measure](../../../../../disintegration-theorem-for-a-probability-measure.md) give

$$
T_*\mu_y=\mu_{Sy},\qquad
\boxed{\|U_T^nh\|_y=\|h\|_{S^ny}\quad(n\in\mathbb Z)}
$$

on common full-measure sets. For the first equality, $y\mapsto T_*\mu_{S^{-1}y}$ is another disintegration over the same fibers: it is supported on $\varphi^{-1}\{y\}$ and integrates to $\mu$. Uniqueness identifies it with $\mu_y$, and iteration gives the norm formula.

Two elementary facts explain [localization of relative almost periodicity to base sets](../../../../../localization-of-relative-almost-periodicity-to-base-sets.md). If $f$ is a [relatively almost periodic observable](../../../../../relatively-almost-periodic-observable.md) and $C\subseteq Y$ is measurable, then $f\,\mathbf1_C\circ\varphi$ is also [relatively almost periodic](../../../../../relatively-almost-periodic-observable.md). Indeed, on a fiber,

$$
U_T^n\bigl(f\,\mathbf1_C\circ\varphi\bigr)
=(U_T^nf)\mathbf1_C(S^ny).
$$

When that indicator is one, use a center for $U_T^nf$; when it is zero, use the additional center $0$. Secondly, [relative almost periodicity](../../../../../relatively-almost-periodic-observable.md) is closed under convergence in the [uniform conditional L2 norm](../../../../../uniform-conditional-l2-norm.md)

$$
\|h\|_{2,\infty\mid Y}
=\mathop{\mathrm{ess\,sup}}_{y\in Y}\|h\|_y.
$$

If this norm of $f-f_j$ tends to zero, covariance bounds the corresponding error between every pair of orbit values by the same number. A finite $\varepsilon/2$-net for one sufficiently close $f_j$ is consequently an $\varepsilon$-net for $f$.

Now take $f=\mathbf1_A$. The [compact extension](../../../../../compact-extension-of-a-measure-preserving-system.md) supplies [relatively almost periodic observables](../../../../../relatively-almost-periodic-observable.md) $f_j$ with

$$
\|f_j-f\|_2^2\leq2^{-j}.
$$

Put $e_j(y)=\|f_j-f\|_y$. The [Tonelli theorem](../../../../../tonelli-theorem.md) gives

$$
\int_Y\sum_{j=1}^\infty e_j(y)^2\,d\nu(y)
=\sum_{j=1}^\infty\|f_j-f\|_2^2<\infty.
$$

Hence $e_j(y)\to0$ for $\nu$-almost every $y$. Since $\int_Y\mu_y(A)d\nu=\mu(A)>0$, choose $\eta>0$ for which

$$
E=\{y:\mu_y(A)\geq\eta\}
$$

has positive measure. The [Egorov theorem](../../../../../egorov-s-theorem.md) gives a measurable $C\subseteq E$ of positive measure on which $e_j\to0$ uniformly. Define

$$
\boxed{B=A\cap\varphi^{-1}C.}
$$

Then

$$
\boxed{\mu(B)=\int_C\mu_y(A)\,d\nu(y)\geq\eta\nu(C)>0.}
$$

For $h_j=f_j\,\mathbf1_C\circ\varphi$, the localization fact makes every $h_j$ [relatively almost periodic](../../../../../relatively-almost-periodic-observable.md), while

$$
\|h_j-\mathbf1_B\|_{2,\infty\mid Y}
=\mathop{\mathrm{ess\,sup}}_{y\in C}e_j(y)\longrightarrow0.
$$

The conditional-norm closure fact therefore proves **$\mathbf1_B$ is a [relatively almost periodic observable](../../../../../relatively-almost-periodic-observable.md)**, with $B\subseteq A$ and positive measure. This is the [positive-measure almost periodic indicator in a compact extension](../../../../../positive-measure-almost-periodic-indicator-in-a-compact-extension.md). No [ergodic](../../../../../ergodicity.md) component or uncountable intersection of exceptional sets is needed in this construction; it in fact works under the same disintegration and compactness hypotheses without using the assumed [ergodicity](../../../../../ergodicity.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
