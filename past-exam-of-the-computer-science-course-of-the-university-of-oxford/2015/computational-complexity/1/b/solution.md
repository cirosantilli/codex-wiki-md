<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Rice's theorem](../../../../../rice-s-theorem.md), in its [formal language](../../../../../formal-language.md) version, says: **every nontrivial property of the [computably enumerable language](../../../../../recursively-enumerable-language.md) accepted by a [Turing machine](../../../../../turing-machine.md) has an [undecidable](../../../../../undecidable-decision-problem.md) set of machine descriptions.** Here nontrivial means that some [computably enumerable language](../../../../../recursively-enumerable-language.md) has the property and some does not. The property must be an [extensional property of programs](../../../../../extensional-property-of-programs.md): any two [Turing machines](../../../../../turing-machine.md) accepting the same [formal language](../../../../../formal-language.md) must agree about it. It need not be a property of all [formal languages](../../../../../formal-language.md), including those no [Turing machine](../../../../../turing-machine.md) accepts.

Let $\mathscr P$ be such a property and write

$$
I_{\mathscr P}=\{\operatorname{enc}(N):\mathcal L(N)\in\mathscr P\}.
$$

We prove the theorem by a [many-one reduction](../../../../../many-one-reduction.md) from the [halting problem](../../../../../halting-problem.md). First suppose the [empty language](../../../../../empty-language.md) is not in $\mathscr P$. Nontriviality provides a fixed [Turing machine](../../../../../turing-machine.md) $B$ with $\mathcal L(B)\in\mathscr P$. Given a [Turing machine](../../../../../turing-machine.md) $M$ and a [word over an alphabet](../../../../../string.md) $w$, effectively construct a [Turing machine](../../../../../turing-machine.md) $N_{M,w}$ which, on [input](../../../../../input-computer-science.md) $x$, first simulates $M$ on $w$. If that simulation ever halts, it simulates $B$ on $x$ and accepts precisely when $B$ accepts. If the first simulation never halts, it never accepts $x$.

The [Turing machine encoding](../../../../../turing-machine-encoding.md) of $N_{M,w}$ is computable from those of $M,w$: the description merely embeds $M,w$ and the fixed simulator for $B$. Constructing it does not require predicting whether $M$ halts. Its accepted [formal language](../../../../../formal-language.md) is

$$
\mathcal L(N_{M,w})=
\begin{cases}
\mathcal L(B),&M\text{ halts on }w,\\
\varnothing,&M\text{ does not halt on }w.
\end{cases}
$$

Consequently

$$
M\text{ halts on }w\quad\Longleftrightarrow\quad
\operatorname{enc}(N_{M,w})\in I_{\mathscr P}.
$$

A decider for $I_{\mathscr P}$ would therefore decide the [halting problem](../../../../../halting-problem.md), a contradiction. Invalid descriptions can be mapped to a fixed description of a machine accepting the [empty language](../../../../../empty-language.md), if the [many-one reduction](../../../../../many-one-reduction.md) is formulated on all [strings](../../../../../string.md).

If the [empty language](../../../../../empty-language.md) does belong to $\mathscr P$, apply the preceding argument to the opposite property, within the [computably enumerable languages](../../../../../recursively-enumerable-language.md). This opposite property is still nontrivial and excludes the [empty language](../../../../../empty-language.md). A hypothetical decider for $I_{\mathscr P}$ would decide the opposite property's index set by first rejecting malformed [Turing machine encodings](../../../../../turing-machine-encoding.md) and otherwise reversing its answer. The opposite property is [undecidable](../../../../../undecidable-decision-problem.md) by the first case, giving the required contradiction in this case too.

$$
\boxed{I_{\mathscr P}\text{ is undecidable for every nontrivial extensional }\mathscr P.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Computational complexity](../../../computational-complexity-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
