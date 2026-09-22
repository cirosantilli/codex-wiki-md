<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [intensity function of a point process](../../../../../intensity-function-of-a-point-process.md) is positive and continuous inside the interval, so its [measure](../../../../../measure.md) is finite on every [compact](../../../../../compact-space.md) subinterval. Consequently the [Poisson point process](../../../../../poisson-point-process.md) is locally finite there. Its nonatomic intensity makes it simple and gives no point at $0$ [almost surely](../../../../../almost-sure-convergence.md). At the endpoints,

$$
\lambda(x)\sim\frac{1}{4(1-x)^3}\quad(x\uparrow1),\qquad\lambda(x)\sim\frac{1}{8(1+x)^2}\quad(x\downarrow-1).
$$

Both half-intervals therefore have infinite intensity. More explicitly, exhaust either half by increasing [compact](../../../../../compact-space.md) intervals with means $t_j\to\infty$. For any fixed integer $k$,

$$
\mathbb P\{\#\Pi\text{ in that half}\leq k\}\leq e^{-t_j}\sum_{i=0}^k\frac{t_j^i}{i!}\longrightarrow0.
$$

Taking the [countable](../../../../../countable-set.md) union over $k$ proves **infinitely many points on each side [almost surely](../../../../../almost-sure-convergence.md)**.

Local finiteness excludes accumulation in the interior, including at $0$. Hence there is a largest negative point and a smallest positive point. For example, given any negative point, the [compact](../../../../../compact-space.md) interval between it and $0$ contains finitely many points and therefore a largest one. Call it $X_0$; call the smallest positive point $X_1$, and enumerate consecutively in both directions. Infinite counts give every integer index, and the lack of interior accumulation implies $X_n\uparrow1$ as $n\to\infty$ and $X_n\downarrow-1$ as $n\to-\infty$. Thus the specified two-sided labeling exists [almost surely](../../../../../almost-sure-convergence.md).

Use the cumulative-intensity transformation

$$
\boxed{f(x)=\int_0^x\frac{dt}{(1+t)^2(1-t)^3}.}
$$

It has $f(0)=0$, positive derivative, and limits $-\infty,+\infty$ at the two endpoints, so it is an increasing [bijection](../../../../../bijection.md) onto $\mathbb R$. One explicit expression is

$$
f(x)=\frac{3}{16}\log\frac{1+x}{1-x}-\frac{1}{8(1+x)}+\frac{1}{4(1-x)}+\frac{1}{8(1-x)^2}-\frac14.
$$

For any bounded interval $(a,b)$ in the target, its preimage has intensity

$$
\int_{f^{-1}(a)}^{f^{-1}(b)}\lambda(x)\,dx=b-a.
$$

Disjoint target sets have disjoint preimages, so their counts are [independent](../../../../../independent-random-variables.md). This proves directly, or by the [Poisson mapping theorem](../../../../../poisson-mapping-theorem.md), that the transformed points form a unit-rate [Poisson process](../../../../../poisson-process.md) on the real line.

Put $Y_n=f(X_n)$. On the positive half-line, the successive spacings are [independent](../../../../../independent-random-variables.md) [exponential random variables](../../../../../exponential-distribution.md) of [mean](../../../../../expected-value.md) $1$, so $Y_n=E_1+\cdots+E_n$. The [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) gives $Y_n/n\to1$ [almost surely](../../../../../almost-sure-convergence.md). On the negative half-line, independently, the reflected points satisfy $-Y_{-k}=E'_1+\cdots+E'_{k+1}$, because $Y_0$ is the first point to the left of zero. Thus $-Y_{-k}/k\to1$, or $Y_n/n\to1$ also as $n\to-\infty$. The shift by one has no effect on these limits.

From the explicit formula, or by integrating the endpoint intensity asymptotics,

$$
f(x)(1-x)^2\longrightarrow\frac18\quad(x\uparrow1),\qquad[-f(x)](1+x)\longrightarrow\frac18\quad(x\downarrow-1).
$$

Substitute $x=X_n$ and use the [strong law for Poisson arrival times](../../../../../strong-law-for-poisson-arrival-times.md). At the right endpoint,

$$
n(1-X_n)^2=\frac{n}{f(X_n)}\,f(X_n)(1-X_n)^2\longrightarrow\frac18,
$$

so

$$
\boxed{\sqrt{2n}\,(1-X_n)\longrightarrow\frac12\quad(n\to+\infty),\ \text{almost surely}.}
$$

At the left endpoint the corresponding result is

$$
\boxed{|n|(1+X_n)\longrightarrow\frac18\quad(n\to-\infty),\ \text{almost surely}.}
$$

Equivalently $8|n|(1+X_n)\to1$. The different powers of $|n|$ reflect the different endpoint singularity orders, an instance of [power-law boundary accumulation of a Poisson point process](../../../../../power-law-boundary-accumulation-of-a-poisson-point-process.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
