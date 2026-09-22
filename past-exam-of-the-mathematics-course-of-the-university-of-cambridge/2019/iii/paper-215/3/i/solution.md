<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Couple two [noisy voter model](../../../../../../noisy-voter-model.md) chains by choosing the same update vertex, the same refresh coin and refreshed spin, and, for a voter update, the same chosen neighbor. Let $D_t$ be their [Hamming distance](../../../../../../hamming-distance.md). If $G$ is $r$-regular, conditioning on the current disagreement set gives

$$
\begin{aligned}
\mathbb E[D_{t+1}\mid D_t]
&=D_t-\frac{D_t}{n}
+\frac{1-p}{n}\sum_{v\in V}
\frac{|N(v)\cap D_t|}{r}\\
&=\left(1-\frac pn\right)D_t,
\end{aligned}
$$

because every disagreeing vertex is counted in exactly $r$ neighbor sets. Therefore

$$
\mathbb E D_t\leq n\left(1-\frac pn\right)^t.
$$

The [coupling inequality for total variation](../../../../../../coupling-inequality-for-total-variation.md) and $\mathbf1_{\{\sigma_t\ne\sigma_t'\}}\leq D_t$ give

$$
\boxed{\max_{\sigma,\sigma'}
\|P^t(\sigma,\cdot)-P^t(\sigma',\cdot)\|_{\mathrm{TV}}
\leq n\left(1-\frac pn\right)^t.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
