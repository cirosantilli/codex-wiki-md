<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

**The [Bell theorem](../../../bell-theorem.md) connects the philosophical problem of [scientific underdetermination](../../../scientific-underdetermination.md) with a precise issue in [quantum mechanics](../../../quantum-mechanics-split.md): whether local underlying causes can reproduce observed correlations.** It shows how a dispute about interpretation can acquire empirical content, while also showing why an [experiment](../../../experiment.md) does not select a unique ontology.

A shared cause can produce strong correlations without a signal between distant measurements. The philosophical question is whether this familiar explanatory strategy can reproduce all predictions for [quantum entanglement](../../../entangled-state.md). In a two-station [Bell test](../../../bell-test.md), let $x,y\in\{0,1\}$ be local settings and $A,B\in\{-1,1\}$ the outcomes. A [local hidden-variable theory](../../../local-hidden-variable-theory.md) satisfying [Bell local causality](../../../bell-local-causality.md) takes

$$
P(A,B\mid x,y,\lambda)
=P(A\mid x,\lambda)P(B\mid y,\lambda).
$$

[Measurement independence](../../../measurement-independence.md) additionally requires $\rho(\lambda\mid x,y)=\rho(\lambda)$. The same ensemble of underlying states must therefore apply across the four setting pairs.

The resulting [CHSH inequality](../../../chsh-inequality.md) can be derived without assuming quantum theory. First take a [deterministic local hidden-variable model](../../../deterministic-local-hidden-variable-model.md) with responses $A_0,A_1,B_0,B_1=\pm1$. For each $\lambda$,

$$
s(\lambda)=A_0(B_0+B_1)+A_1(B_0-B_1)=\pm2,
$$

because exactly one bracket vanishes. Averaging against one normalized [probability distribution](../../../probability-distribution-split.md) gives

$$
\boxed{|S|=|E_{00}+E_{01}+E_{10}-E_{11}|\leq2.}
$$

Stochastic local response functions give no escape: they can be represented by adding independent local random seeds to $\lambda$ and averaging deterministic assignments. The essential restriction is the common setting-independent ensemble and local dependence of responses, not a separate insistence that all nature be deterministic.

For two spin-one-half systems in a [spin singlet state](../../../spin-singlet-state.md), ideal [quantum measurements](../../../quantum-measurement-split.md) along unit directions $\mathbf a,\mathbf b$ give $E(\mathbf a,\mathbf b)=-\mathbf a\cdot\mathbf b$. Choose

$$
\mathbf a_0=\hat{\mathbf z},\qquad
\mathbf a_1=\hat{\mathbf x},\qquad
\mathbf b_0=\frac{\hat{\mathbf z}+\hat{\mathbf x}}{\sqrt2},\qquad
\mathbf b_1=\frac{\hat{\mathbf z}-\hat{\mathbf x}}{\sqrt2}.
$$

The four correlations are $-1/\sqrt2,-1/\sqrt2,-1/\sqrt2,+1/\sqrt2$, so $S=-2\sqrt2$. Thus [quantum mechanics](../../../quantum-mechanics-split.md) predicts an observable incompatibility with the specified [local hidden-variable theory](../../../local-hidden-variable-theory.md) class. This is stronger than saying that two interpretations happen to fit the observations collected so far.

Actual [Bell tests](../../../bell-test.md) require more than the ideal calculation. Setting choices and distant readouts must have the relevant [spacelike separation](../../../spacelike-separation.md); discarding detected pairs selectively can create a [detection loophole](../../../detection-loophole.md). The 2015 [Delft electron-spin Bell test](../../../delft-electron-spin-bell-test.md) combined efficient readout, rapid settings and separated stations to address these issues together. The reported statistic was $S=2.42\pm0.20$, with a test of the local-model hypothesis accounting for device memory.[abstract and experimental account: 1.3 km separation, 245 trials and the reported CHSH statistic](../../../experimental-loophole-free-violation-of-a-bell-inequality-by-bas-hensen-and-others.md) This is statistical evidence under a specified protocol, rather than a logically infallible observation.

The philosophical conclusion must be equally precise. A violation challenges the conjunction of [Bell local causality](../../../bell-local-causality.md), [measurement independence](../../../measurement-independence.md) and the relevant experimental assumptions. It does not disprove every possible hidden-variable account, or establish that the observer's mind creates the outcome. Different theories can reject different premises while agreeing on the observable correlations. That remaining [scientific underdetermination](../../../scientific-underdetermination.md) does not cancel the genuine exclusion of a well-defined class.

Nor does violating [Bell local causality](../../../bell-local-causality.md) entail controllable faster-than-light communication. In the ideal [spin singlet state](../../../spin-singlet-state.md), each local marginal is $P(A=+1\mid x,y)=1/2$, independently of the distant setting. This [quantum no-signalling](../../../quantum-no-signalling.md) condition is weaker than the hidden-state factorization used in the proof. Conflating them turns a precise result into an unwarranted conclusion about signalling.

The example therefore illustrates both the power and the limit of empirical testing in philosophy of science. Mathematical clarification can transform an apparently metaphysical disagreement into rival observational constraints. Evidence can discriminate those constraints without determining every question about the reality represented by a successful theory.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2021](../../2021-split.md)
3. [Past exam of the philosophy of science supplementary subject of the University of Oxford](../../split.md)
4. [Philosophy of science supplementary subject of the University of Oxford](../../../philosophy-of-science-supplementary-subject-of-the-university-of-oxford.md)
5. [Supplementary subject of the physics course of the University of Oxford](../../../supplementary-subject-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
