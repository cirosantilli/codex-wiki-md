# Radial modified Helmholtz equation

↑ **Parent:** [Modified Helmholtz equation](modified-helmholtz-equation.md)

For a [radial function](radial-function.md) in three dimensions, $(\Delta-1)y=g(x)$ becomes $y''+2y'/x-y=g(x)$. Setting $u=xy$ gives $u''-u=xg(x)$, reducing it to a constant-coefficient [linear ordinary differential equation](linear-ordinary-differential-equation.md). If $g=e^{-3x}/x^2$, a decaying particular solution obtained by [variation of parameters](variation-of-parameters.md) is

$$
y(x)=\alpha\frac{e^{-x}}x+\frac{e^{-x}E_1(2x)-e^xE_1(4x)}{2x}.
$$

The [small-argument expansion of the exponential integral](small-argument-expansion-of-the-exponential-integral.md) gives

$$
y(x)=\frac{\alpha+\tfrac12\log2}{x}+\log x-\alpha+\tfrac32\log2+\gamma-1+O(x\log x).
$$

The undetermined decaying homogeneous coefficient $\alpha$ is fixed by a boundary condition or by a [matched asymptotic expansion](matched-asymptotic-expansion.md).

## ↑ Ancestors (6)

1. [Modified Helmholtz equation](modified-helmholtz-equation.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-336/2/solution.md)
