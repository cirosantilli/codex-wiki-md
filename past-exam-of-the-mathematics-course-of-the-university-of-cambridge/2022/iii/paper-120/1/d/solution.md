<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Soundness follows by induction on derivations: assumptions are forced by hypothesis, implication introduction uses the definition of [Kripke forcing relation](../../../../../../kripke-forcing-relation.md), and implication elimination uses it at the current world.

For completeness, form the [canonical Kripke model for implicational intuitionistic logic](../../../../../../canonical-kripke-model-for-implicational-intuitionistic-logic.md). Its worlds are [deductively closed](../../../../../../deductively-closed-set-of-formulae.md) implicational theories $\Delta$ extending $\operatorname{Cn}(\Gamma)$, ordered by inclusion, and

$$
\Delta\Vdash p\quad\Longleftrightarrow\quad p\in\Delta
$$

for each atom $p$. We prove the truth lemma

$$
\Delta\Vdash\alpha\quad\Longleftrightarrow\quad\alpha\in\Delta
$$

by induction on implicational formulas. The atomic case is the definition. For $\alpha\to\beta$, membership implies forcing by closure under implication elimination. Conversely, if $\alpha\to\beta\notin\Delta$, the implication-introduction rule shows that $\operatorname{Cn}(\Delta\cup\{\alpha\})$ does not contain $\beta$; this extension forces $\alpha$ but not $\beta$, so $\Delta$ does not force $\alpha\to\beta$.

If $\Gamma\nvdash_{\mathrm{IPC}(\to)}\varphi$, the root $\operatorname{Cn}(\Gamma)$ of this canonical model forces every member of $\Gamma$ but does not force $\varphi$. Together with soundness, this proves [Kripke completeness of implicational intuitionistic logic](../../../../../../kripke-completeness-of-implicational-intuitionistic-logic.md).

Finally suppose the implicational formulas $\Gamma$ and $\varphi$ satisfy $\Gamma\vdash_{\mathrm{IPC}}\varphi$. The [soundness theorem for propositional logic](../../../../../../soundness-theorem-for-propositional-logic.md) for intuitionistic Kripke semantics gives $\Gamma\models_{\mathrm{Kripke}}\varphi$, and the completeness just proved gives $\Gamma\vdash_{\mathrm{IPC}(\to)}\varphi$. This is the [conservativity of intuitionistic propositional logic over its implicational fragment](../../../../../../conservativity-of-intuitionistic-propositional-logic-over-its-implicational-fragment.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
