# Information entropy dominates min-entropy

↑ **Parent:** [Min-entropy](min-entropy.md)

For a [discrete random variable](discrete-random-variable.md) $X$ with [probability mass function](probability-mass-function.md) $p_x$, using base-two [logarithms](logarithm.md) for both [Shannon entropy](information-entropy-split.md) and [min-entropy](min-entropy.md),

$$
H(X)\geq H_\infty(X)\geq0.
$$

The first inequality says that average [information content](information-content.md) cannot be below the least [information content](information-content.md) of a possible outcome. For a finite [alphabet](alphabet.md), equality $H(X)=H_\infty(X)$ holds exactly when the [probability mass function](probability-mass-function.md) is uniform on its positive-probability outcomes. Impossible outcomes do not need to share that positive [probability](probability.md). In particular, $(1/2,1/2,0)$ has both quantities equal to $1$ [bit](bit.md), while $(1,0,0)$ has both zero. The same equality characterization holds for a countable [alphabet](alphabet.md): equality forces only finitely many positive-probability outcomes, because all must have the same positive mass. The uniform maximum of [Shannon entropy](information-entropy-split.md) is discussed in Shannon's original treatment.[Shannon, A Mathematical Theory of Communication, Section 6, definition of H and properties 1–2](a-mathematical-theory-of-communication-by-claude-shannon.md)

For the proof, $0<p_x\leq p_{\max}$ gives $-\log_2p_x\geq-\log_2p_{\max}$; taking the [expected value](expected-value-split.md) proves [information entropy dominates min-entropy](information-entropy-dominates-min-entropy.md). More precisely, the nonnegative gap is

$$
H(X)-H_\infty(X)
=\sum_{x:p_x>0}p_x\log_2\frac{p_{\max}}{p_x}\geq0.
$$

It vanishes precisely when every positive term vanishes, namely $p_x=p_{\max}$ for every possible outcome. With $m$ such outcomes, normalization forces $p_{\max}=1/m$. If [Shannon entropy](information-entropy-split.md) is infinite, the inequality still holds and is strict, because [min-entropy](min-entropy.md) of a countable [probability mass function](probability-mass-function.md) is finite. No subtraction of two infinite quantities is needed.

An analytical family makes the gap visible. Give $A$ [probability](probability.md) $q$ and each of $B,C,D,E$ [probability](probability.md) $(1-q)/4$, with $1/5\leq q\leq1$. Then $A$ is a most likely outcome, so its [probability](probability.md) is also the best single-guess success [probability](probability.md), and

$$
H_\infty(q)=-\log_2q,\qquad H(q)=h_2(q)+2(1-q),
$$

where $h_2$ is [binary entropy](binary-entropy.md). The [entropy bound with one prescribed probability](entropy-bound-with-one-prescribed-probability.md) explains the second expression: it separates whether $A$ occurred from which of four equally likely alternatives occurred. At $q=1/5$, all five outcomes are uniform and both quantities are $\log_2 5\approx2.3219$ [bits](bit.md). At $q=1/2$, [Shannon entropy](information-entropy-split.md) is $2$ [bits](bit.md) while [min-entropy](min-entropy.md) is $1$ [bit](bit.md), reproducing the biased example in [min-entropy](min-entropy.md). At $q=1$, both are zero; the four impossible alternatives contribute nothing. For every $1/5<q<1$, the [probability mass function](probability-mass-function.md) is nonuniform on its possible outcomes and the gap is strictly positive.

<a id="image-an-analytical-five-outcome-model-separates-average-surprise-from-the-surprise-of-the-most-likely-outcome"></a>
![](min-entropy-guessing-inequality-family.png)

**[Figure 6](#image-an-analytical-five-outcome-model-separates-average-surprise-from-the-surprise-of-the-most-likely-outcome). An analytical five-outcome model separates average surprise from the surprise of the most likely outcome**.

For finite [Shannon entropy](information-entropy-split.md), exponentiating the inequality gives the useful but potentially loose bound $p_{\mathrm{guess}}(X)\geq2^{-H(X)}$. Equality holds exactly for a [discrete uniform distribution](discrete-uniform-distribution.md) on the possible outcomes. Thus [Shannon entropy](information-entropy-split.md) alone supplies a lower bound on optimal success, not the upper bound needed to promise that every guess is unlikely. [Shannon's source coding theorem](shannon-s-source-coding-theorem.md) concerns average compression under its hypotheses, while [min-entropy](min-entropy.md) answers the single-guess question directly. The two quantities serve different tasks even when both are expressed in [bits](bit.md).

## ↑ Ancestors (7)

1. [Min-entropy](min-entropy.md)
2. [Information entropy](information-entropy-split.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Information entropy dominates min-entropy](information-entropy-dominates-min-entropy.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-224/1/d/solution.md)
