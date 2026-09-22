# Antiderivative

↑ **Parent:** [Integral](integral.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antiderivative)

An antiderivative recovers a [function](function-split.md) from its local rate of change. For a [real-valued function](real-valued-function.md) $g$ on an [open subset](open-set.md) $U$ of the [real line](real-line.md), a [differentiable function](differentiable-function.md) $F$ is an antiderivative when

$$
\boxed{F'(x)=g(x)\qquad(x\in U).}
$$

For example, $g(x)=x^2$ has the antiderivatives $F_C(x)=x^3/3+C$ for every real [additive constant](additive-constant.md) $C$. Their [derivatives](derivative.md) agree, while their values can differ. On an [interval](interval-mathematics.md), the [constant of integration](constant-of-integration.md) describes the entire freedom in the answer. [OpenStax Calculus 1, §4.10: antiderivatives and their families](https://openstax.org/books/calculus-volume-1/pages/4-10-antiderivatives)

<a id="image-a-family-of-antiderivatives-has-one-common-derivative-and-an-initial-value-selects-one-member"></a>
![](antiderivative-family-and-initial-value.png)

**[Figure 8](#image-a-family-of-antiderivatives-has-one-common-derivative-and-an-initial-value-selects-one-member). A family of antiderivatives has one common derivative, and an initial value selects one member**.

The indefinite-integral notation $\int g(x)\,dx=F(x)+C$ records this family on an [interval](interval-mathematics.md). For the illustrated family, the extra condition $F(1)=2$ selects $C=5/3$. Thus reversing [differentiation](differentiation.md) requires both a rate and a reference value if a unique [function](function-split.md) is wanted.

The [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) supplies a construction when $g$ is [continuous](continuous-function.md) on an [interval](interval-mathematics.md) $I$. Choose $x_0\in I$ and set $F(x)=\int_{x_0}^x g(t)\,dt$; then $F'=g$. [Integrability](integrability.md) alone does not guarantee a classical antiderivative. The [Heaviside step function](heaviside-step-function.md) is [Riemann integrable](riemann-integrable-function.md) on bounded [intervals](interval-mathematics.md), but cannot be a [derivative](derivative.md) throughout an [interval](interval-mathematics.md) containing its jump: [Darboux theorem for derivatives](darboux-s-theorem-analysis.md) requires every intermediate value. [Lebl, Basic Analysis I, §4.2.5: the intermediate-value property of derivatives](https://www.jirka.org/ra/html/sec_mvt.html)

**Table of contents**

- [Constant of integration](constant-of-integration.md)
  - [Antiderivatives on disconnected domains](antiderivatives-on-disconnected-domains.md)
- [Additive constant](additive-constant.md)

## ↑ Ancestors (7)

1. [Integral](integral.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (27)

- [Additive constant](additive-constant.md)
- [Antiderivatives on disconnected domains](antiderivatives-on-disconnected-domains.md)
- [Change of variables formula](change-of-variables-formula.md)
- [Complex analysis](complex-analysis-split.md)
- [Constant of integration](constant-of-integration.md)
- [Countertravelling decomposition of the one-dimensional wave equation](countertravelling-decomposition-of-the-one-dimensional-wave-equation.md)
- [Definite integral](definite-integral.md)
- [Fourier orthogonality](fourier-orthogonality.md)
- [Fundamental theorem of calculus](fundamental-theorem-of-calculus.md)
- [Hyperbolic sine](hyperbolic-sine.md)
- [Integral](integral.md)
- [Integration by parts](integration-by-parts.md)
- [Interference (wave propagation)](interference-wave-propagation.md)
- [Mellin transform of an interval indicator](mellin-transform-of-an-interval-indicator.md)
- [On-axis magnetic field of a finite solenoid](on-axis-magnetic-field-of-a-finite-solenoid.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/16a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-51/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-71/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5/1/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/4f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-328/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3/23f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/14a/d/solution.md)
- [Primitive of a holomorphic function on a simply connected domain](primitive-of-a-holomorphic-function-on-a-simply-connected-domain.md)
- [Residue theorem](residue-theorem.md)
- [Separable differential equation](separable-differential-equation.md)
- [Signed area under a graph](signed-area-under-a-graph.md)
