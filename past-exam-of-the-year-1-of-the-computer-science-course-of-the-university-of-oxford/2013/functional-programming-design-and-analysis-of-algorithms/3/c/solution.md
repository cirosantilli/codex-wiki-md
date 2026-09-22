<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Compare frequencies in decreasing order and use [lexicographic order](../../../../../lexicographic-order.md) on words to break ties. Implement [merge sort](../../../../../merge-sort.md) explicitly, so no imported sorting routine is needed:

```
-- Entry, TextWord and Frequency are as in part (b).
before :: Entry -> Entry -> Bool
before (w, p) (v, q) = p > q || (p == q && w <= v)

sort :: [Entry] -> [Entry]
sort []  = []
sort [x] = [x]
sort xs  = merge (sort left) (sort right)
  where
    (left, right) = splitAt (length xs `div` 2) xs

merge :: [Entry] -> [Entry] -> [Entry]
merge [] ys = ys
merge xs [] = xs
merge xa@(x:xs) ya@(y:ys)
  | before x y = x : merge xs ya
  | otherwise  = y : merge xa ys
```

The [merge algorithm](../../../../../merge-algorithm.md) step always emits the smaller key under the ordering $(-\text{frequency},\text{word})$. The unchosen heads cannot precede that emitted entry because each input is already sorted. It preserves all entries, and each call removes one head, so it terminates with exactly the sorted union of the inputs. [Mathematical induction](../../../../../mathematical-induction.md) over the recursive splits establishes correctness of [merge sort](../../../../../merge-sort.md).

For $n$ entries, splitting and merging cost $\Theta(n)$ per level, and there are $\Theta(\log n)$ levels:

$$
\boxed{T(n)=T(\lfloor n/2\rfloor)+T(\lceil n/2\rceil)+\Theta(n)=\Theta(n\log n)\quad(n\geq2).}
$$

The base cases take constant time. This counts word comparisons as primitive operations, as in the question. If the maximum compared word length is $L$, the character-operation bound becomes $O(Ln\log n)$, in addition to frequency comparison costs.

For the supplied input, `sort . count` yields

```
[("baa",2),("sir",2),("yes",2),("any",1),("bags",1),("black",1),
 ("full",1),("have",1),("sheep",1),("three",1),("wool",1),("you",1)]
```

In particular, the secondary ordering places `sir` before `yes`, even though `yes` appears earlier in the original text. The $\Theta(n\log n)$ requirement concerns `sort`; the simpler [association list](../../../../../association-list.md) implementation of `count` has its own cost.

## ↑ Ancestors (12)

1. [C](../c.md)
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
