# Derivative of an Abel integral

↑ **Parent:** [Abel integral equation](abel-integral-equation.md)

Suppose $h$ is continuously [differentiable](differentiable-function.md) on $[0,L]$. For $0<x\leq L$, the [improper integral](improper-integral.md) $g(x)=\int_0^xh(t)(x-t)^{-1/2}dt$ exists, but substituting directly into the ordinary [Leibniz integral rule](leibniz-integral-rule.md) produces an undefined endpoint term. First use [integration by parts](integration-by-parts.md) to obtain

$$
g(x)=2h(0)\sqrt x+2\int_0^xh'(t)\sqrt{x-t}\,dt.
$$

The new endpoint term at $t=x$ vanishes, and the differentiated kernel is locally [integrable](integrability.md). Differentiating gives the displayed formula. One rigorous justification rewrites the second term as $\int_0^x[\int_0^s h'(t)(s-t)^{-1/2}dt]ds$ by [Fubini's theorem](fubini-s-theorem.md); the inner [integral](integral-split.md) is continuous for $s>0$, so the [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) applies. Moreover $g(x)=2h(0)\sqrt x+O(x^{3/2})$: if $h(0)\ne0$, the right [difference quotient](difference-quotient.md) at zero diverges rather than defining a finite [derivative](derivative.md).

## ↑ Ancestors (6)

1. [Abel integral equation](abel-integral-equation.md)
2. [Integral equation](integral-equation.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/section-b/10/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/section-b/10/b/iii/solution.md)
