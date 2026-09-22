<h1 id="a3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The first instruction asks for maximization, whereas the later parts refer to minimization. For the literal maximization task, minimize the negative objective:


```
import numpy as np
from scipy import optimize as opt


def f(x):
    return 1 + np.exp(-x*x/5) * np.sin(5*x)


maximum = opt.minimize(lambda z: -f(z[0]), x0=[-1.0])
print(maximum.x[0], f(maximum.x[0]))
```
This gives a [local maximum](../../../../../local-maximum.md) near **$x=-0.927662$, $f(x)=1.839576$**. If minimization was intended, use `opt.minimize(lambda z: f(z[0]), x0=[-1.0])`, which instead returns a [local minimum](../../../../../local-minimum.md) near **$x=-1.546182$, $f(x)=0.384751$**. The optimizer's stopping criterion establishes local numerical convergence, not a certificate of a global optimum.

## ↑ Ancestors (13)

1. [A](../a.md)
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
