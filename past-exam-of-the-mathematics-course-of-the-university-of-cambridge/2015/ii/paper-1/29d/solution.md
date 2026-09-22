<h1 id="29d/solution">Solution</h1>

↑ **Parent:** [29D](../29d.md)

A [Hamiltonian evolution equation](../../../../../hamiltonian-evolution-equation.md) has the form $u_t=J\,\delta H/\delta u$, where $H$ is a functional and the Hamiltonian operator $J$ induces a bilinear antisymmetric bracket obeying the Jacobi identity. For a local functional $H=\int h(u,u_x,\ldots)dx$, its [variational derivative](../../../../../variational-derivative.md) is the coefficient of a test perturbation after all integrations by parts.

Linearizing about zero drops the cubic term and gives $u_t+u_{xxx}=0$. A plane wave $e^{i(kx-\omega t)}$ has **$\omega=-k^3$**, so phase velocity $-k^2$ and group velocity $-3k^2$ depend on wavenumber. This proves small-amplitude [wave dispersion](../../../../../wave-dispersion.md).

Take

$$
\boxed{H[u]=\frac12\int(u_x^2+u^4)dx,\qquad J=\partial_x}.
$$

Then $\delta H/\delta u=-u_{xx}+2u^3$ and $J\delta H/\delta u=-u_{xxx}+6u^2u_x$, the required flow. On sufficiently smooth functionals define the [Poisson bracket](../../../../../poisson-bracket.md)

$$
\boxed{\{F,G\}=\int\frac{\delta F}{\delta u}\,\partial_x\frac{\delta G}{\delta u}\,dx}.
$$

Variational differentiation and integration are linear, proving linearity in both arguments. Integration by parts and the rapid decay give $\{F,G\}=-\{G,F\}$. The constant skew differential operator $\partial_x$ also satisfies the Hamiltonian Jacobi condition, so this is indeed a [Poisson bracket](../../../../../poisson-bracket.md).

Along the flow, the functional chain rule gives $dI/dt=\int(\delta I/\delta u)u_tdx=\{I,H\}$. Thus an autonomous functional is a [first integral](../../../../../first-integral.md) exactly when its bracket with $H$ vanishes identically on phase space. Direct multiplication of the equation by $2u$ gives

$$
\partial_t(u^2)= -2uu_{xxx}+12u^3u_x
=-\partial_x(2uu_{xx}-u_x^2-3u^4).
$$

Integrating the resulting [local conservation law](../../../../../local-conservation-law.md) over the line makes the boundary flux vanish. Hence $I=\int u^2dx$ is conserved and **$\{I,H\}=0$**. As a direct check, its [variational derivative](../../../../../variational-derivative.md) is $2u$, and integration by parts makes $\int2u(-u_{xxx}+6u^2u_x)dx=0$.

## ↑ Ancestors (10)

1. [29D](../29d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
