<h1 id="n/n1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Two states lie in the same [communicating class](../../../../../communicating-class.md) when each is reachable from the other by transitions of positive probability. Inspecting the directed transitions gives **three classes**:

$$
\{1\},\qquad\{2,3,6,7\},\qquad\{4,5,8\}.
$$

State 1 has no incoming transition from another state and can leave, so its singleton class is open and transient. More explicitly, the probability of returning to 1 after time zero is only $0.1$, since a departure can never be reversed.

States $2,3,6,7$ communicate: $2\to3\to7\to2$ and $2\to6\to7$ are positive-probability paths. The class is open because, for example, $2\to8$ and $6\to4$ leave it; no transition from the class $\{4,5,8\}$ returns to it. Every state of $\{2,3,6,7\}$ is transient. One can see eventual exit directly: from each of its four states there is a positive-probability path of at most three steps to 8; the minimum of these four path probabilities is positive, so survival through repeated three-step blocks has a geometrically decreasing upper bound.

Finally $4\to8\to5\to4$ shows that $\{4,5,8\}$ communicates, and every outgoing transition stays inside it. It is a closed finite irreducible class, so all its states are positive recurrent. Therefore **the first two classes are open and transient; the last is closed and recurrent**.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [N1](../../n1.md)
3. [N](../../../n.md)
4. [2006](../../../../2006-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
