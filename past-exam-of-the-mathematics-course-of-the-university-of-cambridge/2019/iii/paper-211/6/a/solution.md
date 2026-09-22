<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the multidimensional [Itô formula](../../../../../../ito-s-lemma.md) to $\xi_t=F(t,S_t,v_t)$. The stated PDE cancels its drift to $rFdt$, leaving

$$
\begin{aligned}
d\xi_t={}&r\xi_tdt
+\sqrt{v_t}\left(S_tF_S+c\rho F_v\right)dW_t\\
&+c\sqrt{v_t}\sqrt{1-\rho^2}F_v\,dZ_t.
\end{aligned}
$$

Consequently $e^{-rt}S_t$ and $e^{-rt}\xi_t$ are local martingales under the physical measure $P$. Thus $P$ itself is an [equivalent local martingale measure](../../../../../../equivalent-local-martingale-measure.md) for the augmented market relative to the bank account. The continuous-time [fundamental theorem of asset pricing](../../../../../../fundamental-theorem-of-asset-pricing.md) says that existence of such a measure for locally bounded prices implies no free lunch with vanishing risk, and hence no arbitrage. The terminal condition also gives $\xi_T=\sqrt{S_T}$ as required.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
