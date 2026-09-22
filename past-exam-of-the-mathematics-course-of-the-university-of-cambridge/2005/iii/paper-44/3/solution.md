<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use $F(t)=\Pr(T>t)$, a nonincreasing right-continuous [survivor function](../../../../../survival-function.md). The [empirical likelihood](../../../../../empirical-likelihood.md) treats an exact event as a probability mass rather than maximizing an unrestricted [probability density function](../../../../../probability-density-function.md) at isolated data points. Under a noninformative observation mechanism, the event-time [likelihood contributions](../../../../../likelihood-contribution.md) are

$$
\begin{array}{c|c}
\text{observed information}&\text{likelihood contribution}\\\hline
T=s&F(s-)-F(s)\\
T>c&F(c)\\
T\leq c&1-F(c)\\
\ell<T\leq r&F(\ell)-F(r)
\end{array}
$$

The second, third and fourth rows account for [right censoring](../../../../../right-censoring.md), [left censoring](../../../../../left-censoring.md) and [interval censoring](../../../../../interval-censoring.md), respectively. A censoring mechanism with unknown dependence on $T$ cannot simply be dropped; these are the event-time factors under [independent censoring](../../../../../independent-censoring.md) or another ignorable mechanism.

There is a useful finite-dimensional reduction before optimization. Let $A_i$ be the set in which observation $i$ tells us its event time lies. Partition the time axis using all observed endpoints, keeping endpoint singletons when required. Within each cell, membership in every $A_i$ is constant. Assign cell masses $w_j\geq0$, with $\sum_jw_j=1$, including a tail cell when necessary, and let $A_{ij}$ be the cell-membership indicator. Then

$$
L(w)=\prod_i\left(\sum_jA_{ij}w_j\right),\qquad
\ell(w)=\sum_i\log\left(\sum_jA_{ij}w_j\right).
$$

Mass locations within a cell are not identifiable and need not be separate parameters. Repeated observation sets can be grouped and their factors raised to their counts. Cells with the same membership column can also be combined. If one column is componentwise dominated by another, transferring its mass to the dominating column weakly increases every factor; hence an unconstrained maximizing distribution can omit the dominated cell. This proves [likelihood support reduction under censoring](../../../../../likelihood-support-reduction-under-censoring.md) directly. The remaining [log-likelihood](../../../../../log-likelihood.md) is a [concave function](../../../../../concave-function.md) of the probability masses on a simplex, often far smaller than the original unrestricted distribution problem. Added constraints can restrict which transfers remain permissible.

For [right censoring](../../../../../right-censoring.md) alone, take a grid of all distinct observation times $s_j$ and initially allow a [discrete hazard](../../../../../discrete-hazard.md)

$$
q_j=\Pr(T=s_j\mid T\geq s_j).
$$

Let $d_j$ be the number of events at $s_j$ and $n_j=\#\{i:x_i\geq s_j\}$ the [risk set](../../../../../risk-set.md) immediately before that time. For tied recorded times, use the convention that events precede censoring, so those censored at $s_j$ remain in this [risk set](../../../../../risk-set.md). The mass at $s_j$ is $q_j\prod_{k<j}(1-q_k)$, and the probability of surviving past $s_j$ is $\prod_{k\leq j}(1-q_k)$. Substitution into the exact-event and right-censoring factors yields

$$
L(q)=\prod_j q_j^{d_j}(1-q_j)^{n_j-d_j},\qquad
\ell(q)=\sum_j\{d_j\log q_j+(n_j-d_j)\log(1-q_j)\}.
$$

The exponent $n_j-d_j$ counts all observed individuals whose information requires survival beyond that jump. In particular, censoring observations affect the [risk set](../../../../../risk-set.md) even though they give no event factor.

Each factor can now be maximized separately. For $0<d_j<n_j$, its derivative is $d_j/q_j-(n_j-d_j)/(1-q_j)$, giving $\widehat q_j=d_j/n_j$; the second derivative is negative. The same result holds at the boundaries: $\widehat q_j=0$ if $d_j=0$, and $\widehat q_j=1$ if $d_j=n_j$. The [Kaplan–Meier estimator](../../../../../kaplan-meier-estimator.md) is therefore

$$
\boxed{\widehat F(u)=\prod_{s_j\leq u}\left(1-\frac{d_j}{n_j}\right).}
$$

Only event times contribute nontrivial factors. Residual mass after the last observation may be placed anywhere later without changing the [empirical likelihood](../../../../../empirical-likelihood.md). A terminal plateau is therefore not evidence of permanent survival; the tail is unobserved.

For a [constrained Kaplan–Meier estimator](../../../../../constrained-kaplan-meier-estimator.md) with $F(t)=p$, first split the support cells at $t$. In the probability-mass representation the exact optimization problem is

$$
\max_{w_j\geq0}\ \ell(w),\qquad
\sum_jw_j=1,\qquad\sum_{\text{cells above }t}w_j=p.
$$

The last sum excludes a singleton mass at $t$, because $F(t)=\Pr(T>t)$. This is a concave maximization with linear equality constraints, so it directly gives a constrained [nonparametric maximum-likelihood estimator](../../../../../nonparametric-maximum-likelihood-estimator.md). It also handles a time lying between observed events or beyond all follow-up.

An equivalent hazard formulation adds $t$ to the grid, permits zero-event jumps when needed, and imposes

$$
\prod_{s_j\leq t}(1-q_j)=p.
$$

For an interior solution using only positive-event jumps before $t$, add $\lambda\{\sum_{s_j\leq t}\log(1-q_j)-\log p\}$ to the [log-likelihood](../../../../../log-likelihood.md). Differentiating gives

$$
\widehat q_j=\frac{d_j}{n_j+\lambda}\quad(s_j\leq t),\qquad
\widehat q_j=\frac{d_j}{n_j}\quad(s_j>t).
$$

The multiplier is found by solving the scalar equation

$$
\prod_{s_j\leq t}\frac{n_j-d_j+\lambda}{n_j+\lambda}=p,
$$

with denominators and fitted hazards in their admissible ranges. On an admissible event-only interior branch, this product is increasing in $\lambda$, making a one-dimensional root search straightforward.

**A constraint can require mass at a time with no observed event.** The event-only multiplier equation must not be used blindly. To include boundary cases, put $u_j=-\log(1-q_j)\geq0$. Before $t$, the constraint becomes $\sum_j u_j=-\log p$, and each contribution is

$$
d_j\log(1-e^{-u_j})-(n_j-d_j)u_j.
$$

For $d_j>0$ its multiplier equation again gives $q_j=d_j/(n_j+\lambda)$. For $d_j=0$, its derivative is $-n_j$, so the maximum has $u_j=0$ when $\lambda>-n_j$, and may have $u_j>0$ when $\lambda=-n_j$. Such a jump supplies mass needed by the constraint; an unobserved tail with $n_j=0$ is included by the same rule. For example, if every observation is right-censored after $t$ and there are no events, the ordinary estimate has $F(t)=1$. To impose $p<1$, put mass $1-p$ at $t$ and the remaining $p$ after all censoring times. The maximized likelihood is $p^n$, although there are no event-time factors at all. The mass-constrained optimization above automatically accounts for this possibility and for any remaining tail nonuniqueness.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
