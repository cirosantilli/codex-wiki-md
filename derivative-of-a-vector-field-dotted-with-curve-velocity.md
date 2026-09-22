# Derivative of a vector field dotted with curve velocity

↑ **Parent:** [Derivative along a curve](derivative-along-a-curve.md)

For a continuously [differentiable](differentiable-function.md) [vector field](vector-field.md) $W:\mathbb R^n\to\mathbb R^n$ and a twice continuously [differentiable](differentiable-function.md) [parametric curve](parametric-curve.md) $r$, the [product rule](product-rule.md) and [multivariable chain rule](multivariable-chain-rule.md) give

$$
\frac d{dt}\bigl[W(r(t))\cdot r'(t)\bigr]
=r'(t)^TJ_W(r(t))r'(t)+W(r(t))\cdot r''(t),
$$

where $(J_W)_{ij}=\partial_jW_i$ is the [Jacobian matrix](jacobian-matrix.md). Indeed, first differentiate the [dot product](dot-product.md) to obtain $(dW(r(t))/dt)\cdot r'+W(r(t))\cdot r''$, and then substitute $dW(r(t))/dt=J_Wr'$.

The first term describes variation in the sampled [vector field](vector-field.md); the second records the changing [velocity vector](velocity-vector.md) of the [parametric curve](parametric-curve.md). In three dimensions one may take $W=\nabla\times F$ for a sufficiently smooth [vector field](vector-field.md) $F$. The formula then involves first and second spatial [partial derivatives](partial-derivative.md) of $F$ and the [velocity](velocity.md) and [acceleration](acceleration.md) of the [parametric curve](parametric-curve.md). Omitting the second term would be valid only when its [dot product](dot-product.md) vanishes, for example for a straight path with constant [velocity](velocity.md).

## ↑ Ancestors (10)

1. [Derivative along a curve](derivative-along-a-curve.md)
2. [Multivariable chain rule](multivariable-chain-rule.md)
3. [Chain rule](chain-rule.md)
4. [Derivative](derivative.md)
5. [Calculus](calculus-split.md)
6. [Real analysis](real-analysis-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)
