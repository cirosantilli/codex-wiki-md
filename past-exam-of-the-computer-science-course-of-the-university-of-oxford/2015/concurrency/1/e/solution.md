<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The obstruction is that the property is about where a transition originates, whereas the three standard [CSP semantic models](../../../../../csp-semantic-model.md) identify processes that can disagree about this fact. Take fresh $h\ne a$ and compare

$$
G=a\to\mathrm{STOP},\qquad B=\bigl(a\to\mathrm{STOP}\mathbin\square h\to a\to\mathrm{STOP}\bigr)\setminus\{h\}.
$$

In $G$, the only $a$ transition leaves a [CSP stable state](../../../../../csp-stable-state.md), so the property holds. Initially $B$ has both an $a$ transition to $\mathrm{STOP}$ and a [CSP internal action](../../../../../csp-internal-action.md) to $a\to\mathrm{STOP}$. Its initial state is therefore not a [CSP stable state](../../../../../csp-stable-state.md), and its direct $a$ transition violates the property.

Nevertheless both have exactly the [CSP traces](../../../../../csp-trace.md) $\langle\rangle$ and $\langle a\rangle$. Initially their possible stable observations offer exactly $a$, so their initial [CSP stable failures](../../../../../csp-stable-failure.md) are precisely $(\langle\rangle,X)$ with $a\notin X$. After $a$, both can refuse every [CSP event](../../../../../csp-event.md). Neither has a [CSP divergence](../../../../../csp-divergence.md): the hidden $h$ can occur at most once. Therefore

$$
\boxed{G=_T B,\quad G=_F B,\quad G=_{FD}B,\qquad\text{but the property separates }G\text{ and }B.}
$$

No [CSP refinement](../../../../../csp-refinement.md) test in one of these models can separate semantically equal operands. This also rules out placing the operand in a fixed context of ordinary CSP operators before the test, since those operators respect the model's equality. A model recording more about the interleaving of stability and acceptance, or an additional operator that explicitly observes stability, would be needed.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Concurrency](../../../concurrency-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
