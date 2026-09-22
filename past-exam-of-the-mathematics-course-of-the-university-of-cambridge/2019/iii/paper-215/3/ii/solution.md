<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a nonregular graph, use the degree-weighted Hamming metric

$$
W_t=\sum_{v\in V}\deg(v)
\mathbf1_{\{\sigma_t(v)\ne\sigma_t'(v)\}}.
$$

Under the same coupling,

$$
\begin{aligned}
\mathbb E[W_{t+1}-W_t\mid\sigma_t,\sigma_t']
={}&-\frac1n\sum_{v\in D_t}\deg(v)\\
&+\frac{1-p}{n}\sum_v\deg(v)
\frac{|N(v)\cap D_t|}{\deg(v)}\\
={}&-\frac pnW_t.
\end{aligned}
$$

Here the final double sum equals $\sum_{u\in D_t}\deg(u)=W_t$. Since $W_0\leq\sum_v\deg(v)=2|E|$ and $W_t\geq1$ whenever the chains differ,

$$
\boxed{\max_{\sigma,\sigma'}
\|P^t(\sigma,\cdot)-P^t(\sigma',\cdot)\|_{\mathrm{TV}}
\leq2|E|\left(1-\frac pn\right)^t.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
