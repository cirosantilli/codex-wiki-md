# Right-fold fusion law

↑ **Parent:** [List fold](list-fold.md)

If $f$ is strict, $f(a)=b$, and $f(g(x,y))=h(x,f(y))$, then $f\circ\operatorname{foldr}(g,a)=\operatorname{foldr}(h,b)$. The empty case uses the base image and the cons case uses compatibility followed by [structural induction](structural-induction.md). Strictness handles a bottom-valued spine. For pure definable continuous [functions](function-split.md), equality on finite [partial lists](partial-list.md) extends to infinite [lists](list-abstract-data-type.md) by finite approximation. For finite total inputs alone, [induction](mathematical-induction.md) does not require the strictness hypothesis.

## ↑ Ancestors (5)

1. [List fold](list-fold.md)
2. [Functional programming](functional-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/4/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/4/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/4/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/functional-programming-design-and-analysis-of-algorithms-resit/1/a/solution.md)
