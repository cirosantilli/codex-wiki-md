<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The external [necessitation rule](../../../../../necessitation-rule.md) assertion is valid.** Suppose $PA\vdash X$ and fix a proof code $m$. If $PA$ is inconsistent the assertion follows by explosion. Otherwise there is no actual proof of $\neg X$. Each of the finitely many bounded checks up to $m$ is therefore a true bounded [arithmetic](../../../../../arithmetic-split.md) fact and is provable. Together with the positive proof check at $m$ this gives

$$
\boxed{PA\vdash X\ \Longrightarrow\ PA\vdash R(\ulcorner X\urcorner).}
$$

**The requested internal modus-ponens assertion needs an additional coding property.** Combining a proof of $X$ and a proof of $X\to Y$ produces a proof of $Y$, but its code can exceed both original codes. The two Rosser hypotheses exclude proofs of $\neg X$ and $\neg(X\to Y)$ only up to their respective witness bounds. They provide no bound excluding proofs of $\neg Y$ below the new proof code. Ordinary internal [modus ponens rule](../../../../../implication-elimination-rule.md) for the unbounded provability predicate does not fill this gap.

Consequently the premises printed here do not, just by themselves, justify

$$
R(\ulcorner X\to Y\urcorner)\to(R(\ulcorner X\urcorner)\to R(\ulcorner Y\urcorner)).
$$

This property varies with the [Rosser proof-order dependence](../../../../../rosser-proof-order-dependence.md): some specially chosen proof predicates satisfy it, while general Rosser proof predicates need not. [Provability Logic, printed page 87: dependence of Rosser [modus ponens rule](../../../../../implication-elimination-rule.md) on proof numbering](https://sartemov.ws.gc.cuny.edu/files/2012/10/Artemov-Beklemishev.-Provability-logic.pdf).

The reference to a proof predicate “as given in the course” would need an explicit additional proof-order lemma to establish this part for that particular coding. Standard correctness on numeral instances and the ordinary [Hilbert-Bernays-Löb derivability conditions](../../../../../hilbert-bernays-lob-derivability-conditions.md) alone are insufficient. The next solution gives the intended argument with the missing condition stated explicitly.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
