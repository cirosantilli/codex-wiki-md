<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $q_0=\operatorname{create}()$ and $e=\text{Empty queue}$. The [axiomatic specification](../../../../../axiomatic-specification.md) starts with

$$
\begin{aligned}
\operatorname{empty}(q_0)&=\mathrm{true},\\
\operatorname{empty}(\operatorname{add}(i,q))&=\mathrm{false},\\
\operatorname{head}(q_0)&=\operatorname{err}_I(e),\\
\operatorname{delete}(q_0)&=\operatorname{err}_Q(e).
\end{aligned}
$$

For insertion at the tail, the head laws are

$$
\operatorname{head}(\operatorname{add}(i,q))=
\begin{cases}
\operatorname{ok}_I(i),&\operatorname{empty}(q),\\
\operatorname{head}(q),&\neg\operatorname{empty}(q).
\end{cases}
$$

The deletion laws are

$$
\operatorname{delete}(\operatorname{add}(i,q))=
\begin{cases}
\operatorname{ok}_Q(q_0),&\operatorname{empty}(q),\\
\operatorname{ok}_Q(\operatorname{add}(i,q')), &\neg\operatorname{empty}(q)\text{ and }\operatorname{delete}(q)=\operatorname{ok}_Q(q').
\end{cases}
$$

Require that queues are generated from `create` by finitely many `add` operations, with the usual equality of indistinguishable queue values. Induction on that construction ensures that the nonempty deletion case supplies a successful queue result, so the last law is well-typed and covers all nonempty queues.

These equations express the behavior of a [FIFO queue](../../../../../fifo-queue.md): adding to a nonempty queue changes neither its existing head nor the order of its remaining items. As a consistency model, interpret $Q$ as finite sequences, `create` as the empty sequence, `add` as append, and successful `head`/`delete` as first-element/tail operations. This model satisfies every displayed law and distinguishes error messages from ordinary items.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
