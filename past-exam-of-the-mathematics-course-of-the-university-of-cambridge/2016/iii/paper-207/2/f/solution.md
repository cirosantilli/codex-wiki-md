<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Let $\epsilon$ be the [false positive rate](../../../../../../false-positive-rate.md) for a genuinely cancer-free person, encompassing the harmless-tumour misclassification, and assume screening errors are conditionally independent given the latent states. A pre-clinical case tests positive with probability one; a clinical case is separately recognized. Thus a negative screen identifies latent state $1$, whereas a positive pre-clinical screen can arise from state $1$ or $2$. This is a [Hidden Markov model](../../../../../../hidden-markov-model.md) with a [screening misclassification model](../../../../../../screening-misclassification-model.md).

Conditional on the negative baseline screen, the state at year $0$ is $1$. The negative screen at year $2$ requires staying in state $1$ for two years and then testing negative. From that state, the positive screen at year $4$ can arise either with probability $\epsilon$ while still disease-free or through pre-clinical disease. Consequently **the conditional likelihood** is

$$
\boxed{L_{\mathrm{cond}}=e^{-2\lambda}(1-\epsilon)\left[\epsilon e^{-2\lambda}+\frac{\lambda}{\nu-\lambda}(e^{-2\lambda}-e^{-2\nu})\right].}
$$

If the study instead specifies an initially disease-free patient and includes the baseline screening result in the [likelihood function](../../../../../../likelihood-function.md), its probability contributes a further factor $1-\epsilon$, giving

$$
\boxed{L_{\mathrm{all}}=(1-\epsilon)^2e^{-2\lambda}\left[\epsilon e^{-2\lambda}+\frac{\lambda}{\nu-\lambda}(e^{-2\lambda}-e^{-2\nu})\right].}
$$

The formulas use the positive emission for a pre-clinical screen, with no clinical diagnosis in this record. A persistent harmless-tumour subtype producing correlated screening errors would need an additional latent-state or emission specification; its likelihood is not determined by the single parameter $\epsilon$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
