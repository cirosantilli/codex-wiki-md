<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\varepsilon=\varepsilon_t$, $\alpha=\alpha_t$, and $s_i=y_i h_t(x_i)\in\{-1,1\}$. Correctly classified observations have $s_i=1$ and total $D_t$-weight $1-\varepsilon$; incorrectly classified observations have $s_i=-1$ and total weight $\varepsilon$. The [normalizing constant](../../../../../normalizing-constant.md) in the [AdaBoost](../../../../../adaboost.md) update is therefore

$$
Z_{t+1}=\sum_iD_t(i)e^{-\alpha s_i}
=(1-\varepsilon)e^{-\alpha}+\varepsilon e^\alpha.
$$

For $0<\varepsilon<1$, the definition of $\alpha$ gives

$$
e^\alpha=\sqrt{\frac{1-\varepsilon}{\varepsilon}},\qquad
e^{-\alpha}=\sqrt{\frac{\varepsilon}{1-\varepsilon}},\qquad
\boxed{Z_{t+1}=2\sqrt{\varepsilon(1-\varepsilon)}.}
$$

If observation $i$ is correct, its multiplier in the normalized update is

$$
\frac{e^{-\alpha}}{Z_{t+1}}=\frac1{2(1-\varepsilon)};
$$

if it is incorrect, the multiplier is

$$
\frac{e^\alpha}{Z_{t+1}}=\frac1{2\varepsilon}.
$$

The corresponding denominators are exactly $1+s_i(1-2\varepsilon)$: they are $2(1-\varepsilon)$ when $s_i=1$ and $2\varepsilon$ when $s_i=-1$. Consequently

$$
\boxed{D_{t+1}(i)=\frac{D_t(i)}{1+y_i h_t(x_i)(1-2\varepsilon_t)}.}
$$

As a check, the new total mass on correctly classified observations is $(1-\varepsilon)/(2(1-\varepsilon))=1/2$, and the mass on incorrectly classified observations is $\varepsilon/(2\varepsilon)=1/2$. The update thus produces a [probability distribution](../../../../../probability-distribution-split.md) and assigns the two groups equal aggregate mass. When $\varepsilon=1/2$, $\alpha=0$ and every individual weight is unchanged.

The displayed finite update assumes **$0<\varepsilon_t<1$**. The usual [weak learner](../../../../../weak-learner.md) guarantees $\varepsilon_t<1/2$, but it can return a perfect [classifier](../../../../../classifier.md) with $\varepsilon_t=0$; then the logarithm is infinite and the normalized exponential formula is not defined. [AdaBoost](../../../../../adaboost.md) stops on that perfect hypothesis rather than executing this update. Similarly, the printed formula is not an ordinary finite update at $\varepsilon_t=1$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Computational learning theory](../../../computational-learning-theory-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
