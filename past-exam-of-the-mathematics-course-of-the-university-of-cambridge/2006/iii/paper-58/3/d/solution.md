<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Continue with equal prior probabilities as in part (c). The two [Bloch vectors](../../../../../../bloch-vector.md) are

$$
r=(\sin\theta\cos\varphi,\sin\theta\sin\varphi,\cos\theta),\qquad
s=(-\sin\theta\cos\varphi,\sin\theta\sin\varphi,\cos\theta).
$$

Their density-matrix difference is $\Delta=\sin\theta\cos\varphi\,\sigma_x$. If a binary measurement effect $E$ declares the first state, its success is

$$
p=\tfrac12\operatorname{Tr}(E\rho_r)+\tfrac12\operatorname{Tr}[(I-E)\rho_s]
=\tfrac12+\tfrac12\operatorname{Tr}(E\Delta).
$$

Diagonalize $\Delta$. Because $0\le E\le I$, the [trace](../../../../../../matrix-trace.md) is maximized by taking $E$ to be its positive-eigenvalue projector. Thus perform a [Pauli measurement](../../../../../../measurement-of-a-pauli-observable.md) of $\sigma_x$, equivalently measure in $(|0\rangle\pm|1\rangle)/\sqrt2$. If $\cos\varphi>0$, identify the first state on the positive outcome and the second on the negative; reverse the labels if $\cos\varphi<0$. The optimum is

$$
\boxed{p_{\mathrm{correct}}=\frac{1+\sin\theta|\cos\varphi|}{2}.}
$$

For $\cos\varphi=0$ the states coincide, so the best probability is $1/2$. This explicit positive-eigenspace optimization proves the [Helstrom measurement for two pure states](../../../../../../helstrom-measurement-for-two-pure-states.md) result in the present case, rather than only quoting its name.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
