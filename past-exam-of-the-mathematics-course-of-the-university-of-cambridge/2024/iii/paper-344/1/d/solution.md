<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose the translationally invariant [Gaussian variational approximation](../../../../../../gaussian-variational-approximation.md)

$$
H_0=\sum_{\mathbf q}^{+}J(q)|\phi_{\mathbf q}|^2,
\qquad J(q)>0.
$$

The superscript $+$ means that one member of each pair $\{\mathbf q,-\mathbf q\}$ is included; this is necessary because a real field obeys $\phi_{-\mathbf q}=\phi_{\mathbf q}^*$. The constrained zero mode is omitted.

For each independent complex mode,

$$
\int_{\mathbb R^2}d(\operatorname{Re}\phi_{\mathbf q})\,d(\operatorname{Im}\phi_{\mathbf q})
e^{-J(q)|\phi_{\mathbf q}|^2}
=\frac{\pi}{J(q)}.
$$

Consequently,

$$
F_0=\sum_{\mathbf q}^{+}\log\frac{J(q)}{\pi},
\qquad
\langle H_0\rangle_0=\sum_{\mathbf q}^{+}1,
\qquad
\left\langle\sum_{\mathbf q}^{+}G(q)|\phi_{\mathbf q}|^2\right\rangle_0
=\sum_{\mathbf q}^{+}\frac{G(q)}{J(q)}.
$$

Substitution into the [Gibbs--Bogoliubov--Feynman inequality](../../../../../../gibbs-bogoliubov-feynman-inequality.md) gives

$$
\widetilde F
=\sum_{\mathbf q}^{+}
\left[
\log\frac{J(q)}{\pi}-1+\frac{G(q)}{J(q)}
\right]
+g\int d^d\mathbf r\,\langle|\phi(\mathbf r)|^3\rangle_0,
$$

which is the required upper bound.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
