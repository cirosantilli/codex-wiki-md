<h1 id="fano-s-inequality-via-an-error-indicator">Fano's inequality via an error indicator</h1>

↑ **Parent:** [Fano's inequality](fano-s-inequality.md)

Under the hypotheses of [Fano's inequality](fano-s-inequality.md), let $J_X=\mathcal X$, $M=|J_X|$, and let $Z=\mathbf1_{\{X\ne f(Y)\}}$ be the [indicator random variable](indicator-random-variable.md) of an error. Its [probability](probability.md) of being one is $p_e$. The $h$ in the displayed bound denotes [binary entropy](binary-entropy.md) $h_2$ in [bits](bit.md). Since $Z$ is a deterministic [function](function-split.md) of $(X,Y)$, $H(Z\mid X,Y)=0$. Applying the [chain rule for conditional entropy](chain-rule-for-conditional-entropy.md) in both orders gives the exact decomposition

$$
\begin{aligned}
H(X\mid Y)
&=H(X,Z\mid Y)\\
&=H(Z\mid Y)+H(X\mid Z,Y).
\end{aligned}
$$

The first term is bounded by $H(Z)=h_2(p_e)$, because [conditioning reduces entropy](conditioning-reduces-entropy.md). For the second term, fix a report $Y=y$: if $Z=0$, then $X=f(y)$ is known; if $Z=1$, then $X$ lies among at most $M-1$ other symbols. [Maximum entropy on a finite alphabet](maximum-entropy-on-a-finite-alphabet.md) bounds the latter uncertainty by $\log_2(M-1)$. Averaging over the reports and the error flag gives

$$
H(X\mid Z,Y)\leq(1-p_e)\cdot0+p_e\log_2(M-1).
$$

This proves [Fano's inequality](fano-s-inequality.md). Events of zero [probability](probability.md) contribute zero to this average, so the proof also covers $p_e=0,1$ without assigning a conditional distribution to an impossible event.[Weissman, Ochoa and Tatwawadi, EE376A course notes, Section 5.7, proof of Theorem 46](https://web.stanford.edu/class/ee376a/files/lecture_notes.pdf)

<a id="image-the-four-symbol-entropy-budget-peaks-at-chance-level-error-and-separates-the-error-flag-from-the-three-alternatives"></a>
![](fano-error-entropy-budget.png)

**[Figure 5](#image-the-four-symbol-entropy-budget-peaks-at-chance-level-error-and-separates-the-error-flag-from-the-three-alternatives). The four-symbol entropy budget peaks at chance-level error and separates the error flag from the three alternatives**.

The decomposition also explains equality. The first bound is exact when the [indicator random variable](indicator-random-variable.md) $Z$ and $Y$ are [independent random variables](independent-random-variables.md): knowing the report does not change the error [probability](probability.md). The second is exact when, for every report with positive error [probability](probability.md), the wrong-symbol [conditional distribution](conditional-distribution.md) is uniform on all $M-1$ alternatives. Both conditions hold in the four-symbol toy [channel](communication-channel.md) of [Fano's inequality](fano-s-inequality.md). At $q=0$, the second condition is vacuous; at $q=1$, the flag is constant but three alternatives remain, giving $H(X\mid Y)=\log_2 3$. For $M=2$, there is just one alternative after an error, so the second term vanishes: all remaining uncertainty is whether the single alternative must replace the guess.

## ↑ Ancestors (7)

1. [Fano's inequality](fano-s-inequality.md)
2. [Conditional entropy](conditional-entropy.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Chain rule for conditional entropy](chain-rule-for-conditional-entropy.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60/2/ii/c/solution.md)
