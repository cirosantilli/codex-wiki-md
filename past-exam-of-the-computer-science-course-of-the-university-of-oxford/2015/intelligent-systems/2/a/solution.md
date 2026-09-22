<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Index the coins so that $c_1$ is smallest and $c_n$ largest. Choose $s_1$ as the initial stack and $s_2$ as the destination, assuming $k\ge2$. The [static predicate](../../../../../static-predicate.md) facts describing size are

$$
S_{\mathrm{size}}=\{\operatorname{Smaller}(c_i,c_j):1\le i<j\le n\}.
$$

No size comparison with $g$ is needed: moving onto empty ground will have a separate [action schema](../../../../../action-schema.md). The initial [STRIPS](../../../../../strips.md) state is

$$
\boxed{
I=S_{\mathrm{size}}
\cup\{\operatorname{OnTop}(c_i,c_{i+1}):1\le i<n\}
\cup\{\operatorname{OnTop}(c_n,g),\operatorname{Topmost}(c_1,s_1)\}
\cup\{\operatorname{Topmost}(g,s_j):2\le j\le k\}.}
$$

Under the [closed-world assumption](../../../../../closed-world-assumption.md), all other ground [ground atoms](../../../../../ground-atom.md) are false. In particular, the initial state contains just one [predicate](../../../../../predicate.md) fact naming the top of each stack. The [predicate](../../../../../predicate.md) $\operatorname{OnTop}$ names the immediate support, not every coin farther below.

An explicit positive conjunctive goal is the following [set](../../../../../set-split.md) of required [ground atoms](../../../../../ground-atom.md):

$$
\boxed{
G_{\mathrm{goal}}=
\{\operatorname{OnTop}(c_i,c_{i+1}):1\le i<n\}
\cup\{\operatorname{OnTop}(c_n,g),\operatorname{Topmost}(c_1,s_2)\}
\cup\{\operatorname{Topmost}(g,s_j):j\ne2\}.}
$$

A state succeeds when it contains $G_{\mathrm{goal}}$. The [static predicate](../../../../../static-predicate.md) facts in $S_{\mathrm{size}}$ persist automatically. Starting from $I$, the [planning state invariants](../../../../../planning-state-invariant.md) proved below make this goal exactly the desired completed stack on $s_2$ with all other stacks empty. If any new stack is acceptable, the choice of $s_2$ loses no generality because the initially empty stacks are interchangeable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Intelligent systems](../../../intelligent-systems-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
