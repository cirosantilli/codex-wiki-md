<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a regular two-parameter model, write $\psi$ for the parameter of interest and $\lambda$ for the [nuisance parameter](../../../../../nuisance-parameter.md). If $u_\psi,u_\lambda$ are its [score functions](../../../../../informant-function.md), the parameters are [orthogonal statistical parameters](../../../../../orthogonal-statistical-parameters.md) when the cross entry of the expected [Fisher information matrix](../../../../../fisher-information-matrix.md) vanishes:

$$
\boxed{I_{\psi\lambda}=\mathbb E(u_\psi u_\lambda)=0.}
$$

This condition may hold at a particular parameter value or throughout the parameter domain. It concerns the information geometry, not exact independence of finite-sample estimators. Under regular asymptotic efficiency, a diagonal information matrix gives zero first-order asymptotic covariance.

An [interest-respecting reparametrization](../../../../../interest-respecting-reparametrization.md) leaves $\psi$ unchanged, or replaces it by a one-to-one function of $\psi$ alone, while changing the nuisance coordinate by a smooth invertible transformation which may depend on both old parameters. Thus it preserves the level sets of the inferential target. Without loss of generality, keep $\psi$ itself and write the old nuisance as $\lambda=g(\psi,\eta)$, where $\eta$ is the new nuisance coordinate and $g_\eta\ne0$.

The [chain rule](../../../../../chain-rule.md) for the [log-likelihood](../../../../../log-likelihood.md) gives new [score functions](../../../../../informant-function.md)

$$
u_\psi^{\rm new}=u_\psi+g_\psi u_\lambda,\qquad u_\eta^{\rm new}=g_\eta u_\lambda.
$$

Their expected cross product is

$$
I_{\psi\eta}^{\rm new}=g_\eta(I_{\psi\lambda}+g_\psi I_{\lambda\lambda}).
$$

Setting this to zero, with $I_{\lambda\lambda}>0$, gives the [orthogonalization equation for two statistical parameters](../../../../../orthogonalization-equation-for-two-statistical-parameters.md)

$$
\boxed{\left.\frac{\partial\lambda}{\partial\psi}\right|_\eta=-\frac{I_{\psi\lambda}(\psi,\lambda)}{I_{\lambda\lambda}(\psi,\lambda)}.}
$$

Solve this [ordinary differential equation](../../../../../ordinary-differential-equation.md) along curves of constant $\eta$, using $\eta$ to label distinct initial conditions. Smooth local solutions with nonzero transverse derivative produce an invertible [interest-respecting reparametrization](../../../../../interest-respecting-reparametrization.md). This informal construction identifies precisely which derivative is held at fixed new nuisance coordinate.

For the given positive-shape [generalized Pareto distribution](../../../../../generalized-pareto-distribution.md), its one-observation [log-likelihood](../../../../../log-likelihood.md) is

$$
\ell(\psi,\sigma)=-\log\sigma-\left(1+\frac1\psi\right)\log\left(1+\frac{\psi y}{\sigma}\right).
$$

Define $L=\log(1+\psi Y/\sigma)$ and $D=e^{-L}$. The density transformation $y=\sigma(e^L-1)/\psi$, $dy/dL=\sigma e^L/\psi$, gives

$$
f_L(l)=\frac1\psi e^{-l/\psi},\qquad l>0.
$$

Thus $L$ has an [exponential distribution](../../../../../exponential-distribution.md) of mean $\psi$. Direct differentiation of the original [log-likelihood](../../../../../log-likelihood.md), holding the other original parameter fixed, gives

$$
u_\psi=\frac{L-(1+\psi)(1-D)}{\psi^2},\qquad u_\sigma=\frac{1-(1+\psi)D}{\psi\sigma}.
$$

The following exponential integrals determine their expected products:

$$
\mathbb EL=\psi,\quad\mathbb EL^2=2\psi^2,\quad\mathbb ED=\frac1{1+\psi},\quad\mathbb ED^2=\frac1{1+2\psi},\quad\mathbb E(LD)=\frac{\psi}{(1+\psi)^2}.
$$

For example, $\mathbb E e^{-kL}=(1+k\psi)^{-1}$ follows by integrating the exponential density, and differentiating this integral in $k$ gives $\mathbb E(Le^{-kL})=\psi/(1+k\psi)^2$. These formulas also give $\mathbb E u_\psi=\mathbb E u_\sigma=0$.

For clarity, the nuisance information and cross information can be calculated explicitly. Put $a=1+\psi$. Then

$$
I_{\sigma\sigma}=\frac{1-2a\mathbb ED+a^2\mathbb ED^2}{\psi^2\sigma^2}=\frac1{\sigma^2(1+2\psi)}.
$$

Using $\mathbb E[L-a+aD]=0$, the cross product is

$$
I_{\psi\sigma}=-\frac{a}{\psi^3\sigma}\{\mathbb E(LD)-a\mathbb ED+a\mathbb ED^2\}=\frac1{\sigma(1+\psi)(1+2\psi)}.
$$

The same moments give $I_{\psi\psi}=\psi^{-4}\mathbb E[L-a+aD]^2=2/[(1+\psi)(1+2\psi)]$. Therefore the [Fisher information matrix](../../../../../fisher-information-matrix.md) for one observation is

$$
I(\psi,\sigma)=\frac1{1+2\psi}\begin{pmatrix}\dfrac2{1+\psi}&\dfrac1{\sigma(1+\psi)}\\[4pt]\dfrac1{\sigma(1+\psi)}&\dfrac1{\sigma^2}\end{pmatrix}.
$$

In particular, $I_{\psi\sigma}>0$ for every admissible pair, proving **the original shape and scale parameters are not orthogonal**. No finite-mean assumption on $Y$ was needed: the transformed logarithm $L$ and the bounded variable $D$ have the required integrable score products even when the Pareto mean is infinite.

The [orthogonalization equation for two statistical parameters](../../../../../orthogonalization-equation-for-two-statistical-parameters.md) now becomes

$$
\left.\frac{\partial\sigma}{\partial\psi}\right|_\eta=-\frac\sigma{1+\psi}.
$$

Integration along a constant-$\eta$ curve gives $\sigma(1+\psi)=\eta$. Hence a global [interest-respecting reparametrization](../../../../../interest-respecting-reparametrization.md) is

$$
\boxed{(\psi,\sigma)\longmapsto(\psi,\eta),\qquad\eta=\sigma(1+\psi).}
$$

It is smoothly invertible on the entire positive parameter domain, with inverse $\sigma=\eta/(1+\psi)$. The [Fisher information matrix](../../../../../fisher-information-matrix.md) transforms as $J^TIJ$, where

$$
J=\frac{\partial(\psi,\sigma)}{\partial(\psi,\eta)}=\begin{pmatrix}1&0\\-\eta/(1+\psi)^2&1/(1+\psi)\end{pmatrix}.
$$

Substitution gives

$$
\boxed{I(\psi,\eta)=\begin{pmatrix}(1+\psi)^{-2}&0\\0&[\eta^2(1+2\psi)]^{-1}\end{pmatrix}.}
$$

This verifies the [orthogonal shape and scale for a generalized Pareto distribution](../../../../../orthogonal-shape-and-scale-for-a-generalized-pareto-distribution.md) directly, as well as by the differential equation. For an iid sample, every information entry is multiplied by the sample size, so the same [parameter orthogonality](../../../../../orthogonal-statistical-parameters.md) remains valid.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
