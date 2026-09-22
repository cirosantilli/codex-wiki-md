<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For [natural logarithms](../../../../../../natural-logarithm.md) and sufficiently large $n$, take the [logarithm](../../../../../../logarithm.md) of the positive expression:

$$
\log\left((\log n)^{\log\log n}\right)=(\log\log n)^2.
$$

Set $t=\log\log n$. Then $\log n=e^t$. The [exponential function](../../../../../../exponential-function.md) grows faster than $t^2$: for example, its power series gives $e^t\geq t^3/6$ for $t>0$, so $t^2/e^t\leq6/t\to0$. In particular, eventually $(\log\log n)^2\leq\log n$. Exponentiating yields

$$
\boxed{(\log n)^{\log\log n}\leq n\text{ eventually},\qquad (\log n)^{\log\log n}=O(n)}.
$$

For logarithms to a fixed base $b>1$, the natural logarithm of the left side is $(\log\log n-\log\log b)^2/\log b$, still smaller than $\log n$ eventually. The [big O notation](../../../../../../big-o-notation.md) conclusion is therefore independent of that base choice.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
