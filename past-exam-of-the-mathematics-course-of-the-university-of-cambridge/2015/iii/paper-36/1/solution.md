<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $p=dP/d\mu$ and $q=dQ/d\mu$. Using natural [logarithms](../../../../../logarithm.md), the [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) is

$$
\boxed{K(P,Q)=\int_\Omega p\log\frac pq\,d\mu.}
$$

The integrand is zero where $p=0$, including where both densities vanish, and is $+\infty$ where $p>0=q$. Equivalently, $K(P,Q)=\int\log(dP/dQ)\,dP$ when $P$ is [absolutely continuous with respect to](../../../../../absolute-continuity-of-measures.md) $Q$, and it is $+\infty$ otherwise. This is a well-defined extended integral: on $p<q$, writing $t=p/q$ gives $-p\log(p/q)=-qt\log t\leq q/e$, so its negative part is integrable.

For [Pinsker's inequality](../../../../../pinsker-s-inequality.md), an infinite [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) makes the conclusion immediate. Assume it is finite. Set

$$
A=\{p\geq q\},\qquad a=P(A),\quad b=Q(A),\quad t=a-b.
$$

Since $\int(p-q)\,d\mu=0$, the positive and negative parts of $p-q$ have equal integrals. Thus

$$
\int|p-q|\,d\mu=2t,\qquad t\geq0.
$$

This $t$ is the [total variation distance](../../../../../total-variation-distance.md) with the convention $\sup_E|P(E)-Q(E)|$.

We first prove the [binary partition bound for relative entropy](../../../../../binary-partition-bound-for-relative-entropy.md). For any measurable $E$ with $Q(E)>0$, apply [Jensen inequality](../../../../../jensen-s-inequality.md) to the [convex function](../../../../../convex-function.md) $u\mapsto u\log u$ under the conditional [probability measure](../../../../../probability-measure.md) $Q(\cdot\mid E)$. [Absolute continuity of measures](../../../../../absolute-continuity-of-measures.md) gives

$$
\int_E p\log\frac pq\,d\mu\geq P(E)\log\frac{P(E)}{Q(E)}.
$$

If $P(E)=0$, both sides are zero; if $Q(E)=0$, finiteness forces $P(E)=0$ as well. Apply this bound to $A$ and its complement to obtain

$$
K(P,Q)\geq d(a,b):=a\log\frac ab+(1-a)\log\frac{1-a}{1-b}.
$$

For $0<b<1$, regarding $d(a,b)$ as a [function](../../../../../function-split.md) of $a$ gives

$$
d(b,b)=0,\qquad \partial_a d(b,b)=0,\qquad \partial_a^2d(a,b)=\frac1{a(1-a)}\geq4.
$$

Consequently $d(a,b)-2(a-b)^2$ is a [convex function](../../../../../convex-function.md) and has its minimum zero at $a=b$. By continuity this also holds at $a=0,1$. For $b=0,1$, the finite case has $a=b$ and the remaining cases have infinite divergence. This proves the [Bernoulli relative entropy lower bound](../../../../../bernoulli-relative-entropy-lower-bound.md) in every case. Combining the bounds yields

$$
K(P,Q)\geq2t^2=\frac12\left(\int|p-q|\,d\mu\right)^2,\qquad\boxed{\int|p-q|\,d\mu\leq\sqrt{2K(P,Q)}.}
$$

For the [Hellinger distance](../../../../../hellinger-distance.md), retain the unnormalized convention in which

$$
H^2(P,Q)=2-2\int\sqrt{pq}\,d\mu.
$$

The integral is the [Hellinger affinity](../../../../../hellinger-affinity.md). In the finite-divergence case, $q/p>0$ for $P$-almost every point. Apply $-\log u\geq1-u$ with $u=\sqrt{q/p}$ to get

$$
\begin{aligned}
K(P,Q)&=\int_{\{p>0\}}-2\log\sqrt{q/p}\,p\,d\mu\\
&\geq2\int_{\{p>0\}}(1-\sqrt{q/p})p\,d\mu\\
&=2-2\int\sqrt{pq}\,d\mu=H^2(P,Q).
\end{aligned}
$$

The affinity is finite by [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). Mass of $Q$ on $\{p=0\}$ creates no difficulty, since the affinity vanishes there and both [probability measures](../../../../../probability-measure.md) have mass one. The infinite-divergence case is again immediate. We obtain the [relative entropy bound for the unnormalized Hellinger distance](../../../../../relative-entropy-bound-for-the-unnormalized-hellinger-distance.md):

$$
\boxed{H(P,Q)\leq\sqrt{K(P,Q)}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 36](../../paper-36-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
