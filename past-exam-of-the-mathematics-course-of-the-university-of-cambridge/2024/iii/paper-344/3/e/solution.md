<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let

$$
t_{\min} =\min(t_2,t_3),
\qquad
t_{\max} =\max(t_2,t_3).
$$

Evolution from the earlier time to the later time multiplies the earlier field by the deterministic decay factor, plus fresh noise independent of that field. The unequal-time [correlation function](../../../../../../correlation-function.md) is therefore

$$
\begin{aligned}
\langle p_{\mathbf q,i}(t_2)p_{-\mathbf q,j}(t_3)\rangle
=\delta_{ij}e^{-r(q)|t_3-t_2|}
\bigg[
&\frac{k_BT}{a_I+\kappa q^2}
e^{-2r(q)(t_{\min}-t_1)}
\\
&+\frac{k_BT}{a_F+\kappa q^2}
\left(1-e^{-2r(q)(t_{\min}-t_1)}\right)
\bigg].
\end{aligned}
$$

Equivalently,

$$
\begin{aligned}
\langle p_{\mathbf q,i}(t_2)p_{-\mathbf q,j}(t_3)\rangle
=\delta_{ij}\bigg[
&\frac{k_BT}{a_F+\kappa q^2}e^{-r(q)|t_3-t_2|}
\\
&+\left(
\frac{k_BT}{a_I+\kappa q^2}
-\frac{k_BT}{a_F+\kappa q^2}
\right)
e^{-r(q)(t_2+t_3-2t_1)}
\bigg].
\end{aligned}
$$

When both observation times are many relaxation times after the quench, the second term vanishes and the stationary [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md) covariance remains:

$$
\boxed{\langle p_{\mathbf q,i}(t_2)p_{-\mathbf q,j}(t_3)\rangle
\longrightarrow
\delta_{ij}\frac{k_BT}{a_F+\kappa q^2}
e^{-r(q)|t_3-t_2|}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
