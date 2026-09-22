<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A scorer applies the same scoring rule, with the fixed secret, independently to each guess:
```
mkScorer :: (secret -> guess -> score)
         -> secret -> [guess] -> [score]
mkScorer score secret = map (score secret)
```
The first score depends only on the first guess, and every later score only on the corresponding guess. Thus this player has no unguarded dependence on its own future output when connected to the guesser by a [lazy feedback stream](../../../../../lazy-feedback-stream.md). Neither the dictionary nor a strategy is needed by a truthful scorer once the secret and scoring rule are fixed.

## ↑ Ancestors (12)

1. [C](../c.md)
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
