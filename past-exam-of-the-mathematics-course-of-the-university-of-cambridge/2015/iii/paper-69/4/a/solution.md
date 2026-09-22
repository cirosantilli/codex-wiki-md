<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $u^*\in\mathcal U$, $e=f-u^*$, $d=\|e\|_\infty$, and $E=\{x:|e(x)|=d\}$. The real [Kolmogorov criterion for uniform approximation](../../../../../../kolmogorov-criterion-for-uniform-approximation.md) says **$u^*$ is best if and only if**

$$
\boxed{\text{for every }v\in\mathcal U,\quad\min_{x\in E}e(x)v(x)\leq0.}
$$

Equivalently, no direction $v$ has the error's sign strictly at every extremal point. If $d=0$, the criterion is automatic.

For sufficiency, a point with $e(x)v(x)\leq0$ gives $|e(x)-v(x)|\geq d$, so $u^*+v$ cannot improve the norm. For necessity, suppose $e(x)v(x)>0$ on $E$. Compactness gives a positive lower bound there and on a neighbourhood of $E$. On that neighbourhood, $(e-\tau v)^2=e^2-2\tau ev+\tau^2v^2<d^2$ for sufficiently small positive $\tau$. Off the neighbourhood, $|e|$ has a strict gap below $d$, and small $\tau$ preserves that gap. Thus $u^*+\tau v$ has smaller error, a contradiction. This also explains why the criterion involves all active extrema.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
