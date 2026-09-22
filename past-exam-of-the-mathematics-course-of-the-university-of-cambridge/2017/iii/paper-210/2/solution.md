<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose a [Borel measurable function](../../../../../borel-measurable-function.md) version of the posterior success [probability](../../../../../probability.md) $\eta:\mathbb R^d\to[0,1]$. Conditional on $X=x$, predicting zero has error [probability](../../../../../probability.md) $\eta(x)$ and predicting one has error [probability](../../../../../probability.md) $1-\eta(x)$. A [Bayes classifier](../../../../../bayes-classifier.md) for [zero-one loss](../../../../../misclassification-loss.md) is therefore

$$
\boxed{C^{\rm Bayes}(x)=\mathbb1_{\{\eta(x)\geq1/2\}},\qquad
R^*=\mathbb E\min\{\eta(X),1-\eta(X)\}.}
$$

Either decision is optimal when $\eta(x)=1/2$. The displayed [Bayes risk](../../../../../bayes-risk.md) also equals $\int\min\{\eta(x),1-\eta(x)\}\,dP_X(x)$ and is unaffected by changing $\eta$ on a $P_X$-null set.

For any measurable set $A\subseteq\mathbb R^d$, [independence](../../../../../independent-random-variables.md) and the [uniform distribution](../../../../../continuous-uniform-distribution.md) of $U_1$ give

$$
\begin{aligned}
\mathbb P(X_1\in A,Y_1=1)
&=\int_A\mathbb P(U_1\leq\eta(x))\,dP_X(x)\\
&=\int_A\eta(x)\,dP_X(x)
=\mathbb P(X\in A,Y=1).
\end{aligned}
$$

Likewise the [probability](../../../../../probability.md) with label zero is $\int_A(1-\eta(x))\,dP_X(x)$. These sets determine the [joint probability distribution](../../../../../joint-probability-distribution.md), so

$$
\boxed{(X_1,Y_1)\ \stackrel{d}{=}\ (X,Y).}
$$

The same construction makes all training pairs [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md).

Fix a [feature-measurable nearest-neighbour tie-breaking](../../../../../feature-measurable-nearest-neighbour-tie-breaking.md) rule, for example increasing original index for observations at equal [Euclidean norm](../../../../../euclidean-norm.md) distance from the query. This is important: the ordering may depend on the features, but not on the $U_i$ or labels. Let $Y_{(j)}(x)$ be the label attached to the $j$th ordered feature. The [classifier](../../../../../classifier.md) from the [K-nearest neighbors algorithm](../../../../../k-nearest-neighbors-algorithm.md) is

$$
\boxed{\widehat C_n^{k{\rm nn}}(x)
=\mathbb1_{\{k^{-1}\sum_{j=1}^kY_{(j)}(x)\geq1/2\}}.}
$$

The displayed rule resolves a tied vote in favour of one; any fixed vote convention would also define the method. When $k=1$, this is the [one-nearest-neighbour classifier](../../../../../one-nearest-neighbour-classifier.md) $\widehat C_n^{1{\rm nn}}(x)=Y_{(1)}(x)$.

Write $I_n(x)$ for the selected original index. Conditional on all features $X_1,\ldots,X_n$, it is fixed, and $U_{I_n(x)}$ is still uniform on $[0,1]$. The two decisions being compared are

$$
\widehat C_n^{1{\rm nn}}(x)
=\mathbb1_{\{U_{I_n(x)}\leq\eta(X_{I_n(x)})\}},\qquad
\widetilde C_n^{1{\rm nn}}(x)
=\mathbb1_{\{U_{I_n(x)}\leq\eta(x)\}}.
$$

The latter is an oracle comparison rule: its relabeling is recomputed at each query $x$, rather than being a fixed relabeling of the [training data](../../../../../training-data.md) for all queries. For a variable $U$ with the [uniform distribution](../../../../../continuous-uniform-distribution.md) on $[0,1]$, the two threshold indicators at $r,s\in[0,1]$ differ exactly when $U$ lies between them, an interval of length $|r-s|$. This [Bernoulli coupling by a shared uniform random variable](../../../../../bernoulli-coupling-by-a-shared-uniform-random-variable.md) proves

