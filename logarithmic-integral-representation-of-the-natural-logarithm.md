# Logarithmic integral representation of the natural logarithm

↑ **Parent:** [Natural logarithm](natural-logarithm.md)

The [natural logarithm](natural-logarithm.md) has the parameter-integral representation

$$
\boxed{\int_0^1\frac{t^x-1}{\ln t}\,dt=\ln(1+x),\qquad x>-1.}
$$

For $0<t<1$, the identity $(t^x-1)/\ln t=\int_0^x t^s\,ds$ shows convergence: the [absolute value](absolute-value.md) is at most $|x|t^{\min(x,0)}$, which is integrable when $x>-1$. At $t=1$, the apparent singularity is removable, with limiting value $x$.

Write the left side as $I(x)$. On a compact parameter [interval](interval-mathematics.md) $c\leq x\leq d$ with $c>-1$, its differentiated integrand $t^x$ is bounded by the integrable [function](function-split.md) $t^c$. The [dominated convergence theorem](dominated-convergence-theorem.md) justifies [differentiation under the integral sign](differentiation-under-the-integral-sign.md), giving $I'(x)=\int_0^1t^xdt=1/(1+x)$. Since $I(0)=0$, the [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) gives $I(x)=\ln(1+x)$. At $x=-1$, the original [improper integral](improper-integral.md) diverges as $-\int_0dt/[t|\ln t|]$, and it also diverges for $x<-1$.

## ↑ Ancestors (9)

1. [Natural logarithm](natural-logarithm.md)
2. [Logarithm](logarithm.md)
3. [Exponential function](exponential-function.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/19/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/20/c/iii/solution.md)
