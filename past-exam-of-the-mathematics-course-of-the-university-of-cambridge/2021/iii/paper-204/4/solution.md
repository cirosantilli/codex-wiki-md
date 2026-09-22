<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [contact process](../../../../../contact-process.md) on $\mathbb Z$ has states $\xi_t(x)\in\{0,1\}$. Each infected site recovers at rate $\mu$, and infection passes across each oriented nearest-neighbour edge at rate $\lambda$. For the [graphical representation of the contact process](../../../../../graphical-representation-of-the-contact-process.md), put independent rate-$\mu$ recovery marks on each vertical time line and independent rate-$\lambda$ infection arrows on each oriented nearest-neighbour edge. Then $y\in\xi_t^A$ exactly when a forward path from some $(x,0)$ with $x\in A$ reaches $(y,t)$ by moving upward, following arrows, and avoiding recovery marks.

If $A\subseteq B$, every path starting in $A$ also starts in $B$, so $\xi_t^A\subseteq\xi_t^B$. A path starts in $A\cup B$ exactly when it starts in one of the two sets, which proves [additivity of the contact process](../../../../../additivity-of-the-contact-process.md):

$$
\xi_t^{A\cup B}=\xi_t^A\cup\xi_t^B.
$$

The event $\xi_t^A\cap B\ne\varnothing$ says that a graphical path runs from $A\times\{0\}$ to $B\times\{t\}$. Reflecting the time interval about $t/2$ and reversing every arrow preserves the joint law of the independent Poisson processes, and the path now runs from $B$ to $A$. This proves [duality of the contact process](../../../../../duality-of-the-contact-process.md):

$$
\mathbb P_{\lambda,\mu}(\xi_t^A\cap B\ne\varnothing)
=\mathbb P_{\lambda,\mu}(\xi_t^B\cap A\ne\varnothing).
$$

The [survival probability of the contact process](../../../../../survival-probability-of-the-contact-process.md) is

$$
\theta(\lambda,\mu)=\mathbb P_{\lambda,\mu}(\xi_t^{\{0\}}\ne\varnothing\text{ for every }t\geq0),
$$

and $\lambda_c(\mu)=\inf\{\lambda:\theta(\lambda,\mu)>0\}$. By duality and translation invariance,

$$
\mathbb P_{\lambda,\mu}(\xi_t^{\mathbb Z}(x)=1)
=\mathbb P_{\lambda,\mu}(\xi_t^{\{x\}}\ne\varnothing)
=\mathbb P_{\lambda,\mu}(\xi_t^{\{0\}}\ne\varnothing).
$$

The events on the right decrease with $t$ because the empty state is absorbing, and their intersection is eternal survival. Therefore

$$
\boxed{\theta(\lambda,\mu)=\lim_{t\to\infty}\mathbb P_{\lambda,\mu}(\xi_t^{\mathbb Z}(x)=1)}.
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 204](../../paper-204-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
