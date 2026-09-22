<h1 id="a/3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For each term $t$ define an $L_2$-formula $E_t(z)$ expressing its value. Use fresh [bound variables](../../../../../../bound-variable.md) at every step:

$$
E_x(z):=(z=x),\qquad E_c(z):=Q(z),\qquad E_{f(t)}(z):=\exists y\,[E_t(y)\land P(y,z)].
$$

Freshness includes avoiding all relevant [free variables](../../../../../../free-variable.md) of the formula being translated. Define the atomic translation by

$$
\sigma(t_1=t_2):=\exists u\exists v\,[E_{t_1}(u)\land E_{t_2}(v)\land u=v],
$$

and extend through the logical operations: $\sigma(\neg\theta)=\neg\sigma(\theta)$, $\sigma(\theta\to\eta)=\sigma(\theta)\to\sigma(\eta)$, and $\sigma(\forall x\theta)=\forall x\sigma(\theta)$. Fresh witnesses prevent variable capture and ensure the translation preserves the original free-variable [set](../../../../../../set-split.md).

For an $L_1$-structure $A$, let $A^r$ have the graph relation of $f^A$ and [singleton](../../../../../../singleton-mathematics.md) relation $\{c^A\}$. Induction on terms proves that $E_t(z)$ holds precisely when $z$ is the value of $t$. Induction on formulas then proves

$$
A,s\models\alpha\quad\Longleftrightarrow\quad A^r,s\models\sigma(\alpha).
$$

Conversely every $L_2$-structure satisfying $\phi,\psi$ is uniquely the relational version of an $L_1$-structure on that same domain. Hence, for arbitrary possibly infinite $\Gamma$, [semantic entailment](../../../../../../semantic-entailment.md) on the left is equivalent to [semantic entailment](../../../../../../semantic-entailment.md) from $\sigma(\Gamma)\cup\{\phi,\psi\}$ on the right, with assignments retained in the free-formula case. Applying [soundness theorem for first-order logic](../../../../../../soundness-theorem-for-first-order-logic.md) and [Gödel's completeness theorem](../../../../../../godel-s-completeness-theorem.md) gives

$$
\boxed{\Gamma\vdash\alpha\quad\Longleftrightarrow\quad\sigma(\Gamma)\cup\{\phi,\psi\}\vdash\sigma(\alpha).}
$$

The prohibition on completeness in the preceding direct equality question is local to that proof; here it supplies the clean semantic-to-syntactic transfer after the actual translation and model correspondence have been established.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the logic and set theory course of the University of Oxford](../../../../../split.md)
7. [Logic and set theory course of the University of Oxford](../../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
