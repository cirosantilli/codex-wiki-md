<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [Herbrand interpretation](../../../../../herbrand-structure.md) $I$ is a [stable model](../../../../../stable-model.md) when it is the [least Herbrand model](../../../../../least-herbrand-model.md) of its [stable model reduct](../../../../../stable-model-reduct.md) $\mathcal K^I$. To form the reduct, ground the rules, delete each rule with a premise $\operatorname{not}A$ for which $A\in I$, and remove the remaining occurrences of `not` and their atoms.

For $\mathcal I_1$, the rules concerning $N$ in the reduct are

$$
\begin{aligned}
\mathit{Year}(N)\land\mathit{DivisibleBy}(N,400)&\to\mathit{Leap}(N),\\
\mathit{Year}(N)\land\mathit{DivisibleBy}(N,4)&\to\mathit{Leap}(N),\\
\mathit{Year}(N)&\to\mathit{Common}(N),
\end{aligned}
$$

together with $\mathit{Year}(N)$. No rule has a divisibility atom in its head, so [forward chaining](../../../../../forward-chaining.md) produces no divisibility facts and no leap fact. Ground rules for the other constants cannot fire because their year premises are absent. Thus

$$
\operatorname{LM}(\mathcal K^{\mathcal I_1})=\{\mathit{Year}(N),\mathit{Common}(N)\}=\mathcal I_1.
$$

Therefore $\boxed{\mathcal I_1\text{ is stable}}$.

For $\mathcal I_2$, the rule using $\operatorname{not}\mathit{DivisibleBy}(N,100)$ is deleted. The common-year rule is retained without its negative premise, since $\mathit{Leap}(N)$ is absent. Crucially, the reduct does not convert atoms already in $\mathcal I_2$ into facts. Its [least Herbrand model](../../../../../least-herbrand-model.md) is again $\{\mathit{Year}(N),\mathit{Common}(N)\}$. The two divisibility atoms in $\mathcal I_2$ have no support. Hence

$$
\boxed{\mathcal I_2\text{ is not stable}.}
$$

Inspecting these two interpretations alone is not sufficient for [skeptical entailment](../../../../../skeptical-entailment.md). That requires every [stable model](../../../../../stable-model.md) to contain $\mathit{Common}(N)$. Here we can finish the argument: every reduct has no rule deriving divisibility atoms, so every [stable model](../../../../../stable-model.md) has empty divisibility relation. Its leap relation must then be empty as well. The common-year rule consequently derives $\mathit{Common}(N)$, and the only year fact is $\mathit{Year}(N)$. Thus $\mathcal I_1$ is the unique [stable model](../../../../../stable-model.md), and

$$
\boxed{\mathcal K\mathrel{\vert\!\approx}\mathit{Common}(N).}
$$

This final uniqueness argument, rather than the examination of just two candidate interpretations, establishes the required universal claim.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Knowledge representation and reasoning](../../../knowledge-representation-and-reasoning-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
