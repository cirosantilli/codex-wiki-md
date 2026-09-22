<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Ignore zero adjacent differences. A segment is bitonic in the question's peak-or-valley sense precisely when its remaining difference signs change at most once. Keep the earliest starts of the current monotone suffix and current bitonic suffix:

```
if n == 0: return (0,0)
monoStart = 0; bitStart = 0
lastDir = 0; lastStrictEnd = 0
best = 1; bestStart = 0
for i = 1,...,n-1:
    dir = compare(a[i],a[i-1])    // -1, 0, or +1
    if dir != 0:
        if lastDir != 0 and dir != lastDir:
            bitStart = monoStart
            monoStart = lastStrictEnd
        lastDir = dir
        lastStrictEnd = i
    length = i-bitStart+1
    if length > best:
        best = length; bestStart = bitStart
return (bestStart,best)
```

After processing $i$, `lastDir` is the most recent nonzero difference sign; `lastStrictEnd` is its endpoint. `monoStart` is the earliest start of a suffix with only that nonzero direction, and `bitStart` is the earliest start of a suffix with at most one sign change. The best recorded interval realizes the largest such length over the whole scanned prefix.

A zero difference changes neither direction. On reversal, a valid new bitonic suffix may retain the entire old monotone suffix, but cannot retain a preceding opposite-direction run as well, which would create two changes. Hence its earliest start is the old `monoStart`. The new monotone suffix starts at `lastStrictEnd`, retaining the intervening plateau. This proves the update and explains why merely starting at $i-1$ loses valid overlapping segments. The [longest bitonic contiguous segment](../../../../../longest-bitonic-contiguous-segment.md) algorithm uses **$O(n)$ time and $O(1)$ auxiliary space**; the sample's maximum length is **5**.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
