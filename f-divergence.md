# f-divergence

↑ **Parent:** [Probability and statistics](probability-and-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/f-divergence)

For a [convex function](real-analysis.md#convex-function) $f$ satisfying $f(1)=0$, the f-divergence between [probability distributions](probability-distribution.md) $P$ and $Q$ is

$$
D_f(P\Vert Q)=\int qf(p/q)\,d\lambda,
$$

where $p=dP/d\lambda$, $q=dQ/d\lambda$, and the integrand uses the lower-semicontinuous perspective convention at $q=0$.

**Table of contents**

- [Kullback-Leibler divergence](#kullback-leibler-divergence)
  - [Binary partition bound for relative entropy](#binary-partition-bound-for-relative-entropy)
    - [Bernoulli relative entropy lower bound](#bernoulli-relative-entropy-lower-bound)
  - [Relative Fisher information](#relative-fisher-information)
    - [Relative Fisher information decay under Ornstein-Uhlenbeck flow](#relative-fisher-information-decay-under-ornstein-uhlenbeck-flow)
  - [Relative entropy nonnegativity](#relative-entropy-nonnegativity)
  - [Generalized Kullback–Leibler divergence](#generalized-kullback-leibler-divergence)
  - [Three-point identity for relative entropy](#three-point-identity-for-relative-entropy)
    - [Pythagorean identity for relative entropy](#pythagorean-identity-for-relative-entropy)
  - [Binary relative entropy](#binary-relative-entropy)
  - [Gibbs inequality](#gibbs-inequality)
    - [Log-optimal multiplicative betting](#log-optimal-multiplicative-betting)
  - [Chain rule for relative entropy](#chain-rule-for-relative-entropy)
  - [Log-sum inequality](#log-sum-inequality)
  - [Gibbs variational principle for relative entropy](#gibbs-variational-principle-for-relative-entropy)
  - [Kullback-Leibler divergence between normal distributions](#kullback-leibler-divergence-between-normal-distributions)
  - [Han's inequality for relative entropy](#han-s-inequality-for-relative-entropy)
    - [Han's entropy inequality](#han-s-entropy-inequality)
      - [Normalized subset entropy](#normalized-subset-entropy)
        - [Monotonicity of normalized subset entropies](#monotonicity-of-normalized-subset-entropies)
    - [Strong form of Han's entropy inequality](#strong-form-of-han-s-entropy-inequality)
  - [Tensorization lower bound for relative entropy](#tensorization-lower-bound-for-relative-entropy)
- [Chi-squared divergence](#chi-squared-divergence)
  - [Chi-squared divergence of product measures](#chi-squared-divergence-of-product-measures)
  - [Second moment of a mixture likelihood ratio](#second-moment-of-a-mixture-likelihood-ratio)
- [Data processing inequality for f-divergences](#data-processing-inequality-for-f-divergences)
  - [Data processing inequality for relative entropy](#data-processing-inequality-for-relative-entropy)
- [Squared Hellinger distance](#squared-hellinger-distance)
  - [Hellinger distance](#hellinger-distance)
    - [Relative entropy bound for the unnormalized Hellinger distance](#relative-entropy-bound-for-the-unnormalized-hellinger-distance)
    - [Hellinger affinity](#hellinger-affinity)
    - [Total variation–Hellinger–relative entropy inequality](#total-variation-hellinger-relative-entropy-inequality)
    - [Unnormalized Hellinger distance](#unnormalized-hellinger-distance)
    - [Hellinger bound for differences of expectations](#hellinger-bound-for-differences-of-expectations)
    - [Hellinger distance between normal distributions](#hellinger-distance-between-normal-distributions)

## Kullback-Leibler divergence

↑ **Parent:** [f-divergence](f-divergence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kullback-Leibler_divergence)

The [Kullback-Leibler divergence](#kullback-leibler-divergence), also called [relative entropy](#kullback-leibler-divergence), compares two [probability distributions](probability-distribution.md) in a specified order. In $D_{\mathrm{KL}}(P\Vert Q)$, observations follow $P$ and the comparison [probability distribution](probability-distribution.md) is $Q$: **the first argument supplies the averaging weights**. For [probability mass functions](probability-distribution.md#probability-mass-function) $p_i,q_i$ on a finite [alphabet](information-theory.md#alphabet),

$$
D_{\mathrm{KL}}(P\Vert Q)=\sum_i p_i\log\frac{p_i}{q_i}
=\mathbb E_P\!\left[\log\frac{p(X)}{q(X)}\right].
$$

Here $X$ is a [random variable](random-variable.md) with [probability distribution](probability-distribution.md) $P$. For [probability density functions](continuous-probability-distribution.md#probability-density-function) relative to the same [measure](measure.md) $\mu$, replace the [sum](arithmetic.md#sum) by $\int p\log(p/q)\,d\mu$. These formulas use [natural logarithms](calculus.md#natural-logarithm) unless stated otherwise. The [expected value](expected-value.md) is under $P$, even though $Q$ appears in the denominator. [Weissman, information measures, 2024, Definition 4](https://web.stanford.edu/class/ee276/files/previous_notes/lecture_2.pdf)

Take $P=(0.75,0.25)$ and $Q=(0.5,0.5)$ on two outcomes. Direct calculation gives

$$
\begin{aligned}
D_{\mathrm{KL}}(P\Vert Q)&=0.75\log(1.5)+0.25\log(0.5)\approx0.130812,\\
D_{\mathrm{KL}}(Q\Vert P)&=0.5\log(2/3)+0.5\log2\approx0.143841.
\end{aligned}
$$

The second outcome contributes negatively to the first [sum](arithmetic.md#sum): assigning it more [probability](probability-theory.md#probability) than $P$ does makes its individual contribution negative. Nevertheless, [relative entropy nonnegativity](#relative-entropy-nonnegativity) guarantees a nonnegative total. Reversing the arguments changes both the [likelihood ratio](statistical-hypothesis-test.md#likelihood-ratio) and the averaging [probabilities](probability-theory.md#probability); taking an absolute value inside the [logarithm](calculus.md#logarithm) would define a different quantity.

<a id="image-direction-changes-the-averaging-weights-a-missing-outcome-can-make-relative-entropy-infinite"></a>
![](kl-direction-and-support.png)

**[Figure 1](#image-direction-changes-the-averaging-weights-a-missing-outcome-can-make-relative-entropy-infinite). Direction changes the averaging weights; a missing outcome can make relative entropy infinite**.

The units depend on the [logarithm](calculus.md#logarithm): [natural logarithms](calculus.md#natural-logarithm) give [nats](information-theory.md#nat-unit), whereas base-two [logarithms](calculus.md#logarithm) give [bits](information-theory.md#bit). Divide a value in [nats](information-theory.md#nat-unit) by $\log2$ to obtain [bits](information-theory.md#bit); the forward example is approximately $0.188722$ [bits](information-theory.md#bit). Changing the base rescales every [Kullback-Leibler divergence](#kullback-leibler-divergence) by the same positive factor. Since the two calculated directions differ, [Kullback-Leibler divergence](#kullback-leibler-divergence) is asymmetric and cannot be a [metric](topological-analysis.md#metric). It also need not satisfy the [triangle inequality](topological-analysis.md#triangle-inequality). [Tse, relative entropy, 2017, Section 3.3](https://web.stanford.edu/~kedart/ee376a_winter1617/Lecture_3.pdf)

The operational meaning is an expected penalty for using the wrong [probability distribution](probability-distribution.md). A prediction $q_i$ incurs [log-loss](foundations-of-mathematics.md#logarithmic-loss) $-\log q_i$ when outcome $i$ occurs, the negative of the [logarithmic scoring rule](statistical-inference.md#logarithmic-scoring-rule). Under $P$, its [expected value](expected-value.md) is the [cross-entropy](information-entropy.md#cross-entropy) $H(P,Q)=-\sum_i p_i\log q_i$. Predicting with $P$ itself incurs [information entropy](information-entropy.md) $H(P)=-\sum_i p_i\log p_i$, so

$$
H(P,Q)-H(P)=D_{\mathrm{KL}}(P\Vert Q).
$$

Thus [Kullback-Leibler divergence](#kullback-leibler-divergence) is exactly excess expected [log-loss](foundations-of-mathematics.md#logarithmic-loss), whenever these separate quantities are finite. [Weissman, information measures, 2024, property 3](https://web.stanford.edu/class/ee276/files/previous_notes/lecture_2.pdf)

For [lossless source coding](information-theory.md#lossless-source-coding), ideal [codeword lengths](coding-theory.md#codeword-length) $-\log_2q_i$ similarly give excess expected length $D_{\mathrm{KL}}(P\Vert Q)$ in [bits](information-theory.md#bit) per symbol. Actual [prefix codes](coding-theory.md#prefix-code) require integer [codeword lengths](coding-theory.md#codeword-length); [Shannon's source coding theorem](coding-theory.md#shannon-s-source-coding-theorem) explains how long blocks approach ideal per-symbol lengths. The interpretation concerns an average, not a fractional physical [bit](information-theory.md#bit) attached to every outcome. In our example, ideal coding with $Q$ costs one [bit](information-theory.md#bit) per symbol, while $H(P)\approx0.811278$ [bits](information-theory.md#bit); the difference is exactly the computed $0.188722$ [bits](information-theory.md#bit). [Tse, information theory, 2017, Section 3.4](https://web.stanford.edu/~kedart/ee376a_winter1617/Lecture_3.pdf)

Zeros require explicit conventions. An outcome with $p_i=0$ contributes zero, including when $q_i=0$; the convention $0\log0=0$ agrees with the relevant [limit](calculus.md#limit-of-a-function). If $p_i>0$ but $q_i=0$, the [Kullback-Leibler divergence](#kullback-leibler-divergence) is infinite: the predictor has declared impossible an outcome that can occur. On a finite [alphabet](information-theory.md#alphabet), the [probability support](probability-distribution.md#support-of-a-probability-distribution) of $P$ must therefore be contained in the [probability support](probability-distribution.md#support-of-a-probability-distribution) of $Q$ for a finite answer. For example, $P=(1,0)$ and $Q=(0.5,0.5)$ give $D(P\Vert Q)=\log2$, but $D(Q\Vert P)=+\infty$. For general [probability measures](probability-space.md#probability-measure), failure of [absolute continuity of measures](measure-theory.md#absolute-continuity-of-measures) $P\ll Q$ likewise gives infinity. Even $P\ll Q$ does not guarantee a finite [integral](integral.md). [van Erven and Harremoës, Rényi Divergence and Kullback-Leibler Divergence, 2014, Section II](https://arxiv.org/pdf/1206.2459)

To see how confidently wrong predictions are punished, hold the true [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) parameter at $p=0.75$ and vary the predicted parameter $q$. Its [binary relative entropy](#binary-relative-entropy) is

$$
d(0.75,q)=0.75\log\frac{0.75}{q}+0.25\log\frac{0.25}{1-q}.
$$

It vanishes at $q=0.75$, equals approximately $2.894055$ [nats](information-theory.md#nat-unit) at $q=0.01$, and equals $0.596495$ [nats](information-theory.md#nat-unit) at $q=0.99$. Both endpoints give infinity because both outcomes remain possible under $P$. Predicting almost no successes is especially costly because successes actually occur three quarters of the time. The reversed [binary relative entropy](#binary-relative-entropy) stays finite at the endpoints: its averaging [probability distribution](probability-distribution.md) concentrates on just one outcome, and $P$ assigns positive [probability](probability-theory.md#probability) to both.

<a id="image-bernoulli-relative-entropy-with-true-success-probability-0-75-and-varying-predicted-probability"></a>
![](kl-bernoulli-penalty.png)

**[Figure 2](#image-bernoulli-relative-entropy-with-true-success-probability-0-75-and-varying-predicted-probability). Bernoulli relative entropy with true success probability 0.75 and varying predicted probability**.

For [model selection](statistical-modelling.md#model-selection), minimizing expected [log-loss](foundations-of-mathematics.md#logarithmic-loss) ranks candidate [statistical models](statistical-model.md) by $D(P\Vert Q)$, since $H(P)$ is common to them. The true [probability distribution](probability-distribution.md) is usually unknown, so one estimates predictive performance using fresh observations or [cross-validation](statistical-learning.md#cross-validation). Fitting and assessing on the same data can reward [overfitting](statistical-learning.md#overfitting); a small fitted [Kullback-Leibler divergence](#kullback-leibler-divergence) alone does not establish useful prediction.

In [variational inference](bayesian-statistics.md#variational-inference), a tractable trial [probability distribution](probability-distribution.md) $R$ commonly minimizes $D(R\Vert\Pi)$ against a target [posterior distribution](bayesian-statistics.md#bayesian-posterior) $\Pi$. Maximizing the [evidence lower bound](bayesian-statistics.md#evidence-lower-bound) accomplishes this without evaluating the target's [normalization constant](continuous-probability-distribution.md#normalizing-constant). The averaging now follows $R$: placing trial [probability](probability-theory.md#probability) where the [posterior distribution](bayesian-statistics.md#bayesian-posterior) assigns almost none is strongly penalized. The chosen direction and trial family therefore matter. [Blei, Kucukelbir and McAuliffe, Variational Inference: A Review for Statisticians, 2017, Section 2.2](https://www.cs.columbia.edu/~blei/papers/BleiKucukelbirMcAuliffe2017.pdf)

These comparisons do not by themselves establish [causal inference](causal-inference.md). Two [statistical models](statistical-model.md) can reproduce the same observed [probability distribution](probability-distribution.md) while predicting different responses to an [intervention](causal-inference.md#treatment). Choosing the smaller [Kullback-Leibler divergence](#kullback-leibler-divergence) therefore needs additional assumptions or experimental evidence before supporting a causal claim. [Pearl, Causal inference in statistics: An overview, 2009, Section 2](https://ftp.cs.ucla.edu/pub/stat_ser/r350.pdf)

The original reference is S. Kullback and R. A. Leibler's 1951 paper [On Information and Sufficiency](https://doi.org/10.1214/aoms/1177729694), published in The Annals of Mathematical Statistics 22(1), pages 79–86. Its title connects this comparison with [sufficient statistics](probability-and-statistics.md#sufficient-statistic): the historical setting was statistical information, before today's widespread applications in prediction and [variational inference](bayesian-statistics.md#variational-inference).

### Binary partition bound for relative entropy

↑ **Parent:** [Kullback-Leibler divergence](#kullback-leibler-divergence)

For a measurable event $A$, applying [Jensen inequality](real-analysis.md#jensen-s-inequality) to $u\log u$ separately on $A$ and its complement shows that the [Kullback-Leibler divergence](#kullback-leibler-divergence) between two [probability measures](probability-space.md#probability-measure) is at least the divergence between the two event indicators. This reduces a general [probability measure](probability-space.md#probability-measure) comparison to a binary one and is the key step in a proof of [Pinsker's inequality](probability-and-statistics.md#pinsker-s-inequality).

#### Bernoulli relative entropy lower bound

↑ **Parent:** [Binary partition bound for relative entropy](#binary-partition-bound-for-relative-entropy)

For $d(a,b)=a\log(a/b)+(1-a)\log((1-a)/(1-b))$, the [second derivative](calculus.md#second-derivative) with respect to $a$ is $1/[a(1-a)]\geq4$. Its value and first derivative at $a=b$ vanish, so $d(a,b)\geq2(a-b)^2$. Boundary values follow by continuity or the infinite-divergence convention. Together with the [binary partition bound for relative entropy](#binary-partition-bound-for-relative-entropy), this gives [Pinsker's inequality](probability-and-statistics.md#pinsker-s-inequality) with the natural-logarithm constant.

### Relative Fisher information

↑ **Parent:** [Kullback-Leibler divergence](#kullback-leibler-divergence)

For sufficiently regular positive [probability densities](wave-function.md#probability-density), this compares their spatial logarithmic derivatives. It is the dissipation functional for [relative entropy](#kullback-leibler-divergence) under suitable diffusion equations. For standard Gaussian $g=\gamma$, it becomes $\int|\nabla\log f+v|^2f$, and in one dimension equals $\int|f'|^2/f+\int v^2f-2$ at unit [mass](classical-mechanics.md#mass).

#### Relative Fisher information decay under Ornstein-Uhlenbeck flow

↑ **Parent:** [Relative Fisher information](#relative-fisher-information)

The differential estimate $I'(t)\leq-2I(t)$ gives the displayed exponential bound by an integrating factor. Start at any time with finite information. Combining this with a zero limiting entropy yields $H(f_t\mid\gamma)=\int_t^\infty I(s)ds\leq I(t)/2$.

### Relative entropy nonnegativity

↑ **Parent:** [Kullback-Leibler divergence](#kullback-leibler-divergence)

For [probability distributions](probability-distribution.md) $P,Q$, [relative entropy](#kullback-leibler-divergence) satisfies $D_{\mathrm{KL}}(P\Vert Q)\geq0$, with equality exactly when $P=Q$. Thus truthful prediction uniquely minimizes expected [log-loss](foundations-of-mathematics.md#logarithmic-loss) whenever the comparison is well defined, explaining the [strictly proper scoring rule](statistical-inference.md#strictly-proper-scoring-rule) property of the [logarithmic scoring rule](statistical-inference.md#logarithmic-scoring-rule).

For a short proof with [probability density functions](continuous-probability-distribution.md#probability-density-function) $f,g$ and $g>0$, set $r=f/g$. Their [integrals](integral.md) both equal one, giving

$$
H(f\mid g)=\int g\bigl(r\log r-r+1\bigr)\,d\mu\geq0.
$$

The [strictly convex function](real-analysis.md#strictly-convex-function) $r\log r-r+1$ is minimized only at $r=1$, so equality means $f=g$ [almost everywhere](measure-theory.md#almost-everywhere). Its value at zero is one by $0\log0=0$. Where $g=0<f$, [relative entropy](#kullback-leibler-divergence) is infinite; where both vanish, the contribution is zero. These conventions extend the argument beyond positive reference [probability density functions](continuous-probability-distribution.md#probability-density-function).

<h3 id="generalized-kullback-leibler-divergence">Generalized Kullback–Leibler divergence</h3>

↑ **Parent:** [Kullback-Leibler divergence](#kullback-leibler-divergence)

For nonnegative densities of possibly different total masses, this divergence includes the mass correction $-x+y$ as well as the logarithmic term. It is the [Bregman distance](inverse-problem.md#bregman-divergence) of the [maximum-entropy regularization functional](inverse-problem.md#maximum-entropy-regularization-functional) at a positive reference $y$. Convexity of $s\log s-s$ proves nonnegativity. For equal masses the correction integrates to zero, recovering the [Kullback-Leibler divergence](#kullback-leibler-divergence); for [probability density functions](continuous-probability-distribution.md#probability-density-function) both masses are one. Use the usual extended-value conventions at zero reference density.

### Three-point identity for relative entropy

↑ **Parent:** [Kullback-Leibler divergence](#kullback-leibler-divergence)

For probability mass functions $P,Q,R$ with compatible supports,

$$
D(P\Vert Q)
=D(P\Vert R)+D(R\Vert Q)
+\sum_a\{P(a)-R(a)\}\log\frac{R(a)}{Q(a)}.
$$

When the final term vanishes, this is the Pythagorean identity for relative entropy.

#### Pythagorean identity for relative entropy

↑ **Parent:** [Three-point identity for relative entropy](#three-point-identity-for-relative-entropy)

The Pythagorean identity is

$$
D(P\Vert Q)=D(P\Vert R)+D(R\Vert Q)
$$

whenever the residual term in the [three-point identity for relative entropy](#three-point-identity-for-relative-entropy) is zero. Convex information projections replace equality by the corresponding Pythagorean inequality.

### Binary relative entropy

↑ **Parent:** [Kullback-Leibler divergence](#kullback-leibler-divergence)

The binary relative entropy is the [Kullback-Leibler divergence](#kullback-leibler-divergence) between Bernoulli distributions:

$$
\operatorname{kl}(a,b)
=a\log\frac ab+(1-a)\log\frac{1-a}{1-b}.
$$

It is the exact exponent obtained by optimizing the Chernoff bound for a Bernoulli mean.

### Gibbs inequality

↑ **Parent:** [Kullback-Leibler divergence](#kullback-leibler-divergence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gibbs_inequality)

For [probability distributions](probability-distribution.md) $p$ and $q$ on the same finite set,

$$
D_{\mathrm{KL}}(p\Vert q)
=\sum_i p_i\log\frac{p_i}{q_i}\geq0,
$$

with equality exactly when $p=q$ on the support of $p$.

#### Log-optimal multiplicative betting

↑ **Parent:** [Gibbs inequality](#gibbs-inequality)

For independent outcomes with positive [probability distribution](probability-distribution.md) $p$, allocations $a_j>0$ summing to one and return multipliers $a_j/u_j$, the [strong law of large numbers](convergence-of-random-variables.md#strong-law-of-large-numbers) gives asymptotic logarithmic fortune growth $g(a)=\sum_jp_j\log(a_j/u_j)$. [Gibbs inequality](#gibbs-inequality) gives $g(a)=g(p)-D(p\Vert a)$, so the unique optimum is $a=p$. Writing $U=\sum_ju_j$ gives $g(p)=D(p\Vert u/U)-\log U$. Thus $U<1$ guarantees positive optimal growth, whereas $U>1$ allows the house to force negative growth by choosing $u_j=Up_j$, but does not guarantee decline for every choice of $u$.

### Chain rule for relative entropy

↑ **Parent:** [Kullback-Leibler divergence](#kullback-leibler-divergence)

For [probability distributions](probability-distribution.md) $P$ and $Q$ on a product space, the [Kullback-Leibler divergence](#kullback-leibler-divergence) decomposes into the divergence of a marginal and the expected divergence of the corresponding conditional distributions. Iteration gives

$$
D(Q\Vert P)=\sum_i\mathbb E_QD\bigl(Q_i(\mathord\cdot\mid X_{<i})\Vert P_i(\mathord\cdot\mid X_{<i})\bigr).
$$

### Log-sum inequality

↑ **Parent:** [Kullback-Leibler divergence](#kullback-leibler-divergence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Log-sum_inequality)

For nonnegative $a_i,b_i$, with $a=\sum_i a_i$ and $b=\sum_i b_i$, the log-sum inequality is

$$
\sum_i a_i\log\frac{a_i}{b_i}\geq a\log\frac ab.
$$

It proves both [Gibbs inequality](#gibbs-inequality) and the [data processing inequality for relative entropy](#data-processing-inequality-for-relative-entropy).

### Gibbs variational principle for relative entropy

↑ **Parent:** [Kullback-Leibler divergence](#kullback-leibler-divergence)

For a [probability mass function](probability-distribution.md#probability-mass-function) $Q$ of full support on a finite [alphabet](information-theory.md#alphabet) and a real function $g$,

$$
\log\mathbb E_Q e^g
=\sup_P\{\mathbb E_Pg-D_e(P\Vert Q)\},
$$

where $D_e$ uses [natural logarithms](calculus.md#natural-logarithm). The unique maximizing [probability mass function](probability-distribution.md#probability-mass-function) is the exponential tilt $P^*(x)=Q(x)e^{g(x)}/\mathbb E_Qe^g$.

### Kullback-Leibler divergence between normal distributions

↑ **Parent:** [Kullback-Leibler divergence](#kullback-leibler-divergence)

For univariate normal distributions,

$$
D_{\mathrm{KL}}\bigl(N(m_1,v_1)\Vert N(m_0,v_0)\bigr)
=\frac12\left[\log\frac{v_0}{v_1}+\frac{v_1+(m_1-m_0)^2}{v_0}-1\right].
$$

<h3 id="han-s-inequality-for-relative-entropy">Han's inequality for relative entropy</h3>

↑ **Parent:** [Kullback-Leibler divergence](#kullback-leibler-divergence)

If $P=\bigotimes_{i=1}^nP_i$ is a product measure, $Q$ is any probability measure, and $X^{(i)}$ omits coordinate $i$, then

$$
D(Q\Vert P)\geq\frac1{n-1}\sum_{i=1}^nD(Q_{X^{(i)}}\Vert P_{X^{(i)}}).
$$

<h4 id="han-s-entropy-inequality">Han's entropy inequality</h4>

↑ **Parent:** [Han's inequality for relative entropy](#han-s-inequality-for-relative-entropy)

For a random vector $X_{1:n}$,

$$
\sum_{i=1}^nH(X^{(i)})\geq(n-1)H(X_{1:n}).
$$

This is equivalent to [Han's inequality for relative entropy](#han-s-inequality-for-relative-entropy) after expansion against a product reference measure.

##### Normalized subset entropy

↑ **Parent:** [Han's entropy inequality](#han-s-entropy-inequality)

For a discrete [random vector](random-variable.md#random-vector) with $n$ coordinates, this is the average [information entropy](information-entropy.md) per coordinate over all subsets of size $k$. Independent coordinates give the same average for every $k$, even when their individual entropies differ. If all coordinates are copies of one random variable $Z$, the average is $h(Z)/k$.

###### Monotonicity of normalized subset entropies

↑ **Parent:** [Normalized subset entropy](#normalized-subset-entropy)

For discrete [random variables](random-variable.md), [normalized subset entropy](#normalized-subset-entropy) decreases with subset size. For finite entropies, the [chain rule for information entropy](information-entropy.md#chain-rule-for-information-entropy) and [conditioning reduces entropy](information-theory.md#conditioning-reduces-entropy) give $\sum_{i\in S}h(X_{S\setminus\{i\}})\geq(|S|-1)h(X_S)$. Sum this over all $k$-subsets $S$. Every $(k-1)$-subset occurs $n-k+1$ times, and $k\binom nk=(n-k+1)\binom n{k-1}$ cancels the normalization factors. This proves $h_k^{(n)}\leq h_{k-1}^{(n)}$. If a marginal entropy is infinite, every one of these subset averages is infinite; otherwise all entropies used in the proof are finite.

<h4 id="strong-form-of-han-s-entropy-inequality">Strong form of Han's entropy inequality</h4>

↑ **Parent:** [Han's inequality for relative entropy](#han-s-inequality-for-relative-entropy)

The strong form

$$
(n-1)\sum_iH(X^{(i)})
\geq n(n-2)H(X_{1:n})+\sum_iH(X_i)
$$

follows by iterating [entropy submodularity](information-theory.md#entropy-submodularity).

### Tensorization lower bound for relative entropy

↑ **Parent:** [Kullback-Leibler divergence](#kullback-leibler-divergence)

For a product reference $P=\bigotimes_iP_i$ and arbitrary $Q$,

$$
D(Q\Vert P)\geq\sum_iD(Q_i\Vert P_i).
$$

It follows from the [chain rule for relative entropy](#chain-rule-for-relative-entropy) and convexity of relative entropy in its first argument.

## Chi-squared divergence

↑ **Parent:** [f-divergence](f-divergence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chi-squared_divergence)

For [probability mass functions](probability-distribution.md#probability-mass-function) $P,Q$ with $P$ absolutely continuous with respect to $Q$,

$$
\chi^2(P\Vert Q)=\sum_x\frac{(P(x)-Q(x))^2}{Q(x)}.
$$

### Chi-squared divergence of product measures

↑ **Parent:** [Chi-squared divergence](#chi-squared-divergence)

If $r=dQ/dP$, [independence](random-variable.md#independent-random-variables) gives $E_{P^{\otimes n}}\prod_i r(X_i)^2=(E_Pr^2)^n$. Since $E_Pr=1$, this proves the displayed identity. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) also gives $\|Q^{\otimes n}-P^{\otimes n}\|_1^2\leq\chi^2(Q^{\otimes n}\Vert P^{\otimes n})$. Thus perturbations of size $\chi^2(Q\Vert P)=O(1/n)$ have a uniformly bounded joint [total variation distance](probability-and-statistics.md#total-variation-distance), a useful input to a [metric squared-loss two-point bound](statistical-inference.md#metric-squared-loss-two-point-bound).

### Second moment of a mixture likelihood ratio

↑ **Parent:** [Chi-squared divergence](#chi-squared-divergence)

If $L_j=dP_j/dQ$ and the nonnegative [mixture weights](statistical-modelling.md#mixture-weight) sum to one, the [likelihood ratio](statistical-hypothesis-test.md#likelihood-ratio) of the [mixture model](statistical-modelling.md#mixture-model) is $L=\sum_jw_jL_j$. Expanding $\mathbb E_QL^2-1$ proves the displayed [chi-squared divergence](#chi-squared-divergence) identity. For [independent random variables](random-variable.md#independent-random-variables) sampled from a fixed component, one-observation cross moments multiply across observations. The component is drawn once for the whole sample; redrawing it per observation gives a different [mixture model](statistical-modelling.md#mixture-model).

## Data processing inequality for f-divergences

↑ **Parent:** [f-divergence](f-divergence.md)

For a [measurable function](measure-theory.md#measurable-function) $T$, every f-divergence contracts under [pushforward](measure.md#pushforward-measure):

$$
D_f(T_*P\Vert T_*Q)\leq D_f(P\Vert Q).
$$

This follows from conditional [Jensen inequality](real-analysis.md#jensen-s-inequality) applied to the jointly convex perspective $(a,b)\mapsto bf(a/b)$.

### Data processing inequality for relative entropy

↑ **Parent:** [Data processing inequality for f-divergences](#data-processing-inequality-for-f-divergences)

This is the [data processing inequality for f-divergences](#data-processing-inequality-for-f-divergences) specialized to [relative entropy](#kullback-leibler-divergence). Passing two [probability distributions](probability-distribution.md) through the same [Markov kernel](markov-chain.md#markov-kernel) cannot increase their [relative entropy](#kullback-leibler-divergence). For a kernel $K$,

$$
D(PK\Vert QK)\leq D(P\Vert Q).
$$

## Squared Hellinger distance

↑ **Parent:** [f-divergence](f-divergence.md)

The squared Hellinger distance is

$$
H^2(P,Q)=\int(\sqrt p-\sqrt q)^2d\lambda
=2-2\int\sqrt{pq}\,d\lambda,
$$

where $p$ and $q$ are densities with respect to any common dominating measure $\lambda$.

### Hellinger distance

↑ **Parent:** [Squared Hellinger distance](#squared-hellinger-distance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hellinger_distance)

The Hellinger distance is the square root of a constant multiple of $\int(\sqrt p-\sqrt q)^2d\lambda$. Common conventions use either the factor $1$ or $1/2$.

#### Relative entropy bound for the unnormalized Hellinger distance

↑ **Parent:** [Hellinger distance](#hellinger-distance)

The scalar inequality $-\log u\geq1-u$, applied to $u=\sqrt{q/p}$ and integrated against $P$, gives $K(P,Q)\geq2-2\int\sqrt{pq}\,d\mu$. The right side is the unnormalized squared [Hellinger distance](#hellinger-distance). Infinite divergence and zero density regions are handled by the usual extended-integral conventions.

#### Hellinger affinity

↑ **Parent:** [Hellinger distance](#hellinger-distance)

The [Hellinger affinity](#hellinger-affinity) of dominated [probability measures](probability-space.md#probability-measure) is the integral of the geometric mean of their [probability density functions](continuous-probability-distribution.md#probability-density-function). It lies in $[0,1]$ by [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). The unnormalized squared [Hellinger distance](#hellinger-distance) is $2-2$ times this affinity; this identity makes the relation with [relative entropy](#kullback-leibler-divergence) particularly simple.

<h4 id="total-variation-hellinger-relative-entropy-inequality">Total variation–Hellinger–relative entropy inequality</h4>

↑ **Parent:** [Hellinger distance](#hellinger-distance)

For the [unnormalized Hellinger distance](#unnormalized-hellinger-distance), $\operatorname{TV}(P,Q)\leq h(P,Q)\leq\sqrt{\operatorname{KL}(P,Q)}$. Factor $|p-q|=|\sqrt p-\sqrt q|(\sqrt p+\sqrt q)$ and use the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) to bound the [total variation distance](probability-and-statistics.md#total-variation-distance). For the other bound, $\log t\leq t-1$ gives $p\log(p/q)\geq2(p-\sqrt{pq})$, whose integral is the squared [unnormalized Hellinger distance](#unnormalized-hellinger-distance). Infinite [Kullback-Leibler divergence](#kullback-leibler-divergence) is allowed.

#### Unnormalized Hellinger distance

↑ **Parent:** [Hellinger distance](#hellinger-distance)

The [Hellinger distance](#hellinger-distance) convention $h^2(P,Q)=\int(\sqrt p-\sqrt q)^2\,d\nu$, with no factor $1/2$, for densities under a common dominating measure. Its range is $[0,\sqrt2]$. This convention makes $\operatorname{TV}(P,Q)\leq h(P,Q)\leq\sqrt{\operatorname{KL}(P,Q)}$ hold with the displayed constants.

#### Hellinger bound for differences of expectations

↑ **Parent:** [Hellinger distance](#hellinger-distance)

If $f$ is a measurable function into a separable [Banach space](banach-space.md) and has finite second [moments](expected-value.md#moment) under [probability measures](probability-space.md#probability-measure) $\mu,\mu'$, then their [Bochner integral](measure-theory.md#bochner-integral) [expected values](expected-value.md) satisfy

$$
\|\mathbb E^\mu f-\mathbb E^{\mu'}f\|
\leq2\left(\mathbb E^\mu\|f\|^2+\mathbb E^{\mu'}\|f\|^2\right)^{1/2}d_{\mathrm{Hell}}(\mu,\mu').
$$

Here the [Hellinger distance](#hellinger-distance) includes the factor $1/2$ in its square. For a proof, use $\nu=(\mu+\mu')/2$, $p=d\mu/d\nu$, and $q=d\mu'/d\nu$. Apply the norm bound for a [Bochner integral](measure-theory.md#bochner-integral) and the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) to $f(p-q)=f(\sqrt p-\sqrt q)(\sqrt p+\sqrt q)$, then use $(\sqrt p+\sqrt q)^2\leq2(p+q)$. This explains why stability of a [Bayesian posterior](bayesian-statistics.md#bayesian-posterior) in [Hellinger distance](#hellinger-distance) controls posterior [expected values](expected-value.md) when the relevant second [moments](expected-value.md#moment) remain bounded.

#### Hellinger distance between normal distributions

↑ **Parent:** [Hellinger distance](#hellinger-distance)

With the convention $d_{\mathrm{Hell}}^2=\frac12\int(\sqrt p-\sqrt q)^2$, the [Hellinger distance](#hellinger-distance) between two [normal distributions](probability-distribution.md#normal-distribution) with $\sigma_1,\sigma_2>0$ is

$$
d_{\mathrm{Hell}}^2=1-\sqrt{\frac{2\sigma_1\sigma_2}{\sigma_1^2+\sigma_2^2}}
\exp\left[-\frac{(\theta_1-\theta_2)^2}{4(\sigma_1^2+\sigma_2^2)}\right].
$$

To prove it, integrate the geometric mean of their [probability density functions](continuous-probability-distribution.md#probability-density-function). [Completing the square](polynomial.md#completing-the-square) makes that geometric mean the density of a [normal distribution](probability-distribution.md#normal-distribution) times the displayed prefactor and exponential. For example, writing $S=\sigma_1^2+\sigma_2^2$, that [normal distribution](probability-distribution.md#normal-distribution) has mean $(\theta_1\sigma_2^2+\theta_2\sigma_1^2)/S$ and [variance](variance.md) $2\sigma_1^2\sigma_2^2/S$. The identity $d_{\mathrm{Hell}}^2=1-\int\sqrt{pq}$ then proves the formula.

For equal unit [variances](variance.md), this becomes $1-e^{-(\theta_1-\theta_2)^2/8}$. More generally, put $B=\sqrt{2\sigma_1\sigma_2/S}\leq1$ and $x=(\theta_1-\theta_2)^2/(4S)$. Then $1-Be^{-x}=(1-B)+B(1-e^{-x})$, $1-B=(\sigma_1-\sigma_2)^2/[S(1+B)]$, and $1-e^{-x}\leq x$, proving

$$
d_{\mathrm{Hell}}^2\leq\frac{(\sigma_1-\sigma_2)^2+(\theta_1-\theta_2)^2}{\sigma_1^2+\sigma_2^2}.
$$

## ↑ Ancestors (4)

1. [Probability and statistics](probability-and-statistics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-210.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-210.md#4/solution)
