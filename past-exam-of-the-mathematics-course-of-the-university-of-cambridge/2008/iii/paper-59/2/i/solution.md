<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Consider two spacelike-separated measurement regions $R_A$ and $R_B$, with locally chosen settings $a,b\in\{0,1\}$ and recorded outcomes $A,B\in\{-1,1\}$. A relevant past region supplies a sufficient specification $\lambda$ of the common preparation and other hidden physical information needed to screen the outcomes. This is not necessarily just a [quantum state](../../../../../../quantum-state.md) written at the source, nor a conditioning on arbitrary records which already contain the future choices. The spacetime shielding and sufficiency requirements are substantive causal assumptions.

Use [Bell local causality](../../../../../../bell-local-causality.md): once the relevant past is sufficiently specified, learning facts in the remote measurement region changes no local outcome probability. In particular, require

$$
P(A\mid a,b,B,\lambda)=P(A\mid a,\lambda),\qquad P(B\mid a,b,\lambda)=P(B\mid b,\lambda),
$$

where conditional probabilities are defined. The probability chain rule gives

$$
P(A,B\mid a,b,\lambda)=P(A\mid a,\lambda)P(B\mid b,\lambda).
$$

This factorization combines [parameter independence](../../../../../../parameter-independence.md) with [outcome independence](../../../../../../outcome-independence.md). Neither probability is required to be zero or one: the argument includes stochastic [local hidden-variable theories](../../../../../../local-hidden-variable-theory.md).

Also assume [measurement independence](../../../../../../measurement-independence.md), $\rho(\lambda\mid a,b)=\rho(\lambda)$, so all four setting pairs average over one normalized nonnegative past-variable distribution. This is a statistical condition on the setting procedure and relevant hidden information, not a proof of a metaphysical doctrine of free will. Finally the recorded outcomes must represent the same ensemble of trials. One can include nondetections in a specified bounded-outcome rule; if instead one discards events depending on setting or outcome, a further sampling assumption is required. Setting-dependent postselection is not covered silently by the argument.

Let $\alpha_a(\lambda)=\sum_A AP(A\mid a,\lambda)$ and $\beta_b(\lambda)=\sum_B BP(B\mid b,\lambda)$. They lie in $[-1,1]$, and the factorization gives

$$
E_{ab}=\int\rho(\lambda)\alpha_a(\lambda)\beta_b(\lambda)\,d\lambda.
$$

For each $\lambda$,

$$
|\alpha_0(\beta_0+\beta_1)+\alpha_1(\beta_0-\beta_1)|\le|\beta_0+\beta_1|+|\beta_0-\beta_1|=2\max(|\beta_0|,|\beta_1|)\le2.
$$

Averaging with the same $\rho$ proves the [CHSH inequality](../../../../../../chsh-inequality.md)

$$
\boxed{|E_{00}+E_{01}+E_{10}-E_{11}|\le2.}
$$

No separate assumption of simultaneous predetermined values for incompatible quantum [observables](../../../../../../observable.md) was needed. The common probability model and its screening relations did the work.

A [Reichenbach common cause principle](../../../../../../reichenbach-common-cause-principle.md) can motivate the same calculation: a complete classical common cause in the past screens the two outcomes, while each setting affects only its own wing. Together with setting-independent sampling this gives the displayed factorization. It is not enough to provide a different screening variable for each pair of settings: those constructions need not form one compatible common-cause model for the four correlations.

A [stochastic Einstein locality](../../../../../../stochastic-einstein-locality.md) formulation instead constrains objective chances by facts in the appropriate causal past. To use it as a sufficient premise here, specify both local dependence on settings and a joint screening condition for the two outcomes. Merely requiring local marginal chances not to depend on a remote setting gives [parameter independence](../../../../../../parameter-independence.md), which is weaker than factorization. Thus the precise stochastic locality version matters; one should not infer a [Bell inequality](../../../../../../bell-inequality.md) from every condition loosely described as no superluminal influence.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
