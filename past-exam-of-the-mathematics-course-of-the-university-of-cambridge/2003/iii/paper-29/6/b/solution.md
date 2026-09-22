<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $q=b/a>1$. Each successive crossing time $N_j$, $j\geq1$, is a [stopping time](../../../../../../stopping-time.md), since in discrete time the event that a threshold is first met after the previous [stopping time](../../../../../../stopping-time.md) can be written as a finite union of events known at the candidate time. Use $\inf\varnothing=\infty$, with all later crossing times then infinite as well.

For the supermartingale assertion, build a process by finitely many switches. Begin with the constant [supermartingale](../../../../../../supermartingale.md) one. At $N_1$ switch to $X_n/a$; the new value at that time is at most one. At $N_2$ switch to the constant $q$; the old value there is $X_{N_2}/a\geq q$. At $N_3$ switch to $qX_n/a$, whose value is at most $q$, and at $N_4$ switch to the constant $q^2$, whose value is at most the previous process. More generally, the switches at $N_{2\ell-1}$ and $N_{2\ell}$ are respectively from cash $q^{\ell-1}$ to $q^{\ell-1}X_n/a$ and from that stock value to cash $q^\ell$. Every switch is downward, including possible overshoots of either threshold.

Each candidate continuation is a [supermartingale](../../../../../../supermartingale.md), being either constant or a fixed positive multiple of $X$. Part (a) therefore proves by induction that the process $M^{(j)}$ obtained after the first $j$ switches is a [supermartingale](../../../../../../supermartingale.md). It agrees with $Y$ through $N_j$. For fixed $j,n$, its values are bounded in absolute value by a deterministic constant depending on $j$ times $1+X_n$, which also verifies the required [integrability](../../../../../../integrability.md) rather than assuming it for an infinite sequence of pastings.

Stopping a discrete [supermartingale](../../../../../../supermartingale.md) preserves the property. Indeed its stopped increment is $\mathbf1_{\{N_j>n\}}(M^{(j)}_{n+1}-M^{(j)}_n)$, with an $\mathcal F_n$-[measurable](../../../../../../measurability.md) indicator; integrability at any fixed time follows from a finite sum of the absolute values at earlier times. Hence

$$
\boxed{Y_{n\wedge N_j}=M^{(j)}_{n\wedge N_j}\text{ is a nonnegative supermartingale for }j\geq1.}
$$

This is the [multiplicative upcrossing supermartingale](../../../../../../multiplicative-upcrossing-supermartingale.md) construction. The printed $j=0$ case uses $N_0=-1$, while $Y$ was only defined from time zero. With the natural pre-start convention $Y_{-1}=1$, it is the constant process one and the assertion also holds for $j=0$. Without such an extension, that single displayed stopped process is undefined.

For the probability bound, the actual initial value is

$$
Y_0=\min(X_0/a,1),
$$

because $N_1=0$ exactly when $X_0\leq a$. For an integer $k\geq1$, stop after the $k$th completed [upcrossing](../../../../../../upcrossing.md), at $N_{2k}$. The nonnegative stopped [supermartingale](../../../../../../supermartingale.md) satisfies

$$
q^k\mathbb P(N_{2k}\leq n)\leq\mathbb E Y_{n\wedge N_{2k}}\leq\mathbb E Y_0,
$$

since $Y_{N_{2k}}=q^k$ on the event in the left side. Letting $n\to\infty$, and identifying $\{U\geq k\}=\{N_{2k}<\infty\}$, proves the [Dubins upcrossing inequality](../../../../../../dubins-upcrossing-inequality.md):

$$
\boxed{\mathbb P(U\geq k)\leq\left(\frac ab\right)^k\mathbb E\min(X_0/a,1),\qquad k=1,2,\ldots.}
$$

Neither finiteness of $N_{2k}$ nor [uniform integrability](../../../../../../uniform-integrability.md) is needed. The bound is for positive integers $k$; extending it to $k=0$ would generally be false, because its left side would be one while $\mathbb E\min(X_0/a,1)$ can be less than one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
