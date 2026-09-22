<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Normalize each word once by applying `toLower` to its characters. Maintain an [association list](../../../../../association-list.md) whose keys are distinct normalized words and whose values are their frequencies:

```
import Data.Char (toLower)

type TextWord = String
type Text = [TextWord]
type Frequency = Integer
type Entry = (TextWord, Frequency)

count :: Text -> [Entry]
count = foldl addWord [] . map (map toLower)
  where
    -- Increment the unique matching key, or append a new key with count one.
    addWord :: [Entry] -> TextWord -> [Entry]
    addWord [] w = [(w, 1)]
    addWord ((v, n):rest) w
      | w == v    = (v, n + 1) : rest
      | otherwise = (v, n) : addWord rest w
```

After any input prefix, each normalized word seen so far occurs exactly once as a key, with its number of occurrences as value. This [loop invariant](../../../../../loop-invariant.md) holds initially for the empty [association list](../../../../../association-list.md). A step either increments the unique existing entry or introduces exactly one new entry, so [mathematical induction](../../../../../mathematical-induction.md) proves

$$
\boxed{\operatorname{lookup}\ w\ (\operatorname{count}\ \mathrm{input})=\operatorname{Just}(\text{number of normalized occurrences of }w)}
$$

for every word that occurs. In particular, `Baa` and `baa` contribute to the same key `baa`; the three frequency-two keys in the source example are `baa`, `yes` and `sir`.

The [association list](../../../../../association-list.md) preserves first-occurrence order, although the specification allows any order here. For $t$ input words and $d$ distinct normalized words, it performs $O(td)$ key comparisons in the worst case. Character normalization costs the total input character count, and a [string](../../../../../string.md) comparison can inspect multiple characters. Characterwise `toLower` supplies the intended [case-insensitive comparison](../../../../../case-insensitive-comparison.md) convention for the example; full Unicode case folding can require a different normalization policy.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