$$
\boxed{\mathbb P\{\widetilde C_n^{1{\rm nn}}(x)\ne\widehat C_n^{1{\rm nn}}(x)\}
=\mathbb E|\eta(X_{(1)}(x))-\eta(x)|.}
$$

Take the test pair $(X,Y)$ [independent](../../../../../independent-random-variables.md) of the [training data](../../../../../training-data.md) and its auxiliary uniforms. Let $\mathcal T_n=\sigma((X_i,Y_i,U_i):1\leq i\leq n)$, and interpret $L(C)$ as [conditional misclassification risk](../../../../../conditional-misclassification-risk.md) given $\mathcal T_n$. The [tower property of conditional expectation](../../../../../law-of-total-expectation.md) gives $\mathbb E L(C)=\mathbb P(C(X)\ne Y)$. Conditional on the test feature $X=x$ and all training features, $\widetilde C_n^{1{\rm nn}}(x)$ and $Y$ are [independent](../../../../../independent-random-variables.md) variables with a [Bernoulli distribution](../../../../../bernoulli-distribution.md) of parameter $\eta(x)$. Consequently, for every $n$,

$$
\boxed{\mathbb E L(\widetilde C_n^{1{\rm nn}})
=\mathbb E[2\eta(X)\{1-\eta(X)\}].}
$$

This is an exact finite-sample equality, not merely a limit.

The two error indicators can differ only if the two [classifiers](../../../../../classifier.md) disagree, so

$$
\begin{aligned}
\left|\mathbb E L(\widehat C_n^{1{\rm nn}})
-\mathbb E L(\widetilde C_n^{1{\rm nn}})\right|
&\leq\mathbb P\{\widehat C_n^{1{\rm nn}}(X)\ne\widetilde C_n^{1{\rm nn}}(X)\}\\
&=\mathbb E|\eta(X_{(1)}(X))-\eta(X)|.
\end{aligned}
$$

The permitted nearest-neighbour approximation theorem states that the last [expected value](../../../../../expected-value.md) tends to zero for the feature-based selection rule. This establishes the [one-nearest-neighbour asymptotic risk](../../../../../one-nearest-neighbour-asymptotic-risk.md)

$$
\boxed{\lim_{n\to\infty}\mathbb E L(\widehat C_n^{1{\rm nn}})
=\lim_{n\to\infty}\mathbb E L(\widetilde C_n^{1{\rm nn}})
=\mathbb E[2\eta(X)\{1-\eta(X)\}].}
$$

For $r\in[0,1]$, put $a=\min(r,1-r)\in[0,1/2]$. Then $2r(1-r)=2a(1-a)$, and $a\leq2a(1-a)\leq2a$. Integrating gives the [Bayes risk bound for one-nearest-neighbour classification](../../../../../bayes-risk-bound-for-one-nearest-neighbour-classification.md)

$$
\boxed{R^*\leq\lim_{n\to\infty}\mathbb E L(\widehat C_n^{1{\rm nn}})\leq2R^*.}
$$

Thus a [one-nearest-neighbour classifier](../../../../../one-nearest-neighbour-classifier.md) need not achieve the [Bayes risk](../../../../../bayes-risk.md): for constant $\eta=1/4$, its limiting [misclassification risk](../../../../../misclassification-risk.md) is $3/8$, while $R^*=1/4$.

**Feature-based neighbour tie-breaking is required.** The convention cannot be dropped for arbitrary $P_X$. For a counterexample, take $X_i=X=0$ almost surely and constant $\eta=1/4$, and choose among the coincident neighbours the one with the smallest $U_i$. Then the predicted label is one with [probability](../../../../../probability.md) $1-(3/4)^n$, so its [misclassification risk](../../../../../misclassification-risk.md) tends to $3/4$, exceeding the claimed upper bound $2R^*=1/2$. The corrected theorem uses ties determined independently of the uniforms and labels, as above.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
