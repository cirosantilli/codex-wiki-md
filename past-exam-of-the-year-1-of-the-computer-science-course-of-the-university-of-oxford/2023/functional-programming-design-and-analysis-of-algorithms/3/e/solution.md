<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $N$ be the number of distinct dictionary candidates. A wrong guess is itself a current candidate, but its actual score differs from its score against itself, which has all positions as bulls. Therefore each wrong reply removes at least that candidate while retaining the true secret. There can be at most $N-1$ wrong guesses. A correct guess leaves only the secret consistent with the all-bull reply. Hence every such infinite game's history eventually has the constant tail

$$
(\text{secret},\text{all-bull score}),\quad
(\text{secret},\text{all-bull score}),\quad\ldots.
$$

This is the [finite candidate elimination bound](../../../../../finite-candidate-elimination-bound.md); it assumes a nonempty finite dictionary of fixed-length secrets and a strategy that chooses from the remaining candidates.

The stated end condition is identification, so stop when just one candidate remains, even if it has not been guessed. Replace the worker above by
```
play [] _ = []
play [_] _ = []
play candidates replies =
  let g = strategy candidates
  in g : case replies of
      [] -> []
      r:rs -> play [s | s <- candidates, score s g == r] rs
```
The scorer can stay `map (score secret)`: once the guess list ends, its score list ends too. The unchanged `game` then returns a finite history, with at most $N-1$ rounds; a singleton initial dictionary needs no round. If the identified secret is also wanted as an explicit output, return that sole surviving candidate alongside the history.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
