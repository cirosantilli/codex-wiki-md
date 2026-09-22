<h1 id="a1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the first 10, 20, 30 and 40 entries of the already computed list in a two-by-two array of axes. Each subplot needs an index sequence starting at one and having the same length as its data:


```
import matplotlib.pyplot as plt

fig, axes = plt.subplots(2, 2, figsize=(8, 6), layout="constrained")
for ax, stop in zip(axes.flat, [10, 20, 30, 40]):
    ax.plot(range(1, stop + 1), list50[:stop])
    ax.set(title=f"n = {stop}", xlabel="n", ylabel="f(n)")
plt.show()
```
The panels use different vertical scales, which is why the exponential-looking growth remains visible at each range. The available values through 50 are retained in `list50`, even though the requested four panels stop at 40.

<a id="a1/c/image-fibonacci-growth-over-four-index-ranges-generated-directly-from-the-closed-formula"></a>
![](../../../../../past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2024/paper-2-fibonacci.png)

**[Figure 1](#a1/c/image-fibonacci-growth-over-four-index-ranges-generated-directly-from-the-closed-formula). Fibonacci growth over four index ranges, generated directly from the closed formula**.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [A1](../../a1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
