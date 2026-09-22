<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a fixed [polytropic index](../../../../../../polytropic-index.md) $n>0$ and fixed equation-of-state constant $K$, let $\xi_1$ be the first zero of the regular [Lane-Emden equation](../../../../../../lane-emden-equation.md) solution. A finite-radius model requires such a zero; for the usual nonnegative indices this holds for $n<5$. The surface radius and mass follow from $r=\alpha\xi$ and $\rho=\rho_c\theta^n$:

$$
R=\alpha\xi_1,\qquad M=4\pi\alpha^3\rho_c\int_0^{\xi_1}\xi^2\theta^n\,d\xi=4\pi\alpha^3\rho_c[-\xi_1^2\theta'(\xi_1)].
$$

The last equality integrates the [Lane-Emden equation](../../../../../../lane-emden-equation.md); define the positive [Lane-Emden surface mass constant](../../../../../../lane-emden-surface-mass-constant.md) $\omega_n=-\xi_1^2\theta'(\xi_1)$. Substituting $\alpha=C_1\rho_c^{(1-n)/(2n)}$ gives

$$
R=C_1\xi_1\rho_c^{(1-n)/(2n)},\qquad M=4\pi C_1^3\omega_n\rho_c^{(3-n)/(2n)}.
$$

The central-density exponents cancel when the required powers are taken. Thus the [polytropic mass-radius relation](../../../../../../polytropic-mass-radius-relation.md) is

$$
\boxed{M^{n-1}R^{3-n}=C_2=(4\pi C_1^3\omega_n)^{n-1}(C_1\xi_1)^{3-n}.}
$$

It is independent of $\rho_c$, with $n,K$ and composition held fixed. For $n=1$ the radius is fixed; for $n=3$ the mass is fixed. These limiting powers need no division by a vanishing exponent.

For $n=0$, the literal pressure-density power and the supplied expression for $\alpha$ are singular. Interpret this case separately as an [incompressible planetary interior](../../../../../../incompressible-planetary-interior.md) with constant density. Then $M=4\pi\rho R^3/3$, or **$R\propto M^{1/3}$** at fixed density. A weakly compressed rocky body, or a rough uniform-density approximation to [Earth](../../../../../../earth.md), is an example; realistic terrestrial planets are stratified and compressible.

For $n=3/2$, $P\propto\rho^{5/3}$. This describes a cold nonrelativistic degenerate electron gas of fixed composition, or a fully convective monatomic [ideal gas](../../../../../../ideal-gas.md) at fixed [entropy](../../../../../../entropy.md). Examples are a nonrelativistic [white dwarf](../../../../../../white-dwarf.md), a sufficiently cooled partly degenerate [brown dwarf](../../../../../../brown-dwarf.md) as an approximation, and an approximately fully convective low-mass star for the ideal-gas version. The fixed-$K$ scaling is **$R\propto M^{-1/3}$**. It must not be applied to an entire main-sequence stellar sequence with different entropies; the [entropy dependence of a polytropic mass-radius relation](../../../../../../entropy-dependence-of-a-polytropic-mass-radius-relation.md) explains the distinction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
