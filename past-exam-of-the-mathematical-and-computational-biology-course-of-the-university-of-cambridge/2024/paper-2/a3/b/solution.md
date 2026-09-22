<h1 id="a3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Plot the entire stated interval:


```
import matplotlib.pyplot as plt

x_grid = np.linspace(-4, 4, 1500)
plt.plot(x_grid, f(x_grid))
plt.xlabel("x")
plt.ylabel("f(x)")
plt.show()
```
The oscillating objective has several wells. A local search starting at $-1$ need not reach the deepest one, which is near $-0.309$. For the literal maximization in part (a), no minimum was being sought at all. Under the intended minimization interpretation, the result near $-1.546$ belongs to a different attraction region from the [global minimum](../../../../../global-minimum.md).

<a id="a3/b/image-local-extrema-the-global-minimum-and-the-constrained-minimum-of-the-oscillatory-objective"></a>
![](../../../../../past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2024/paper-2-multistart-optimization.png)

**[Figure 2](#a3/b/image-local-extrema-the-global-minimum-and-the-constrained-minimum-of-the-oscillatory-objective). Local extrema, the global minimum and the constrained minimum of the oscillatory objective**.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [A3](../../a3.md)
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
