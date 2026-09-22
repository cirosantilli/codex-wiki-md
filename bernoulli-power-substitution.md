# Bernoulli power substitution

↑ **Parent:** [Bernoulli differential equation](bernoulli-differential-equation.md)

For arbitrary real $n\ne0,1$, work first on an [interval](interval-mathematics.md) where $y>0$. Define [exponentiation](exponentiation.md) by $y^r=\exp(r\log y)$, using the real [logarithm](logarithm.md). The change of variable is differentiable and invertible there, and the [chain rule](chain-rule.md) gives

$$
z'= (1-n)y^{-n}y',\qquad y=z^{1/(1-n)},\quad z>0.
$$

Multiplying the [Bernoulli differential equation](bernoulli-differential-equation.md) by $(1-n)y^{-n}$ yields the [first-order linear differential equation](first-order-linear-differential-equation.md)

$$
z'+(1-n)P(x)z=(1-n)Q(x).
$$

This is an exact transformation of nonzero [solutions of a differential equation](solution-of-a-differential-equation.md) on the chosen branch; it is valid far from any reference state and does not discard higher powers as a local [linearization](linearization.md) would.

Given the [initial condition](initial-condition.md) $y(x_0)=y_0>0$, the [integrating factor](integrating-factor.md) and transformed [solution of a differential equation](solution-of-a-differential-equation.md) are

$$
\mu(x)=\exp\!\left((1-n)\int_{x_0}^xP(s)\,ds\right),\qquad z(x)=\frac{y_0^{1-n}+(1-n)\int_{x_0}^x\mu(s)Q(s)\,ds}{\mu(x)}.
$$

The [product rule](product-rule.md) verifies $(\mu z)'=(1-n)\mu Q$. Recover $y=z^{1/(1-n)}$ only on the [connected component](connected-component.md) of $\{x:z(x)>0\}$ containing $x_0$, inside the original coefficient [interval](interval-mathematics.md). The [first-order linear differential equation](first-order-linear-differential-equation.md) can have a longer existence [interval](interval-mathematics.md) than this inverse transformation allows.[Notes on Diffy Qs, §1.4 Linear equations and the integrating factor: product derivative, formula (1.4), and Remark 1.4.1 on existence throughout a coefficient-continuity interval](notes-on-diffy-qs-differential-equations-for-engineers-by-jiri-lebl/1-4-linear-equations-and-the-integrating-factor.md)

Negative values need a separately justified real branch. For [integer](integer-split.md) $n$, the required powers are real and differentiable for $y<0$ too, but the inverse must retain the sign selected by the [initial condition](initial-condition.md). For $n=3$, $z=y^{-2}>0$ represents either $y=+1/\sqrt z$ or $y=-1/\sqrt z$; both [square roots](square-root.md) are taken of positive $z$. For $n=2$, $z=1/y$ retains the sign directly. For a general noninteger exponent, use the positive branch unless a specific differentiable real negative branch has been established. Never evaluate a real fractional power of a negative value merely because the linear formula has become negative.

Division by $y^n$ excludes $y=0$. When $n>0$ and the original real power is defined at zero, $y\equiv0$ is an additional [solution of a differential equation](solution-of-a-differential-equation.md) and must be checked in the original equation. When $n<0$, the equation as written is undefined at zero. On a positive branch the right-hand side is [locally Lipschitz](locally-lipschitz-function.md) in $y$, so the [Picard-Lindelöf theorem](picard-lindelof-theorem.md) gives local uniqueness. At zero, the same hypothesis needs a fresh check: it holds for the polynomial $n=2$ example, whereas for $0<n<1$ a nonzero power coefficient prevents local [Lipschitz continuity](lipschitz-continuity.md) there. If $z\downarrow0$, the inverse sends $y\to\infty$ for $n>1$, but sends $y\downarrow0$ for $0<n<1$. The latter endpoint can lead to [finite-time extinction in a sublinear Bernoulli equation](finite-time-extinction-in-a-sublinear-bernoulli-equation.md), where the original equation determines how to join to zero.

## ↑ Ancestors (7)

1. [Bernoulli differential equation](bernoulli-differential-equation.md)
2. [Ordinary differential equation](ordinary-differential-equation.md)
3. [Differential equation](differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Bernoulli differential equation](bernoulli-differential-equation.md)
- [Reciprocal Bernoulli equation with finite-time blowup](reciprocal-bernoulli-equation-with-finite-time-blowup.md)
