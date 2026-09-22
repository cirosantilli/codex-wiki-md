# Derivative of a local inverse map

↑ **Parent:** [Inverse function theorem](inverse-function-theorem.md)

For the [continuously differentiable](continuously-differentiable-function.md) [inverse function](inverse-function.md) $g$ supplied by the [inverse function theorem](inverse-function-theorem.md), the [chain rule](chain-rule.md) applied to $f(g(y))=y$ gives

$$
Df(g(y))Dg(y)=I,\qquad
Dg(y)=[Df(g(y))]^{-1}.
$$

Here $I$ is the [identity matrix](identity-matrix.md). The [matrix inverse](matrix-inverse.md) is taken at the recovered input $g(y)$, not at the output $y$. In one dimension this is the [inverse function rule](inverse-function-rule.md) $g'(y)=1/f'(g(y))$.

The formula also describes sensitivity. For a small output perturbation $h$, [differentiability](differentiability.md) gives $g(y+h)-g(y)=Dg(y)h+o(\|h\|)$. A large [operator norm](operator-norm.md) of $Dg(y)$ permits large amplification in some directions. In the [square root](square-root.md) example, $g'(y)=1/(2\sqrt y)$ grows without bound as positive $y$ approaches zero. Existence of a local [inverse function](inverse-function.md) therefore does not imply that recovery is insensitive to measurement error.

## ↑ Ancestors (9)

1. [Inverse function theorem](inverse-function-theorem.md)
2. [Differentiable map](differentiable-map.md)
3. [Multivariable calculus](multivariable-calculus.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Inverse function theorem](inverse-function-theorem.md)
