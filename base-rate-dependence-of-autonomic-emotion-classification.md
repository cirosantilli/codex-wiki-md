# Base-rate dependence of autonomic emotion classification

↑ **Parent:** [Autonomic emotion classification](autonomic-emotion-classification.md)

Fix a true-positive [probability](probability.md) $s>0$ and false-positive [probability](probability.md) $f>0$. The [positive predictive value](positive-predictive-value.md) at [base rate](base-rate.md) $p$ is $v(p)=sp/(sp+f(1-p))$. Differentiation gives $v'(p)=sf/[f+(s-f)p]^2>0$, while $v(p)\to0$ as $p\to0$. Thus a [classifier](classifier.md) can retain the same conditional performance yet become unreliable among its positive classifications when the target [emotion](emotion.md) is rare. This is a mathematical implication of the specified binary model, not an empirical performance estimate.

## ↑ Ancestors (5)

1. [Autonomic emotion classification](autonomic-emotion-classification.md)
2. [Psychophysiology](psychophysiology.md)
3. [Psychology](psychology-split.md)
4. [Science](science.md)
5. [Codex Wiki](split.md)
