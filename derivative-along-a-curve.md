# Derivative along a curve

↑ **Parent:** [Multivariable chain rule](multivariable-chain-rule.md)

If $F:\mathbb R^n\to\mathbb R$ is [differentiable](differentiable-function.md) at the point $\gamma(t)$ of a [differentiable](differentiable-function.md) [parametric curve](parametric-curve.md), the [multivariable chain rule](multivariable-chain-rule.md) gives

$$
\frac d{dt}F(\gamma(t))=\nabla F(\gamma(t))\cdot\gamma'(t).
$$

The [gradient](gradient.md) supplies the local spatial rates; the [velocity vector](velocity-vector.md) $\gamma'(t)$ supplies the direction and rate of movement. Their [dot product](dot-product.md) is the change in the sampled [scalar field](scalar-field.md) per unit parameter. If the parameter is time, this is a rate per unit time; a [directional derivative](directional-derivative.md) per unit distance instead uses a [unit vector](unit-vector.md).

Take $F(x,y)=x^2+2y^2$ and the [unit circle](complex-unit-circle.md) path $\gamma(t)=(\cos t,\sin t)$. Along the path,

$$
F(\gamma(t))=1+\sin^2t,\qquad
\frac d{dt}F(\gamma(t))=2\sin t\cos t=\sin2t.
$$

At $t=\pi/4$, the [gradient](gradient.md) is $(\sqrt2,2\sqrt2)$, the [velocity vector](velocity-vector.md) is $(-1/\sqrt2,1/\sqrt2)$, and their [dot product](dot-product.md) is $-1+2=1$. The sampled value is $3/2$ and increases at rate one, even though one coordinate is decreasing. This is why a moving observation must combine every coordinate's contribution.

<a id="image-the-gradient-and-path-velocity-combine-to-give-the-rate-of-change-along-a-curve"></a>
![](chain-rule-along-a-path.png)

**[Figure 25](#image-the-gradient-and-path-velocity-combine-to-give-the-rate-of-change-along-a-curve). The gradient and path velocity combine to give the rate of change along a curve**. Left: [level curves](level-curve.md) of $F(x,y)=x^2+2y^2$, the [unit circle](complex-unit-circle.md) path, and arrows at $t=\pi/4$ for its [velocity vector](velocity-vector.md) and a scaled [gradient](gradient.md). Right: the sampled [function](function-split.md) $F(\gamma(t))=1+\sin^2t$ and its [tangent line](tangent-line.md), of [slope](slope.md) one at that parameter. The displayed gradient arrow is scaled for readability, without changing its direction.

For a [level curve](level-curve.md), $F(\gamma(t))$ is constant, so the [derivative along a curve](derivative-along-a-curve.md) is zero and its [velocity vector](velocity-vector.md) is [orthogonal](orthogonal-vectors.md) to the [gradient](gradient.md). Along other paths, the same formula combines a field's geometry with the observer's motion. [OpenStax, multivariable chain rule and parameter-dependent inputs](https://openstax.org/books/calculus-volume-3/pages/4-5-the-chain-rule).

**Table of contents**

- [Derivative of a vector field dotted with curve velocity](derivative-of-a-vector-field-dotted-with-curve-velocity.md)

## ↑ Ancestors (9)

1. [Multivariable chain rule](multivariable-chain-rule.md)
2. [Chain rule](chain-rule.md)
3. [Derivative](derivative.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Derivative along a curve](derivative-along-a-curve.md)
- [Directional derivative](directional-derivative.md)
- [Scalar field](scalar-field.md)
