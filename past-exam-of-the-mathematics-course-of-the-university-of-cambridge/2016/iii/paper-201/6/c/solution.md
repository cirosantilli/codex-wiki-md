<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The printed uniqueness claim omits nondegeneracy of the limit.** The zero process is a [Lévy process](../../../../../../levy-process.md), and every $\alpha>1/2$ yields that limit. We first classify all possibilities under the stated assumptions, then identify the unique nonzero one.

For $t>0$, part (b) gives

$$
\mathbb E e^{i\theta X_t^{(n)}}
=\exp\{-nt(1-\cos(n^{-\alpha}\theta))\},
\qquad
n(1-\cos(n^{-\alpha}\theta))
=\frac{\theta^2}{2}n^{1-2\alpha}(1+o(1))
$$

for each fixed $\theta\ne0$. If $\alpha<1/2$, the characteristic functions tend to zero for every nonzero parameter and remain one at zero. This discontinuous function cannot be the [characteristic function](../../../../../../characteristic-function.md) of a probability law. The [characteristic-function convergence theorem](../../../../../../levy-s-continuity-theorem.md) therefore rules out even one-dimensional [weak convergence of random variables](../../../../../../convergence-in-distribution.md) at a positive time.

For joint convergence, take $0=t_0<t_1<\cdots<t_m$ and write $q_k=\sum_{j=k}^m\theta_j$. [Independent increments](../../../../../../independent-increments.md) give

$$
\mathbb E\exp\left(i\sum_{j=1}^m\theta_jX_{t_j}^{(n)}\right)
=\exp\left\{-n\sum_{k=1}^m(t_k-t_{k-1})\left(1-\cos(n^{-\alpha}q_k)\right)\right\}.
$$

At $\alpha=1/2$, this tends to $\exp\{-\frac12\sum_k(t_k-t_{k-1})q_k^2\}$. These are exactly the joint laws of standard [Brownian motion](../../../../../../brownian-motion-split.md): increments are independent centred normals with variances $t_k-t_{k-1}$. The assumed limiting [Lévy process](../../../../../../levy-process.md) thus has the Brownian law.

For $\alpha>1/2$, the same joint characteristic functions tend to one. Every limiting vector is zero. The càdlàg path convention then makes the limiting process identically zero almost surely: first intersect the zero-value events at rational times, then use right continuity. The complete [scaling classification of a continuous-time symmetric simple random walk](../../../../../../scaling-classification-of-a-continuous-time-symmetric-simple-random-walk.md) is

$$
\boxed{\begin{array}{c|c}
0<\alpha<1/2&\text{no finite-dimensional probability limit}\\
\alpha=1/2&Y\text{ is standard Brownian motion}\\
1/2<\alpha\leq1&Y_t\equiv0.
\end{array}}
$$

In particular, **if a nonzero limiting Lévy process is intended, the unique exponent is $\alpha=1/2$**, and

$$
\boxed{Y_t\sim\mathcal N(0,t),\qquad \mathbb E[Y_sY_t]=\min(s,t).}
$$

The finite-dimensional Brownian law, together with the Lévy càdlàg convention, determines the process law and its continuous version. No assertion of path-space convergence of the approximating walks is needed here.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
