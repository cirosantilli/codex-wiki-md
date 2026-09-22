<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The score function takes a proposed secret first and a guess second:
```
mkGuesser :: Eq score
          => (guess -> guess -> score)
          -> ([guess] -> guess)
          -> [guess] -> [score] -> [guess]
mkGuesser score strategy dictionary = play dictionary
  where
    play candidates replies =
      let g = strategy candidates
      in g : case replies of
          [] -> []
          r:rs -> play [s | s <- candidates, score s g == r] rs
```
Assume that the initial dictionary contains the secret, that scores are truthful, and that `strategy` returns a candidate from its nonempty input. The candidate [invariant](../../../../../invariant-mathematics.md) is exactly the dictionary entries consistent with every score already received. Filtering by `score s g == r` establishes the same invariant after the next reply and retains the true secret.

Crucially, the next guess `g` is placed under the outer list constructor before `replies` is inspected. It depends on earlier replies only; the first guess depends on none. This guarded [lazy feedback stream](../../../../../lazy-feedback-stream.md) makes the mutually recursive `game` productive whenever the strategy and scoring operations terminate. Moving the `case replies` outside the constructor would create a circular demand before the first guess.

## ↑ Ancestors (12)

1. [D](../d.md)
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
