<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the standard [right censoring](../../../../../right-censoring.md) setup with everyone entering observation at time zero. At each observed time $x_j$, the pre-exit [risk set](../../../../../risk-set.md) has size $r_j=\#\{i:x_i\geq x_j\}$. The [Nelson–Aalen estimator](../../../../../nelson-aalen-estimator.md) of the [cumulative hazard function](../../../../../cumulative-hazard-function.md) is

$$
\boxed{\widehat H(t)=\sum_{j:x_j\leq t}\frac{v_j}{r_j}.}
$$

Censoring removes an individual from later risk sets but contributes no event increment.

Exchange the two finite sums:

$$
\sum_i\widehat H(x_i)=\sum_i\sum_{j:x_j\leq x_i}\frac{v_j}{r_j}=\sum_j\frac{v_j}{r_j}\#\{i:x_i\geq x_j\}=\sum_jv_j=d.
$$

Each event increment appears in exactly as many subjects' fitted cumulative hazards as there were subjects at risk for that increment. This proves the [event-count identity for Nelson–Aalen cumulative hazards](../../../../../event-count-identity-for-nelson-aalen-cumulative-hazards.md). Common entry is relevant: with delayed entry, a subject does not accumulate the increments before entering, so an entry-time subtraction would be needed.

One method for ties is to **group observations at each distinct recorded time**. If $d_k$ events occur at $\tau_k$, use the pre-time [risk set](../../../../../risk-set.md) size $R_k$ including observations censored at that same recorded time, and take one jump $d_k/R_k$. This is the usual events-before-censoring convention within a recorded tie. Since $R_k=\#\{i:x_i\geq\tau_k\}$,

$$
\sum_i\widehat H(x_i)=\sum_k\frac{d_k}{R_k}\#\{i:x_i\geq\tau_k\}=\sum_kd_k.
$$

Thus the [grouped Nelson–Aalen event-count identity](../../../../../grouped-nelson-aalen-event-count-identity.md) **preserves the required identity at the recorded observation times**. It is a sum over individuals, not an unweighted sum over distinct times.

A second method, suitable when ties reflect rounded times, is to **break ties by small perturbations or an artificial ordering**, then apply the untied estimator. The event-count identity holds on that new, untied time grid. It does not generally persist if all estimates are mapped back to the original common time. For example, two tied failures among two individuals give a grouped jump $2/2=1$, so the original-time sum is $2$. Sequentially breaking the failures gives jumps $1/2$ and $1$, whose total is $3/2$; assigning the completed jump to both original tied observations gives sum $3$. On the perturbed grid the two values are $1/2$ and $3/2$, whose sum is again $2$. This distinction states exactly what the second method does and does not preserve.

Another common grouped survival approach is the [Kaplan–Meier estimator](../../../../../kaplan-meier-estimator.md), from which one may estimate cumulative hazard by $-\log\widehat S(t)$. Its jump is $-\log(1-d_k/R_k)$, not $d_k/R_k$, and it likewise does not have the Nelson–Aalen event-count identity. In particular it becomes infinite at a time when all remaining individuals fail.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
