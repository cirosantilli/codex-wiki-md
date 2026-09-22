<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $J_A(P,Q)=P\mathbin\triangle_AQ$. The following five [CSP operational semantics](../../../../../csp-operational-semantics.md) rules suffice, with $a$ always visible:

$$
\frac{P\xrightarrow{\tau}P'}{J_A(P,Q)\xrightarrow{\tau}J_A(P',Q)}\qquad
\frac{Q\xrightarrow{\tau}Q'}{J_A(P,Q)\xrightarrow{\tau}J_A(P,Q')},
$$



$$
\frac{P\xrightarrow aP'\quad a\notin A}{J_A(P,Q)\xrightarrow aJ_A(P',Q)}\qquad
\frac{Q\xrightarrow aQ'\quad a\notin A}{J_A(P,Q)\xrightarrow aQ'},
$$



$$
\boxed{\frac{P\xrightarrow aP'\quad Q\xrightarrow aQ'\quad a\in A}{J_A(P,Q)\xrightarrow aJ_A(P',Q')}.}
$$

Thus a [CSP internal action](../../../../../csp-internal-action.md) of either operand preserves the wrapper. A visible action outside $A$ by the left operand also preserves it, whereas such an action by the right operand performs an ordinary [CSP interrupt](../../../../../csp-interrupt.md) and discards the left operand. An action in $A$ requires both operands and advances both without discarding either. If both can perform the same event outside $A$, there are two transitions with the same visible label and potentially different derivatives; neither should be deleted. The paper excludes successful termination, so no extra termination rules are needed.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Concurrency](../../../concurrency-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
