<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the distributive law of [Boolean algebra](../../../../../boolean-algebra.md) to the two [logical conjunctions](../../../../../logical-conjunction.md). With $A=P$, $B=\neg Q$, $C=\neg P$, and $D=Q$, the identity $(A\land B)\lor(C\land D)\equiv(A\lor C)\land(A\lor D)\land(B\lor C)\land(B\lor D)$ gives

$$
\begin{aligned}
(P\land\neg Q)\lor(\neg P\land Q)
&\equiv(P\lor\neg P)\land(P\lor Q)\land(\neg Q\lor\neg P)\land(\neg Q\lor Q)\\
&\equiv\top\land(P\lor Q)\land(\neg P\lor\neg Q)\land\top\\
&\equiv\boxed{(P\lor Q)\land(\neg P\lor\neg Q).}
\end{aligned}
$$

The second step uses complementation and commutativity in [Boolean algebra](../../../../../boolean-algebra.md); the last uses the identity law for [logical conjunction](../../../../../logical-conjunction.md). The result is in [conjunctive normal form](../../../../../conjunctive-normal-form.md): its first [Boolean clause](../../../../../clause-of-a-boolean-formula.md) requires at least one input to be true, and its second [Boolean clause](../../../../../clause-of-a-boolean-formula.md) prohibits both inputs being true. Together they express [exclusive or](../../../../../exclusive-or.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Logic and proof](../../../logic-and-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
