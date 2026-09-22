<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [exponential classification risk](../../../../../../exponential-classification-risk.md) for the training sample is $\mathcal L(F)=\sum_i e^{-y_iF(x_i)}$. At the start of round $m$, define

$$
w_i=e^{-y_iF_{m-1}(x_i)},\qquad W=\sum_iw_i,\qquad D_m(i)=w_i/W.
$$

Thus the observation weights arise directly from each point's current exponential loss. For a candidate base classifier $G$ and coefficient $\alpha$,

$$
\mathcal L(F_{m-1}+\alpha G)=\sum_iw_ie^{-\alpha y_iG(x_i)}=W\{(1-\epsilon)e^{-\alpha}+\epsilon e^\alpha\},
$$

where $\epsilon$ is its error under $D_m$. For a fixed $\alpha>0$ the bracket is increasing in $\epsilon$, so the appropriate base fit minimizes weighted classification error. With $G$ fixed, differentiation gives

$$
-(1-\epsilon)e^{-\alpha}+\epsilon e^\alpha=0,\qquad e^{2\alpha}=\frac{1-\epsilon}{\epsilon}.
$$

The second derivative is positive, hence the [exponential-loss derivation of AdaBoost](../../../../../../exponential-loss-derivation-of-adaboost.md) yields

$$
\boxed{\alpha_m=\frac12\log\frac{1-\epsilon_m}{\epsilon_m},\qquad D_{m+1}(i)=\frac{D_m(i)e^{-\alpha_m y_iG_m(x_i)}}{2\sqrt{\epsilon_m(1-\epsilon_m)}}.}
$$

The normalizer is $Z_m=(1-\epsilon_m)e^{-\alpha_m}+\epsilon_m e^{\alpha_m}=2\sqrt{\epsilon_m(1-\epsilon_m)}$. Consequently the next normalized weights again satisfy $D_{m+1}(i)\propto e^{-y_iF_m(x_i)}$, proving the update by induction from uniform initial weights. The factor by which an error gains weight relative to a correct observation is $e^{2\alpha_m}=(1-\epsilon_m)/\epsilon_m$.

This calculation also explains why repeated weak fits can improve training performance. Since the initial mean exponential loss is one, its value after $M$ rounds is $\prod_mZ_m$. A misclassified point has $y_iF_M(x_i)\le0$ and hence exponential loss at least one, giving the [AdaBoost training error bound](../../../../../../adaboost-training-error-bound.md)

$$
\frac1n\sum_i\mathbf1_{\{y_iF_M(x_i)\le0\}}\le\prod_{m=1}^M2\sqrt{\epsilon_m(1-\epsilon_m)}\le\exp\left(-2\sum_{m=1}^M\gamma_m^2\right),\qquad\gamma_m=\frac12-\epsilon_m.
$$

The last inequality uses $\sqrt{1-4\gamma_m^2}\le e^{-2\gamma_m^2}$. This is a training guarantee under positive edges, not a guarantee that further rounds always improve prediction on new observations.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
