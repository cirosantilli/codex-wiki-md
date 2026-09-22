# Exponential forcing response with zero initial data

↑ **Parent:** [Linear ordinary differential equation](linear-ordinary-differential-equation-split.md)

For pairwise distinct rates $a,b,c$, the response is

$$
y=\frac{e^{ax}}{(a-b)(a-c)}+\frac{e^{bx}}{(b-a)(b-c)}+\frac{e^{cx}}{(c-a)(c-b)}.
$$

Set $v=y'-by$. Solving $v'-av=e^{cx}$ with $v(0)=0$ gives $(e^{cx}-e^{ax})/(c-a)$; solving the remaining first-order equation by an [integrating factor](integrating-factor.md) gives the formula. Equivalently this is the convolution of $e^{cx}$ with the zero-displacement unit-impulse response $(e^{ax}-e^{bx})/(a-b)$ on the positive half-line. In the resonant case $c=b\ne a$, the finite limit is $y=[e^{ax}-e^{bx}-(a-b)xe^{bx}]/(a-b)^2$. The apparent singularity of the distinct-rate expression is removable, and the limit exhibits the polynomial factor of a [resonant exponential particular solution](resonant-exponential-particular-solution.md).

## ↑ Ancestors (7)

1. [Linear ordinary differential equation](linear-ordinary-differential-equation-split.md)
2. [Ordinary differential equation](ordinary-differential-equation.md)
3. [Differential equation](differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2005/paper-1/10/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2005/paper-1/10/b/solution.md)
