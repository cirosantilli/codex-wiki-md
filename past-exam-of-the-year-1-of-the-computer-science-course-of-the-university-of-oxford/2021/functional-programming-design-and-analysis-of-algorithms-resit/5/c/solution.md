<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A strict [majority element](../../../../../majority-element.md) in the whole [array](../../../../../array-data-structure.md) must be a strict [majority element](../../../../../majority-element.md) in at least one half: otherwise summing the two non-[majority element](../../../../../majority-element.md) frequency bounds would give at most half of all entries. This observation supplies at most two candidates, but they must still be verified in the whole subarray.
```
majority(A, left, right):
    if left == right: return NoMajority
    if right - left == 1: return Candidate(A[left])
    middle = floor((left + right)/2)
    first = majority(A, left, middle)
    second = majority(A, middle, right)
    for candidate in the two returned tagged results:
        if candidate is Candidate(x):
            count = 0
            for i from left to right-1:
                if A[i] == x: count = count + 1
            if 2*count > right-left: return Candidate(x)
    return NoMajority
```
`NoMajority` is a separate result tag, not a possible input element. The two-candidate loop does not require ordering, hashing or conversion of arbitrary elements to a [set](../../../../../set-split.md). It may count the same candidate twice without changing correctness or the bound.

[Induction](../../../../../mathematical-induction.md) proves the recursive candidates correct. If the whole subarray has a [majority element](../../../../../majority-element.md), the observation ensures it reaches the verification step; if a candidate passes the strict frequency test, it really is a [majority element](../../../../../majority-element.md). The worst-case recurrence has two balanced [recursive calls](../../../../../recursive-call.md) and linear combination work, so the running time is **$\Theta(n\log n)$**, with $O(\log n)$ auxiliary [recursion](../../../../../recursion-computer-science.md) depth when the [array](../../../../../array-data-structure.md) is passed by index ranges. A different cancellation-based method can achieve linear time, but is not needed for this divide-and-conquer construction.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
