<h1 id="20h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $C$ be an [open communicating class](../../../../../../open-communicating-class.md), and fix $i\in C$. There is a path of positive probability from $i$ to a state outside $C$. Choose a shortest such path, so it does not revisit $i$ before exiting. No state reached outside $C$ can have a path back to $C$: combined with the exit path and communication within $C$, such a path would put it in the same [communicating class](../../../../../../communicating-class.md). Thus with positive probability the chain never returns to $i$. Its return probability is less than one, making $i$ a [transient state](../../../../../../transient-state.md). This proves transience throughout $C$.

Conversely, suppose a finite [communicating class](../../../../../../communicating-class.md) were both closed and transient. Starting inside it, a path stays there forever. Since it has finitely many states, at least one state must be visited infinitely often. But a [transient state](../../../../../../transient-state.md) is visited only finitely often almost surely, and the union of finitely many exceptional null events still has probability zero. This is a contradiction. **Every finite transient [communicating class](../../../../../../communicating-class.md) is therefore open.**

For the infinite counterexample, take the [biased random walk](../../../../../../biased-random-walk.md) on $\mathbb Z$ with independent increments $+1$ of probability $3/4$ and $-1$ of probability $1/4$. All states communicate, so $\mathbb Z$ is one infinite [closed communicating class](../../../../../../closed-communicating-class.md). The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $X_n/n\to1/2$ almost surely. Consequently every fixed state is visited only finitely often, and the class is transient. Finiteness is exactly what fails in the preceding argument.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20H](../../20h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
