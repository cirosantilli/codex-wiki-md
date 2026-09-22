<h1 id="fano-s-inequality">Fano's inequality</h1>

↑ **Parent:** [Conditional entropy](conditional-entropy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fano's_inequality)

Fano's inequality turns remaining uncertainty into a constraint on decision errors. If an observation leaves many plausible answers, a [decoder](channel-decoder.md) cannot usually recover the answer reliably. Its elegant idea is to separate two uncertainties: whether the guess was wrong, and which alternative was correct when it was wrong.

Let $X,Y$ be [discrete random variables](discrete-random-variable.md), with $X$ taking values in a finite [alphabet](alphabet.md) $\mathcal X$ of [cardinality](cardinality.md) $M\geq2$. Choose any deterministic [decoder](channel-decoder.md) $\widehat X=f(Y)$ whose output lies in $\mathcal X$, and define its average error [probability](probability.md) $p_e=\mathbb P\{\widehat X\ne X\}$. With base-two [logarithms](logarithm.md), [Fano's inequality](fano-s-inequality.md) states

$$
H(X\mid Y)\leq h_2(p_e)+p_e\log_2(M-1),\qquad 0\leq p_e\leq1.
$$

Here $H(X\mid Y)$ is [conditional entropy](conditional-entropy.md) and $h_2$ is [binary entropy](binary-entropy.md), with $0\log_2 0=0$ at the endpoints. Both sides are measured in [bits](bit.md); using [natural logarithms](natural-logarithm.md) throughout gives the same inequality in [nats](nat-unit.md). No uniform source, independence of $X,Y$, or optimality of the [decoder](channel-decoder.md) is assumed. Requiring its output to belong to the same [alphabet](alphabet.md) is what leaves at most $M-1$ alternatives after an error.[Polyanskiy and Wu, MIT 6.441 course notes, Section 5.3, Theorem 5.3](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others.md)

For an exact toy example, give $X$ the [discrete uniform distribution](discrete-uniform-distribution.md) on $\{A,B,C,D\}$. A [channel](communication-channel.md) reports $Y=X$ with [probability](probability.md) $1-q$ and reports each of the other three symbols with [probability](probability.md) $q/3$, where $0\leq q\leq1$. Use the [decoder](channel-decoder.md) $f(y)=y$. The output is uniform, and the [conditional probabilities](conditional-probability.md) after any report $y$ are

$$
\mathbb P(X=x\mid Y=y)=
\begin{cases}
1-q,&x=y,\\
q/3,&x\ne y.
\end{cases}
$$

Thus $p_e=q$ and direct calculation of the [conditional entropy](conditional-entropy.md) gives

$$
H(X\mid Y)=-(1-q)\log_2(1-q)-3\frac q3\log_2\frac q3
=h_2(q)+q\log_2 3.
$$

This is equality in [Fano's inequality](fano-s-inequality.md) for every $q\in[0,1]$. At $q=0.3$, each report leaves [probabilities](probability.md) $(0.7,0.1,0.1,0.1)$, up to their order, and $H(X\mid Y)\approx1.3568$ [bits](bit.md). The two contributions are $h_2(0.3)\approx0.8813$ [bits](bit.md) for the error flag and $0.3\log_2 3\approx0.4755$ [bits](bit.md) for identifying the correct alternative after an error. These are theoretical [probabilities](probability.md), not measured data.

<a id="image-a-symmetric-four-symbol-toy-channel-makes-every-step-of-fano-s-bound-an-equality"></a>
![](fano-four-symbol-posterior.png)

**[Figure 4](#image-a-symmetric-four-symbol-toy-channel-makes-every-step-of-fano-s-bound-an-equality). A symmetric four-symbol toy channel makes every step of Fano's bound an equality**.

The identity [decoder](channel-decoder.md) in this example minimizes error only for $0\leq q\leq3/4$: its guessed symbol has the largest [posterior probability](posterior-probability.md) exactly when $1-q\geq q/3$. At $q=3/4$, $X,Y$ are [independent random variables](independent-random-variables.md) and all four guesses tie. For $q>3/4$, guessing any one of the three other symbols has error [probability](probability.md) $1-q/3<q$. Equality in [Fano's inequality](fano-s-inequality.md) therefore does not certify an optimal [decoder](channel-decoder.md).

For usefulness, combine $h_2(p_e)\leq1$ with $\log_2(M-1)\leq\log_2 M$ to obtain the simpler consequence

$$
p_e\geq\max\!\left\{0,\frac{H(X\mid Y)-1}{\log_2 M}\right\}.
$$

For a uniform $X$, $H(X\mid Y)=\log_2 M-I(X;Y)$, so this becomes $p_e\geq\max\{0,1-(I(X;Y)+1)/\log_2 M\}$. This connects [mutual information](mutual-information.md) to unavoidable decision error in [channel coding](channel-coding.md) or [classification in statistical learning](classification-in-statistical-learning.md); it can rule out reliable recovery regardless of the chosen [decoder](channel-decoder.md).[Weissman, Ochoa and Tatwawadi, EE376A course notes, Sections 5.7–5.8](https://web.stanford.edu/class/ee376a/files/lecture_notes.pdf)

The sharper right-hand side $F_M(p)=h_2(p)+p\log_2(M-1)$ increases from zero to $\log_2 M$ on $0\leq p\leq1-1/M$, then decreases: in the interior, $F_M'(p)=\log_2((M-1)(1-p)/p)$. When interpreting the inequality by inverting a curve, use its increasing branch to obtain a lower error threshold. A [decoder](channel-decoder.md) that chooses a largest [posterior probability](posterior-probability.md), as in [maximum a posteriori decoding](maximum-a-posteriori-decoding.md), always has $p_e\leq1-1/M$, since the largest of $M$ conditional [probabilities](probability.md) is at least $1/M$. Arbitrary [decoders](channel-decoder.md) can have larger error. In particular, low [conditional entropy](conditional-entropy.md) does not force every [decoder](channel-decoder.md) to work well: with a fair binary $X$ and $Y=X$, the rule $f(Y)=1-Y$ has $p_e=1$ even though $H(X\mid Y)=0$. [Fano's inequality](fano-s-inequality.md) supplies a constraint, not an exact error prediction for each rule.

**Table of contents**

- [Fano's inequality via an error indicator](fano-s-inequality-via-an-error-indicator.md)
- [List-decoding Fano inequality](list-decoding-fano-inequality.md)

## ↑ Ancestors (6)

1. [Conditional entropy](conditional-entropy.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Fano's inequality](fano-s-inequality.md)
- [Fano's inequality via an error indicator](fano-s-inequality-via-an-error-indicator.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-34/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-48/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/4/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323/5/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/3g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323/3/ii/solution.md)
- [Product-input block bound for a qubit depolarizing channel](product-input-block-bound-for-a-qubit-depolarizing-channel.md)
- [Product-input classical-capacity converse](product-input-classical-capacity-converse.md)
