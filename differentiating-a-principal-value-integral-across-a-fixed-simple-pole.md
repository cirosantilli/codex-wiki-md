# Differentiating a principal-value integral across a fixed simple pole

↑ **Parent:** [Cauchy principal value](cauchy-principal-value.md)

Suppose $q(t)=A/(t-c)+r(t)$, where $r$ is continuous, the pole $c$ is fixed, and differentiable endpoints obey $a(x)<c<b(x)$ locally. Then

$$
\operatorname{PV}\int_{a(x)}^{b(x)}q(t)dt=A\ln\frac{|b(x)-c|}{|a(x)-c|}+\int_{a(x)}^{b(x)}r(t)dt.
$$

Apply the [chain rule](chain-rule.md) and the [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) to get

$$
\boxed{\frac d{dx}\operatorname{PV}\int_{a(x)}^{b(x)}q(t)dt=q(b(x))b'(x)-q(a(x))a'(x).}
$$

The same boundary expression as in the [Leibniz integral rule](leibniz-integral-rule.md) thus applies to this explicitly specified [Cauchy principal value](cauchy-principal-value.md). If $A\ne0$, the two ordinary one-sided [improper integrals](improper-integral.md) diverge, so their sum is not an ordinary [integral](integral-split.md). A finite boundary derivative alone does not make that divergent integral meaningful.

## ↑ Ancestors (6)

1. [Cauchy principal value](cauchy-principal-value.md)
2. [Complex analysis](complex-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/20/a/solution.md)
