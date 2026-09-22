<h1 id="15a/solution">Solution</h1>

↑ **Parent:** [15A](../15a.md)

A [stationary state](../../../../../stationary-state.md) has the form

$$
\Psi(t)=e^{-iEt/\hbar}\psi.
$$

For a time-independent [quantum observable](../../../../../observable.md) $Q$, the global phases cancel in the [expectation value](../../../../../expectation-value.md):

$$
\langle Q\rangle_{\Psi(t)}
=\langle e^{-iEt/\hbar}\psi,Qe^{-iEt/\hbar}\psi\rangle
=\langle\psi,Q\psi\rangle.
$$

It is therefore independent of time.

For the [infinite square well](../../../../../infinite-square-well.md),

$$
E_n=\frac{n^2\pi^2\hbar^2}{2ma^2}.
$$

The possible [energy measurement](../../../../../energy-measurement.md) results are

$$
\boxed{E_1=\frac{\pi^2\hbar^2}{2ma^2},
\qquad E_2=\frac{2\pi^2\hbar^2}{ma^2}},
$$

with respective [Born rule](../../../../../born-rule.md) probabilities $|c_1|^2$ and $|c_2|^2$. Normalization gives $|c_1|^2+|c_2|^2=1$.

At time $t$,

$$
\Psi(x,t)=c_1e^{-iE_1t/\hbar}\psi_1(x)
+c_2e^{-iE_2t/\hbar}\psi_2(x).
$$

The required [matrix elements](../../../../../matrix-element.md) are

$$
\langle\psi_1,\hat x\psi_1\rangle
=\langle\psi_2,\hat x\psi_2\rangle=\frac a2,
\qquad
\langle\psi_1,\hat x\psi_2\rangle=-\frac{16a}{9\pi^2}.
$$

Consequently

$$
\boxed{\langle\hat x\rangle_{\Psi(t)}
=\frac a2-\frac{32a}{9\pi^2}
\operatorname{Re}\!\left(c_1^*c_2e^{-i\omega t}\right)},
$$

where the [angular frequency](../../../../../angular-frequency.md) is

$$
\boxed{\omega=\frac{E_2-E_1}{\hbar}
=\frac{3\pi^2\hbar}{2ma^2}}.
$$

Finally, $2|c_1c_2|\le |c_1|^2+|c_2|^2=1$, so

$$
\boxed{\left|\langle\hat x\rangle_{\Psi(t)}-\frac a2\right|
\le\frac{16a}{9\pi^2}}.
$$

## ↑ Ancestors (10)

1. [15A](../15a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
