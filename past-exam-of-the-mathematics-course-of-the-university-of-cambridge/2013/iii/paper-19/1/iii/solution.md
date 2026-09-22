<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\theta=\xi^*$, and work with the set structure $V_\theta\models\mathrm{ZFC}$. Its [ordinal](../../../../../../ordinal.md) height is an infinite limit: a [transitive model](../../../../../../transitive-model.md) of [ZFC](../../../../../../zermelo-fraenkel-set-theory-with-choice.md) has no largest [ordinal](../../../../../../ordinal.md), since it can take the successor of each [ordinal](../../../../../../ordinal.md) it contains. Thus $\operatorname{cf}(\theta)\ge\omega$.

Suppose instead that $\operatorname{cf}(\theta)>\omega$. Enumerate all [first-order formulas](../../../../../../first-order-formula.md), and close each finite initial collection under subformulas. Applying [Lévy reflection theorem](../../../../../../levy-reflection-theorem.md) inside $V_\theta$, choose a strictly increasing sequence $\beta_m<\theta$ such that $V_{\beta_m}$ agrees with $V_\theta$ on the first $m$ collections. Take $\eta=\sup_m\beta_m<\theta$. The internal rank levels here are the actual rank levels, because $V_\theta$ is a transitive rank model.

If $V_\theta\models\exists x\,\psi(x,\vec a)$ with $\vec a\in V_\eta$, choose $m$ large enough to include this formula and all the parameters in $V_{\beta_m}$. Reflection supplies a witness in $V_{\beta_m}\subseteq V_\eta$. The [Tarski-Vaught test](../../../../../../tarski-vaught-test.md) therefore gives $V_\eta\prec V_\theta$. In particular $V_\eta$ satisfies all of [ZFC](../../../../../../zermelo-fraenkel-set-theory-with-choice.md), contrary to the minimality of $\theta$.

Consequently

$$
\boxed{\operatorname{cf}(\xi^*)=\omega.}
$$

The countable enumeration is of formulas, not merely axioms: witness closure is what makes the union a model of the entire theory.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
