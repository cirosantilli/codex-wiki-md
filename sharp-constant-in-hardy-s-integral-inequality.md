<h1 id="sharp-constant-in-hardy-s-integral-inequality">Sharp constant in Hardy's integral inequality</h1>

↑ **Parent:** [Hardy's integral inequality](hardy-s-integral-inequality.md)

The [indicator function](indicator-function.md) example reaches a squared [L2 norm](l2-norm.md) ratio of two. To approach four, concentrate more strongly near zero. For $0\leq a<1/2$, use the [measurable function](measurable-function.md)

$$
f_a(x)=x^{-a}\mathbf1_{(0,1)}(x),\qquad Hf_a(x)=\begin{cases}x^{-a}/(1-a),&0<x\leq1,\\1/((1-a)x),&x>1.\end{cases}
$$

All [integrals](integral-split.md) use [Lebesgue measure](lebesgue-measure.md) $dx$. Keeping both portions of the squared [L2 norm](l2-norm.md) gives

$$
\|f_a\|_2^2=\frac1{1-2a},\qquad \int_0^1|Hf_a|^2\,dx=\frac1{(1-a)^2(1-2a)},\qquad \int_1^\infty|Hf_a|^2\,dx=\frac1{(1-a)^2}.
$$

Consequently,

$$
\frac{\|Hf_a\|_2^2}{\|f_a\|_2^2}=\frac1{(1-a)^2}+\frac{1-2a}{(1-a)^2}=\frac2{1-a}\longrightarrow4\quad\text{as }a\uparrow\frac12.
$$

Every allowed member has ratio strictly below four. For any proposed constant $C<4$, a sufficiently large $a<1/2$ has ratio greater than $C$. Combined with [Hardy's integral inequality](hardy-s-integral-inequality.md), this proves that four is the smallest possible squared [L2 norm](l2-norm.md) constant.[Inequalities, second edition, §9.8, Theorem 327, printed p. 240, and sharpness argument on printed p. 243](inequalities-by-godfrey-harold-hardy-and-others.md)

The endpoint is excluded: at $a=1/2$, $\int_0^1|f_a|^2\,dx=\int_0^1x^{-1}\,dx=\infty$, and the inner portion of $\|Hf_a\|_2^2$ also diverges. Its tail still has finite [integral](integral-split.md) four. There is no finite [L2 norm](l2-norm.md) ratio at this endpoint, hence no equality example obtained by substituting it. The [limit](limit-of-a-function.md) four is unattained by this family. Multiplying each $f_a$ by $\sqrt{1-2a}$ makes its [L2 norm](l2-norm.md) one without changing the ratio.

<a id="image-a-power-family-approaches-the-sharp-constant-in-hardy-s-integral-inequality"></a>
![](hardy-power-family-sharp-constant.png)

**[Figure 2](#image-a-power-family-approaches-the-sharp-constant-in-hardy-s-integral-inequality). A power family approaches the Sharp constant in Hardy's integral inequality**. Dashed input curves and solid [Hardy operator](hardy-operator.md) averages show three allowed [exponents](exponent.md). The right panel splits the exact squared [L2 norm](l2-norm.md) ratio into inner and tail contributions. The hollow endpoint marks a [limit](limit-of-a-function.md), not an admissible [function](function-split.md) in [L2 space](l2-space-is-a-hilbert-space.md).

## ↑ Ancestors (7)

1. [Hardy's integral inequality](hardy-s-integral-inequality.md)
2. [Hardy's inequality](hardy-s-inequality.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Sharp constant in Hardy's integral inequality](sharp-constant-in-hardy-s-integral-inequality.md)
