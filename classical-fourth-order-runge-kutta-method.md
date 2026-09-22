# Classical fourth-order Runge-Kutta method

↑ **Parent:** [Runge-Kutta method](runge-kutta-method.md)

The classical four-stage explicit [Runge-Kutta method](runge-kutta-method.md) uses

$$
A=\begin{pmatrix}0&0&0&0\\1/2&0&0&0\\0&1/2&0&0\\0&0&1&0\end{pmatrix},\qquad
b=(1/6,1/3,1/3,1/6)^T,\qquad c=(0,1/2,1/2,1)^T.
$$

It satisfies the [fourth-order conditions for a Runge-Kutta method](fourth-order-conditions-for-a-runge-kutta-method.md). Its polynomial [stability function](stability-function.md) excludes [A-stability](a-stability.md), while $|R(iq)|^2=1-q^6/72+q^8/576$ gives the imaginary-axis stability interval $|q|\leq2\sqrt2$.

## ↑ Ancestors (6)

1. [Runge-Kutta method](runge-kutta-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/7/solution.md)
