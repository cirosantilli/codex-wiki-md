<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Consider a B-node whose parent is an A-node with an already completed incumbent outcome having A-coordinate $\alpha$. At the B-node, let $(x,y)$ be the best completed child pair found so far according to B's coordinate. Every remaining child can be skipped, and this B-option discarded by its parent, if

$$
\boxed{\epsilon-y\le\alpha,\quad\text{equivalently }y\ge\epsilon-\alpha.}
$$

Use a strict inequality if ties must remain open; equality is safe under the fixed rule that the parent retains its already selected child on an A-coordinate tie. This is a [nearly-zero-sum pruning](../../../../../nearly-zero-sum-pruning.md) rule.

To prove it, note first that a completed [max-n search](../../../../../max-n-search.md) value is some terminal [utility](../../../../../utility.md) pair: each backup copies one entire child pair. Thus the nearly-zero-sum inequality holds at every completed subtree, not just at leaves. Since B maximizes its own coordinate, the ultimately selected pair $(u,v)$ at this B-node has $v\ge y$. Therefore

$$
u+v\le\epsilon
\quad\Longrightarrow\quad
u\le\epsilon-v\le\epsilon-y\le\alpha.
$$

The already available A-option is at least as good, so remaining children of this B-node cannot alter the parent's selected continuation under the stated tie rule. The second half of the two-sided nearly-zero-sum condition also gives $x+y\ge-\epsilon$, hence

$$
u\le\epsilon-y\le x+2\epsilon.
$$

Consequently **$x+2\epsilon\le\alpha$ is another sufficient cutoff**, useful if one phrases the test using the observed A-coordinate. The pair-based test is sharper: the value of $y$ can certify a cutoff even when the conservative $x+2\epsilon$ test cannot.

When $\epsilon=0$, every pair satisfies $y=-x$, and the rule reduces to $x\le\alpha$, the ordinary MIN-node [alpha-beta pruning](../../../../../alpha-beta-pruning.md) cutoff. The extra $2\epsilon$ in the A-coordinate-only condition is necessary in general: an observed pair $(-1,0)$ satisfies the bound for $\epsilon=1$, but B prefers an unseen $(1-\delta,\delta)$ for $0<\delta<1$. A increases by almost $2\epsilon$; using just $x+\epsilon$ as the upper bound would be invalid.

Implementation must discard the ruled-out B-option at its parent rather than return $(x,y)$ as an exact completed [utility](../../../../../utility.md) pair. The proof uses an actual completed alternative at that parent; it does not authorize passing arbitrary distant ancestor bounds through [general-sum game](../../../../../general-sum-game.md) backups as if every scalar [alpha-beta pruning](../../../../../alpha-beta-pruning.md) invariant still held. With these local certified cutoffs, an induction over completed subtrees preserves the selected pair and hence the root outcome.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
