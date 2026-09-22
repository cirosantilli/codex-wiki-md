# Information projection on three outcomes

↑ **Parent:** [Information projection](information-projection.md)

Let the possible numerical outcomes be $-1,0,1$, and give the reference law $p$ [uniform distribution on a finite set](discrete-uniform-distribution.md): $p=(1/3,1/3,1/3)$. We want a law $q$ with [expected value](expected-value.md) $1/2$. Write the three [probabilities](probability.md) in outcome order as $(q_-,q_0,q_+)$. The [mean](expected-value.md) constraint is $q_+-q_-=1/2$, while normalization requires $q_-+q_0+q_+=1$.

These conditions leave a whole line of possible [probability distributions](probability-distribution.md):

$$
q=(x,1/2-2x,1/2+x),\qquad 0\leq x\leq1/4.
$$

For example, $(0,1/2,1/2)$ and $(1/4,0,3/4)$ both have the required [mean](expected-value.md). The constraint alone does not choose between them. [Information projection](information-projection.md) selects the point on this line with the smallest [relative entropy](kullback-leibler-divergence.md) from the reference.

[Exponential tilting](exponential-tilting.md) gives weights proportional to $e^{-\theta},1,e^\theta$. Set $t=e^\theta>0$ and multiply these weights by $t$ to obtain $q^*=(1,t,t^2)/(1+t+t^2)$. Enforcing the [mean](expected-value.md) gives

$$
\frac{t^2-1}{1+t+t^2}=\frac12
\quad\Longleftrightarrow\quad t^2-t-3=0.
$$

The positive root is $t=(1+\sqrt{13})/2$, hence

$$
\boxed{q^*\approx(0.116204,0.267592,0.616204),\qquad
D(q^*\Vert p)\approx0.197378\text{ nats}.}
$$

The most favored outcome becomes $1$, but all three remain possible. This is an exact constructed example with a stipulated reference law and constraint, not a fitted distribution from measurements.

<a id="image-a-mean-constraint-selects-the-least-divergent-law-in-a-probability-simplex"></a>
![](information-projection-probability-simplex.png)

**[Figure 15](#image-a-mean-constraint-selects-the-least-divergent-law-in-a-probability-simplex). A mean constraint selects the least-divergent law in a probability simplex**. Each point represents a [probability distribution](probability-distribution.md) on $\{-1,0,1\}$. The color is [relative entropy](kullback-leibler-divergence.md) from the uniform reference, in [nats](nat-unit.md). The green segment fixes [expected value](expected-value.md) $1/2$, and its marked point is the exact [information projection on three outcomes](information-projection-on-three-outcomes.md). The diagram is calculated from the stated model.

**Table of contents**

- [Information projection and Euclidean projection](information-projection-and-euclidean-projection.md)

## ↑ Ancestors (8)

1. [Information projection](information-projection.md)
2. [Method of types](method-of-types.md)
3. [Type (information theory)](type-information-theory.md)
4. [Information theory](information-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Information projection and rare sample means](information-projection-and-rare-sample-means.md)
- [Information projection on three outcomes](information-projection-on-three-outcomes.md)
