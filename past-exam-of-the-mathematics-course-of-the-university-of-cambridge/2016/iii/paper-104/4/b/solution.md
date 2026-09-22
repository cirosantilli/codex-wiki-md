<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If the [Turing machine](../../../../../../turing-machine.md) halts on $w$, follow its computation from $hq_1wh$. A transition at an already represented cell is one of the corresponding relations. At a boundary, first insert the required blank using a padding relation. Thus the computation gives a finite equality derivation to $huq_0vh$. Replace $q_0$ by $q$, erase the symbols of $u,v$ using $s_jq=q=qs_j$, and erase both boundary markers. This proves $hq_1wh=q$ in the [semigroup](../../../../../../semigroup.md).

For the converse, equality in a presented [semigroup](../../../../../../semigroup.md) means a finite sequence of contextual replacements using defining relations in either direction. In any derivation from $hq_1wh$ to $q$, consider the first occurrence of the special symbol $q$. Before it occurs, the erasure relations cannot be used in either direction. Each word therefore still has exactly two markers $h$, exactly one state letter, and the form $huq_i vh$. Both directions of a transition relation join configurations linked by one actual machine step; both directions of a boundary-padding relation merely change how much blank tape is represented.

The first occurrence of $q$ must come from $q_0=q$ in the forward direction. Hence the initial configuration is connected, by transitions in either direction and harmless padding, to a configuration in state $q_0$. For a deterministic [Turing machine](../../../../../../turing-machine.md), the property of eventually reaching $q_0$ is invariant along each transition edge: if $C\to D$ is a step, then $C$ halts if and only if $D$ halts, since that step is the unique next step of $C$ and $C$ is not already in the halting state. The same property is unchanged by padding. A finite path of these edges to $q_0$ therefore shows that the initial configuration halts.

Consequently

$$
\boxed{w\in\Omega(T)\quad\Longleftrightarrow\quad hq_1wh=q\text{ in }\Gamma(T).}
$$

The invariance argument is necessary because equality in a [semigroup presentation](../../../../../../semigroup-presentation.md) allows reversed transitions as well as forward computation steps.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 104](../../../paper-104-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
