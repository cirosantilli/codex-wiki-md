<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $N_m=|B(m)|$ and $\theta=\theta(p)>0$. By translation invariance and [linearity of expectation](../../../../../../linearity-of-expectation.md),

$$
\mathbb E_pR(m)=\sum_{x\in B(m)}\mathbb P_p(x\text{ belongs to the infinite cluster})=\theta N_m.
$$

Let $r=\mathbb P_p(R(m)\geq\theta N_m/2)$. Since $0\leq R(m)\leq N_m$, splitting the [expectation](../../../../../../expected-value.md) at the threshold gives

$$
\theta N_m\leq\frac{\theta N_m}{2}(1-r)+N_mr.
$$

Rearranging produces the slightly stronger estimate

$$
\boxed{\mathbb P_p\left(R(m)\geq\frac{\theta(p)|B(m)|}{2}\right)\geq\frac{\theta(p)}{2-\theta(p)}\geq\frac{\theta(p)}2.}
$$

Only the mean and boundedness of the [random variable](../../../../../../random-variable-split.md) are used; independence of the vertex-membership events is unnecessary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
