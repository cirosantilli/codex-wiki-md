<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

To apply [bounded model checking](../../../../../bounded-model-checking.md), seek an initial [path in a transition system](../../../../../path-in-a-transition-system.md) satisfying

$$
\mathrm{fair}\land\neg\varphi_1
\equiv GF\neg(a\land b)\land GF\neg a.
$$

A [satisfying assignment](../../../../../satisfying-assignment.md) for its bounded encoding is enough to disprove the specification. Use a [lasso path](../../../../../lasso-path.md): positions $q_0,\ldots,q_k$ follow the [transition relation](../../../../../transition-relation.md), and a final arrow returns from $q_k$ to some $q_\ell$, $0\leq\ell\leq k$. The repeated part is $q_\ell\cdots q_k$. On such a [lasso path](../../../../../lasso-path.md), $GF r$ is equivalent to having $r$ true at some position of the repeated part.

For this example an explicit [Boolean formula](../../../../../boolean-formula.md) for the bounded search is

$$
\begin{aligned}
E_k={}&I(q_0)\land\bigwedge_{i=0}^{k-1}T(q_i,q_{i+1})\\
&\land\bigvee_{\ell=0}^{k}\left(
T(q_k,q_\ell)
\land\bigvee_{i=\ell}^{k}\neg(a(q_i)\land b(q_i))
\land\bigvee_{i=\ell}^{k}\neg a(q_i)
\right).
\end{aligned}
$$

Here $I(q)$ means $q\in\{s_0,s_3\}$ and $T(q,r)$ means that the source diagram has the arrow $q\to r$; each can be encoded by finite [Boolean variables](../../../../../boolean-variable.md) for the [states](../../../../../state-computer-science.md). The loop requirements are the [fairness assumption](../../../../../fairness-assumption.md) and the negated specification respectively. Unrolling the [transition relation](../../../../../transition-relation.md) and adding a loop closure is the usual [bounded model checking](../../../../../bounded-model-checking.md) construction.[§2, worked example with an unrolled transition relation and a returning loop; §3, infinite-path semantics](../../../../../symbolic-model-checking-without-bdds-by-armin-biere-and-others.md)

At bound $k=0$, an initial [self-loop](../../../../../loop-graph-theory.md) would be needed. The only such choice is $q_0=s_3$, whose repeated label satisfies $a\land b$ and $a$. It violates both loop requirements. The other initial [state](../../../../../state-computer-science.md), $s_0$, has no [self-loop](../../../../../loop-graph-theory.md). Thus $E_0$ has no [satisfying assignment](../../../../../satisfying-assignment.md).

At bound $k=1$, choose

$$
\boxed{q_0=s_0,\qquad q_1=s_1,\qquad\ell=0.}
$$

Both required arrows $s_0\to s_1$ and $s_1\to s_0$ exist. At $q_1$, $a$ is false and hence $a\land b$ is false, so both repeated-part requirements are true. Equivalently, the label values are $a(q_0)=b(q_0)=b(q_1)=1$ and $a(q_1)=c(q_0)=c(q_1)=0$. These values give a [satisfying assignment](../../../../../satisfying-assignment.md) of $E_1$, representing the fair [counterexample](../../../../../counterexample.md) $(s_0s_1)^\omega$. Consequently

$$
\boxed{TS\not\models_{\mathrm{fair}}FGa.}
$$

Here the bound counts forward arrows before the returning arrow, so $k=1$ stores two positions and describes a two-[state](../../../../../state-computer-science.md) repeated part. There is no need for a completeness bound: the exhibited fair [counterexample](../../../../../counterexample.md) settles the negative answer. These [satisfying assignments](../../../../../satisfying-assignment.md) are checked directly; no claim of executing an external [SAT solver](../../../../../sat-solver.md) is needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Computer aided formal verification](../../../computer-aided-formal-verification-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
