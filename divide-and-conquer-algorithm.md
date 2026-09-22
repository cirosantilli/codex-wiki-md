# Divide-and-conquer algorithm

↑ **Parent:** [Algorithm](algorithm-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Divide-and-conquer_algorithm)

A [divide-and-conquer algorithm](divide-and-conquer-algorithm.md) divides a problem into smaller instances, solves them using [recursion](recursion-computer-science.md), and combines their answers. In [merge sort](merge-sort.md), the division makes two contiguous halves, and the [merge algorithm](merge-algorithm.md) combines the resulting [sorted arrays](sorted-array.md). The important design step is finding a combination rule cheaper than solving the whole problem afresh.

Halving the [input](input-computer-science.md) is only one part of the design. The number of [recursive calls](recursive-call.md) and the work outside those calls determine whether the smaller instances actually save time. [Divide-and-conquer combination cost](divide-and-conquer-combination-cost.md) keeps these quantities separate; the [divide-and-conquer product ledger](divide-and-conquer-product-ledger.md) shows how an algebraic identity changes the number of required calls in [Karatsuba multiplication](karatsuba-multiplication.md).

For [algorithm correctness](algorithm-correctness.md), specify the meaning of each returned answer, prove the [base cases](base-case.md), and show that combining correct smaller answers gives the required [output](output-computing.md). [Induction](mathematical-induction.md) then proves correctness, provided every [recursive call](recursive-call.md) progresses towards a [base case](base-case.md). The combination rule must reconstruct everything the caller needs: two sorted halves alone are not a [sorted array](sorted-array.md), and four digit blocks alone are not their [integer](integer-split.md) product.

**Table of contents**

- [Integer rounding in a divide-and-conquer recurrence](integer-rounding-in-a-divide-and-conquer-recurrence.md)
- [Simultaneous minimum and maximum](simultaneous-minimum-and-maximum.md)
- [Array local maximum](array-local-maximum.md)
- [Divide-and-conquer majority element](divide-and-conquer-majority-element.md)
- [CDQ divide and conquer](cdq-divide-and-conquer.md)
- [Divide-and-conquer combination cost](divide-and-conquer-combination-cost.md)
- [Divide-and-conquer product ledger](divide-and-conquer-product-ledger.md)

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (23)

- [Algorithm design](algorithm-design.md)
- [Array local maximum](array-local-maximum.md)
- [Bitonic sorting algorithm](bitonic-sorting-algorithm.md)
- [Divide-and-conquer algorithm](divide-and-conquer-algorithm.md)
- [Divide-and-conquer combination cost](divide-and-conquer-combination-cost.md)
- [Karatsuba multiplication](karatsuba-multiplication.md)
- [Maximum-subarray segment summary](maximum-subarray-segment-summary.md)
- [Merge sort](merge-sort.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/4/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/4/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/6/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/5/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/6/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/5/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/5/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/5/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/6/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/5/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/5/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/5/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/8/d/solution.md)
- [Quicksort](quicksort.md)
- [Simultaneous minimum and maximum](simultaneous-minimum-and-maximum.md)
