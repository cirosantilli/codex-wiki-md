# Neumann Green function for a second-order ordinary differential equation

↑ **Parent:** [Green's function](green-s-function.md)

Let $y_1,y_2$ solve $y''+\alpha y'+\beta y=0$ with $y_1'(0)=0$ and $y_2'(1)=0$. For Neumann boundary conditions, the Green function is

$$
G(x,\xi)=\frac1{W(\xi)}
\begin{cases}
y_1(x)y_2(\xi),&x<\xi,\\
y_2(x)y_1(\xi),&x>\xi,
\end{cases}
$$

where $W=y_1y_2'-y_1'y_2$. The derivative jump is one. If $\alpha=0$, the Abel identity makes $W$ constant and $G$ symmetric.

## ↑ Ancestors (5)

1. [Green's function](green-s-function.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-1/13b/solution.md)
