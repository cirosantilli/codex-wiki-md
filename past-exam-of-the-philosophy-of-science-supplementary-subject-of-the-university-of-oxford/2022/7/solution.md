<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

[Scientific confirmation](../../../scientific-confirmation.md) is evidential support rather than deductive proof. Two distinct problems concern, first, what counts as relevant positive evidence and, second, which part of a tested theoretical package that evidence supports. A defensible response makes background information and the production of evidence explicit. The following two problems are independent: resolving the logical puzzle about positive instances does not eliminate ambiguity about [auxiliary hypotheses](../../../auxiliary-hypothesis.md).

**Problem one: the [raven paradox](../../../raven-paradox.md).** Write the hypothesis as

$$
H:\quad\forall x\,(R(x)\Rightarrow B(x)),
$$

where $R$ means “is a raven” and $B$ “is black”. Its [contrapositive](../../../contrapositive.md) is

$$
\forall x\,(\neg B(x)\Rightarrow\neg R(x)).
$$

The hypotheses are [logically equivalent](../../../logical-equivalence.md). A plausible equivalence principle says that identical information must support them equally. A plausible instance principle says that an observed $F$ that is $G$ confirms “every $F$ is $G$”. Combining the principles makes a nonblack nonraven, such as a white shoe, support the raven hypothesis. That conflicts with the intuition that inspecting shoes tells us nothing about ravens. [Hempel](../../../carl-gustav-hempel.md) develops the puzzle in his analysis of instance-based [scientific confirmation](../../../scientific-confirmation.md).[section 5: equivalence, Nicod's criterion and the paradoxical confirming instances](../../../studies-in-the-logic-of-confirmation-i-by-carl-hempel.md)

My preferred response retains logical equivalence while rejecting an unconditional instance rule. By [Bayes' theorem](../../../bayes-theorem.md), for evidence $E$, background $K$ and positive relevant [probabilities](../../../probability.md),

$$
\boxed{P(H\mid E,K)>P(H\mid K)\quad\Longleftrightarrow\quad P(E\mid H,K)>P(E\mid\neg H,K).}
$$

An instance's bearing depends on how likely it was under the competing possibilities, including how the object was selected. No rule depending only on the grammatical form of an instance can settle that comparison. [Branden Fitelson](../../../branden-fitelson.md) and [James Hawthorne](../../../james-hawthorne.md) analyse the role of background assumptions and [Bayesian confirmation](../../../bayesian-confirmation.md) in this puzzle.[opening sections on the equivalence condition, versions of Nicod's condition and background evidence](../../../how-bayesian-confirmation-theory-handles-the-paradox-of-the-ravens-by-branden-fitelson-and-james-hawthorne.md)

Here is an explicit illustrative model. There are 100 labelled objects: ten known ravens and ninety known nonravens. Under $H$ all ten ravens are black; under the sole alternative $A$, exactly one of the ten is nonblack, with its identity uniformly distributed. Nonraven colours are already known and identical under both possibilities, and the [prior probabilities](../../../prior-probability.md) of $H,A$ are equal. Selecting a known white shoe according to a rule independent of $H,A$ has the same [likelihood](../../../likelihood-function.md) under each, so the [posterior probability](../../../posterior-probability.md) of $H$ stays $1/2$. A uniformly selected raven, however, is black with [probability](../../../probability.md) $1$ under $H$ and $9/10$ under $A$. After observing it to be black,

$$
P(H\mid\text{black selected raven})=\frac{1}{1+9/10}=\frac{10}{19}>\frac12.
$$

If sampling is instead from known nonblack objects whose membership is uncertain, discovering a nonraven can rule out a possible counterexample and provide support. There is no context-independent prohibition on support from a nonraven. The response explains both the familiar irrelevance intuition and why it is not universally correct. Its limit is that the [prior probabilities](../../../prior-probability.md) and sampling assumptions need independent defence; the calculation is a transparent model, not a theorem that all shoes are irrelevant.

**Problem two: the [Duhem problem](../../../duhem-problem.md) of testing a package.** Suppose the target hypothesis $T$ and [auxiliary hypotheses](../../../auxiliary-hypothesis.md) $A$ jointly imply an outcome $E$:

$$
T\land A\Rightarrow E.
$$

A failure gives $\neg(T\land A)$, equivalently $\neg T\lor\neg A$, rather than $\neg T$ alone. Success also does not establish either premise: that would affirm the consequent. [Pierre Duhem](../../../pierre-duhem.md)'s point is especially pressing for physical experiments whose predictions require theories of the apparatus as well as the target system.[part II, chapter VI, section 2: an experiment tests a theoretical group rather than an isolated hypothesis](../../../the-aim-and-structure-of-physical-theory-by-pierre-duhem.md)

My preferred response combines independent calibration, deliberately varied tests and explicit comparison of packages. For a simple model, suppose a detector has independently calibrated false-positive [probability](../../../probability.md) $f$ and detection efficiency $d$. A target predicts a signal on each trial with [probability](../../../probability.md) $s$. Then the positive-output [probability](../../../probability.md) is

$$
p_T=sd+(1-s)f.
$$

Under a no-signal rival it is $p_0=f$. If $s=1/2$, $d=9/10$, and $f=1/10$, then $p_T=1/2$. One positive reading supplies a [Bayes factor](../../../bayes-factor.md) of $5$ for the specified target package against the specified no-signal package. But an uncalibrated faulty detector with false-positive [probability](../../../probability.md) $1/2$ fits the same positive-reading rate. Target data alone do not distinguish those packages.

Signal-absent calibration trials test the false-positive assumption directly. If ten independent such trials are all negative, their [likelihood ratio](../../../likelihood-ratio.md) in favour of $f=1/10$ against $f=1/2$ is

$$
\boxed{\frac{(9/10)^{10}}{(1/2)^{10}}=\left(\frac95\right)^{10}\simeq357.05.}
$$

This does not magically isolate $T$: the calibration relies on its own assumptions, and correlated trials would invalidate the power calculation. It shows concretely how additional evidence can discriminate explanations that the initial data leave unresolved. Repeating the target measurement with apparatus based on different physical processes further reduces dependence on one shared failure mode.

Thus the [Duhem problem](../../../duhem-problem.md) defeats automatic attribution of support or failure, not rational experimental comparison. Where rivals remain [empirically equivalent](../../../empirical-equivalence.md), suspension of judgement about their difference is appropriate. Together, the two responses defend [scientific confirmation](../../../scientific-confirmation.md) as a structured, fallible comparison using background information, rather than either pure instance counting or a mechanical verdict on an isolated hypothesis.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2022](../../2022-split.md)
3. [Past exam of the philosophy of science supplementary subject of the University of Oxford](../../split.md)
4. [Philosophy of science supplementary subject of the University of Oxford](../../../philosophy-of-science-supplementary-subject-of-the-university-of-oxford.md)
5. [Supplementary subject of the physics course of the University of Oxford](../../../supplementary-subject-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
