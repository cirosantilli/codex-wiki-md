<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [Bayesian confirmation](../../../bayesian-confirmation.md) account can dissolve the apparent conflict between logical equivalence and ordinary judgements about relevant evidence. It does so by rejecting an unrestricted positive-instance rule and specifying how the evidence was sampled. [Bayes' theorem](../../../bayes-theorem.md) alone does not guarantee that every white shoe is irrelevant, or that every black [raven](../../../raven.md) provides strong support.

Let $H$ assert that every [raven](../../../raven.md) is black. Its contrapositive is [logically equivalent](../../../logical-equivalence.md) to $H$, so the two descriptions must receive the same [conditional probability](../../../conditional-probability.md). The [raven paradox](../../../raven-paradox.md) arises if every positive instance of a universal statement automatically confirms it: a white nonraven then confirms the contrapositive and hence $H$. The disputed step is that unrestricted confirmation rule, not the logical equivalence.[section 5: equivalence and the paradoxes of instance confirmation](../../../studies-in-the-logic-of-confirmation-i-by-carl-hempel.md)

For background $K$, set $p=P(H\mid K)$, $a=P(E\mid H,K)$ and $b=P(E\mid\neg H,K)$. For $0<p<1$ and positive evidence probability,

$$
P(H\mid E,K)=\frac{pa}{pa+(1-p)b}>p\quad\Longleftrightarrow\quad a>b.
$$

Thus it is the comparison of [likelihoods](../../../likelihood-function.md), including the sampling protocol and alternatives, that determines support. Merely rewriting $H$ cannot change it.

The [finite-population model of raven confirmation](../../../finite-population-model-of-raven-confirmation.md) makes the intuitive difference quantitative. Fix $r$ ravens and $M$ nonblack objects. Compare an all-black-ravens hypothesis with the alternative that exactly one raven is nonblack. A uniform draw among nonblack objects that finds a nonraven has [likelihood ratio](../../../likelihood-ratio.md) $1/(1-1/M)$. A uniform draw among ravens that finds a black one has [likelihood ratio](../../../likelihood-ratio.md) $1/(1-1/r)$. If $M\gg r>1$, the former is much nearer one. With equal [prior probabilities](../../../prior-probability.md), $M=10^6$ and $r=100$ give posterior probabilities approximately $0.50000025$ and $0.50251256$. A tiny amount of confirmation need have no practical significance.

This example is not a theorem about every possible background. Inspecting an object already known to be a white shoe adds no relevant information about its being a nonraven. Other alternatives or selection mechanisms change the likelihoods and can remove or reverse the support. Conditioning only on the observed colour while silently changing how the object was selected would compare different experiments.[Introduction and the treatment of background-sensitive confirmation; the finite model here is stated separately](../../../how-bayesian-confirmation-theory-handles-the-paradox-of-the-ravens-by-branden-fitelson-and-james-hawthorne.md)

The resolution is therefore qualified. A coherent probability model preserves equivalence and explains why superficially parallel observations need carry radically different evidence. It does not select a unique prior or sampling model without scientific judgement. Those remaining modelling questions are limitations of an application, rather than a contradiction in [Bayesian inference](../../../bayesian-statistics-split.md).

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2019](../../2019-split.md)
3. [Past exam of the philosophy of science supplementary subject of the University of Oxford](../../split.md)
4. [Philosophy of science supplementary subject of the University of Oxford](../../../philosophy-of-science-supplementary-subject-of-the-university-of-oxford.md)
5. [Supplementary subject of the physics course of the University of Oxford](../../../supplementary-subject-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
