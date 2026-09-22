<h1 id="m/m5/a/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Let $e_k$ be the expected number of children receiving a sticker when $k$ remain. A first-step decomposition gives

$$
e_0=0,\qquad e_k=1+\frac1k\sum_{j=0}^{k-1}e_j\quad(k\geq1).
$$

Subtracting the equations for $ke_k$ and $(k-1)e_{k-1}$ gives $e_k-e_{k-1}=1/k$. Hence $e_k=H_k$, the $k$th [harmonic number](../../../../../../harmonic-number.md). In particular

$$
\boxed{e_4=1+\frac12+\frac13+\frac14=\frac{25}{12}.}
$$

Every visit before absorption counts exactly one child who receives at least one sticker.

The same first-step argument applies to the [uniform depletion Markov chain](../../../../../../uniform-depletion-markov-chain.md) at every initial stock size.

## ↑ Ancestors (14)

1. [V](../v.md)
2. [A](../../a.md)
3. [M5](../../../m5.md)
4. [M](../../../../m.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
