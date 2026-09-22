# Algorithm termination

↑ **Parent:** [Total correctness](total-correctness.md)

[Algorithm termination](algorithm-termination.md) means that execution finishes after finitely many steps on the [inputs](input-computer-science.md) under consideration. Specify that domain: the stalled loop in [partial correctness](partial-correctness.md) terminates for $n=0$ but runs forever for $n=4$. A successful run on one [input](input-computer-science.md) does not establish termination on another.

A useful method is a [loop variant](loop-variant.md) $V$ that is a nonnegative [integer](integer-split.md) at every condition check and strictly decreases whenever the condition is true and the body completes. Also prove that condition evaluation and each body execution terminate. An infinite run would then give an infinite strictly decreasing [sequence](sequence.md) of nonnegative [integers](integer-split.md), contradicting their [well-founded relation](well-founded-relation.md). This establishes [algorithm termination](algorithm-termination.md) without enumerating all executions.

For the [summation loop verification](summation-loop-verification.md), $V=n-i$ begins at $n$ and decreases by exactly one per iteration. The body executes exactly $n$ times, including zero times for $n=0$. Merely bounding a decreasing measure below is insufficient for [real numbers](real-number.md): $1,1/2,1/4,\ldots$ decreases forever while staying positive. The choice of a [well-founded relation](well-founded-relation.md) supplies the essential progress argument; [well-founded progress in recursion](well-founded-progress-in-recursion.md) applies the same idea to [recursive calls](recursive-call.md).

## ↑ Ancestors (5)

1. [Total correctness](total-correctness.md)
2. [Algorithm correctness](algorithm-correctness.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (40)

- [Algorithm correctness](algorithm-correctness.md)
- [Algorithm termination](algorithm-termination.md)
- [Base case](base-case.md)
- [Binary array sum by recursion](binary-array-sum-by-recursion.md)
- [Factorial recursion and returning frames](factorial-recursion-and-returning-frames.md)
- [Finite termination of K-means clustering](finite-termination-of-k-means-clustering.md)
- [Greedy Egyptian fraction expansion](greedy-egyptian-fraction-expansion.md)
- [Linear probing](linear-probing.md)
- [Loop variant](loop-variant.md)
- [Matrix-chain split reconstruction](matrix-chain-split-reconstruction.md)
- [Partial correctness](partial-correctness.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2017/prelims/mathematics-iii/9/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/4/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/6/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/6/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/7/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/2/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability/3/c/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming-resit/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming-resit/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming-resit/4/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming/3/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming/4/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming/4/c/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/5/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/functional-programming-design-and-analysis-of-algorithms-resit/2/f/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/functional-programming-design-and-analysis-of-algorithms-resit/4/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/functional-programming-design-and-analysis-of-algorithms-resit/4/g/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/2/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/3/d/solution.md)
- [Postcondition](postcondition.md)
- [Prefix maximum correctness example](prefix-maximum-correctness-example.md)
- [Quickselect](quickselect.md)
- [Recursion (computer science)](recursion-computer-science.md)
- [Summation loop verification](summation-loop-verification.md)
- [Total correctness](total-correctness.md)
- [While loop](while-loop.md)
