<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose each team once using `teams`, then scan every match with that team as the reference perspective:

```
data Results = Results Team [(Int,Int)]

extract :: [[Match]] -> [Results]
extract days = [Results t (scores t) | t <- teams days]
  where
    games = concat days
    scores t = concatMap (contribution t) games
    contribution t (Match a ga b gb)
      | t == a    = [(ga,gb)]
      | t == b    = [(gb,ga)]
      | otherwise = []
```

In a valid match the teams are distinct. The first guard records the first team's goals-for and goals-against; the second reverses that perspective for the opponent. The common `games` binding preserves day/match order, although the result does not need a chronological ordering condition. Each team receives exactly one record because `teams` has no duplicates. The algorithm makes one scan per team; it deliberately prioritizes a transparent [functional programming](../../../../../functional-programming.md) definition over an unrequested performance improvement.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
