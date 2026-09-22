# Singular endpoint compatibility for a differential equation

↑ **Parent:** [Linear differential equation](linear-differential-equation.md)

A vanishing highest-derivative coefficient can make the two initial values of a second-order [differential equation](differential-equation-split.md) dependent. Suppose $h$ is continuous at zero, $a$ is constant, and a solution of $[t(y'+ay)]'=h(t)$ has finite continuous $y,y'$ at zero. Integration gives

$$
t(y'+ay)=C+\int_0^t h(s)\,ds.
$$

Regularity forces $C=0$. Dividing by $t>0$ and taking the limit gives $y'(0)+ay(0)=h(0)$, since the integral average tends to $h(0)$. The remaining equation is first order and therefore has only one free regular initial value. For $a=1$ and $h(t)=t$, it yields $y'+y=t/2$ and $y=Ae^{-t}+(t-1)/2$. This explains the reduced constant count without treating the singular endpoint as an ordinary second-order initial point.

## ↑ Ancestors (7)

1. [Linear differential equation](linear-differential-equation.md)
2. [Ordinary differential equation](ordinary-differential-equation.md)
3. [Differential equation](differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
