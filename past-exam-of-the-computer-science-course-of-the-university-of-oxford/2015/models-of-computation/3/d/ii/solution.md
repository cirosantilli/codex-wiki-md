<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**The problem is undecidable.** Reduce the [halting problem](../../../../../../halting-problem.md) to it. Given a [Turing machine](../../../../../../turing-machine.md) $M$ and input [word](../../../../../../string.md) $w$, construct a [Turing machine](../../../../../../turing-machine.md) $T$ over $\{a,b,c\}$ with the following behavior on input $x$:

- If $x\ne\varepsilon$, reject.
- If $x=\varepsilon$, simulate $M$ on the fixed [word](../../../../../../string.md) $w$. If that simulation ever halts, whether accepting or rejecting, accept $x$; otherwise continue the simulation forever.

This is an effective construction: $M,w$ are fixed data stored in the description of $T$. Its recognized [formal language](../../../../../../formal-language.md) is

$$
\boxed{L(T)=\begin{cases}\{\varepsilon\}&M\text{ halts on }w,\\\varnothing&M\text{ does not halt on }w.\end{cases}}
$$

Therefore $T$ accepts exactly one input [word](../../../../../../string.md) if and only if $M$ halts on $w$. A supposed decision procedure for the [singleton-language problem for Turing machines](../../../../../../singleton-language-problem-for-turing-machines.md), applied to the constructed $T$, would decide the [halting problem](../../../../../../halting-problem.md). The standard undecidability of the [halting problem](../../../../../../halting-problem.md) excludes that possibility.

$$
\boxed{\text{The singleton-language problem for Turing machines is undecidable}.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Models of computation](../../../../models-of-computation-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
