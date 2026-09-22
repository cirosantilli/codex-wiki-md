<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use labels $y_i\in\{-1,1\}$ and base predictions $G_m(x)\in\{-1,1\}$. The binary [AdaBoost](../../../../../../adaboost.md) algorithm starts with observation weights $D_1(i)=1/n$ and score $F_0(x)=0$. For rounds $m=1,\ldots,M$:

- Fit the [weak learner](../../../../../../weak-learner.md) to the training observations using weights $D_m(i)$, producing $G_m$.
- Compute its weighted error $\epsilon_m=\sum_iD_m(i)\mathbf1_{\{G_m(x_i)\ne y_i\}}$.
- For $0<\epsilon_m<1/2$, choose $\alpha_m=\tfrac12\log[(1-\epsilon_m)/\epsilon_m]$ and update $F_m=F_{m-1}+\alpha_mG_m$.
- Reweight and normalize: $D_{m+1}(i)=D_m(i)e^{-\alpha_m y_iG_m(x_i)}/Z_m$, where $Z_m$ is the sum of the unnormalized weights.

The final classifier is

$$
\boxed{\widehat G(x)=\operatorname{sign}\left\{\sum_{m=1}^M\alpha_mG_m(x)\right\}.}
$$

Resolve a zero-score tie by a fixed convention. A classifier with error above $1/2$ may be sign-reversed if the base class permits it; otherwise it fails the weak-learning requirement and should be replaced. Error $1/2$ gives zero weight and no improvement. Error zero gives the limiting perfect-classifier step with infinite coefficient, so terminate with that classifier rather than computing the undefined finite update. Misclassified observations are multiplied by $e^{\alpha_m}$ and correctly classified observations by $e^{-\alpha_m}$, increasing the relative weight of errors for the next round. The procedure is sequential, and its number of rounds is a tuning parameter.

## ↑ Ancestors (11)

1. [A](../a.md)
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
