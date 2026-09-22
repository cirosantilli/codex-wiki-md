<h1 id="38a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the stage solution continuous from $k_2=f(y)$ as $h\to0$. Its displacement is $\delta=h[(1-a)f+ak_2]=hf+ah^2f'f+O(h^3)$. Taylor expansion of $f(y+\delta)$ gives

$$
k_2=f+hf'f+h^2\left(af'^2f+\tfrac12f''f^2\right)+O(h^3).
$$

Consequently the [Runge-Kutta method](../../../../../../runge-kutta-method.md) advances by

$$
y_{n+1}=y+hf+\tfrac12h^2f'f+h^3\left(\tfrac a2f'^2f+\tfrac14f''f^2\right)+O(h^4).
$$

The exact solution has third-order term $h^3(f'^2f+f''f^2)/6$. The first two orders agree for every real $a$, but the $f''f^2$ coefficient is always $1/4$ instead of $1/6$. Therefore **the general nonlinear method has $\boxed{\text{order }2}$ for every fixed real $a$**. The special value $a=1/3$ matches the linear test equation at third order but does not raise the nonlinear order. This is the [two-stage Runge-Kutta family with an implicit second stage](../../../../../../two-stage-runge-kutta-family-with-an-implicit-second-stage.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38A](../../38a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
