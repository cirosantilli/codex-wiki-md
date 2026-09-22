<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Under the [first-order smoothing approximation](../../../../../first-order-smoothing-approximation.md), neglect the fluctuating product in the [resistive induction equation](../../../../../resistive-induction-equation.md) while retaining its contribution to the mean electromotive force. Since the test field $\mathbf B_0$ is constant and the velocity is a [solenoidal vector field](../../../../../solenoidal-vector-field.md), the fluctuation equation is

$$
\partial_t\mathbf b-\eta\nabla^2\mathbf b=(\mathbf B_0\cdot\nabla)\mathbf u.
$$

Let $a=\eta k^2>0$, $d=a^2+\Omega^2$, and $\mathbf C_j=i(\mathbf B_0\cdot\mathbf k_j)\hat{\mathbf u}_j$. For each [Fourier mode](../../../../../fourier-mode.md), the [diffusion equation](../../../../../diffusion-equation-split.md) becomes a scalar linear relaxation equation applied to each vector component. Take its long-time periodic response, with $\Omega\ne0$. For the first mode,

$$
a\mathbf p_1+\Omega\mathbf q_1=\mathbf C_1,\qquad a\mathbf q_1-\Omega\mathbf p_1=0,
$$

while for the second,

$$
a\mathbf p_2+\Omega\mathbf q_2=0,\qquad a\mathbf q_2-\Omega\mathbf p_2=\mathbf C_2.
$$

Thus **the complex response coefficients** are

$$
\boxed{\mathbf p_1=\frac{a\mathbf C_1}{d},\quad \mathbf q_1=\frac{\Omega\mathbf C_1}{d},\quad
\mathbf p_2=-\frac{\Omega\mathbf C_2}{d},\quad \mathbf q_2=\frac{a\mathbf C_2}{d}.}
$$

They give

$$
\mathbf b=\operatorname{Re}\sum_{j=1}^{2}e^{i\mathbf k_j\cdot\mathbf x}(\mathbf p_j\cos\Omega t+\mathbf q_j\sin\Omega t).
$$

An arbitrary initial fluctuation also contains a homogeneous diffusive transient. In the forced modes this is $\operatorname{Re}\sum_j\mathbf r_j e^{i\mathbf k_j\cdot\mathbf x-a t}$; more general initial modes also diffuse. The displayed harmonic expression is the periodic particular solution after those transients, not the most general solution at finite time. The constants $a,d$ and the factors of $i$ are unchanged by taking the final [real part](../../../../../real-part.md).

To justify the helicity relation, write $\hat{\mathbf u}_j=\mathbf a_j+i\mathbf c_j$ with real vectors. Solenoidality gives $\mathbf k_j\cdot\mathbf a_j=\mathbf k_j\cdot\mathbf c_j=0$. Their [cross product](../../../../../cross-product.md) is parallel to $\mathbf k_j$, and

$$
\frac12\operatorname{Re}(i\hat{\mathbf u}_j^*\times\hat{\mathbf u}_j)
=-\mathbf a_j\times\mathbf c_j=H_j\mathbf k_j,
\qquad
H_j=\frac{\mathbf k_j\cdot\operatorname{Re}(i\hat{\mathbf u}_j^*\times\hat{\mathbf u}_j)}{2k^2}\in\mathbb R.
$$

This is the [helicity vector of a solenoidal Fourier mode](../../../../../helicity-vector-of-a-solenoidal-fourier-mode.md). In these conventions the spatially averaged [kinetic helicity density](../../../../../kinetic-helicity-density.md) of $\operatorname{Re}(\hat{\mathbf u}_je^{i\mathbf k_j\cdot\mathbf x})$ is $-H_jk^2$; the sign is set by the specified cross-product order.

For equal [wavevectors](../../../../../wavevector.md), spatial averaging of two real harmonic fields gives

$$
\left\langle\operatorname{Re}(\mathbf v e^{i\mathbf k\cdot\mathbf x})\times\operatorname{Re}(\mathbf w e^{i\mathbf k\cdot\mathbf x})\right\rangle_x
=\frac12\operatorname{Re}(\mathbf v^*\times\mathbf w).
$$

Time averaging gives another factor $1/2$, because $\langle\cos^2\Omega t\rangle_t=\langle\sin^2\Omega t\rangle_t=1/2$ and the mixed temporal average is zero. Consequently each diagonal mode contributes to the [mean-field electromotive force](../../../../../mean-field-electromotive-force.md)

$$
\mathcal E_j=\frac{a}{4d}(\mathbf B_0\cdot\mathbf k_j)\operatorname{Re}(i\hat{\mathbf u}_j^*\times\hat{\mathbf u}_j)
=\frac{a}{2d}H_j\mathbf k_j(\mathbf k_j\cdot\mathbf B_0).
$$

Distinct modes with $\mathbf k_1\ne\pm\mathbf k_2$ have no spatially averaged cross term. The printed condition also permits the opposite-wavevector case. The possible cross terms still cancel after time averaging: the out-of-phase response coefficients are $\mathbf p_2=-\Omega\mathbf C_2/d$ and $\mathbf q_1=\Omega\mathbf C_1/d$, while integration by parts gives $\langle\mathbf u_1\times(\mathbf B_0\cdot\nabla)\mathbf u_2\rangle_x=\langle\mathbf u_2\times(\mathbf B_0\cdot\nabla)\mathbf u_1\rangle_x$ for the real spatial fields. This handles all the distinct [wavevectors](../../../../../wavevector.md) allowed by the question, assuming the usual periodic-cell or whole-space spatial average.

Thus **the [alpha tensor](../../../../../alpha-tensor.md) is**

$$
\boxed{\alpha_{ij}=\frac{\eta k^2}{2(\Omega^2+\eta^2k^4)}\left(H_1 k_{1i}k_{1j}+H_2 k_{2i}k_{2j}\right),\qquad \boldsymbol{\mathcal E}=\boldsymbol\alpha\mathbf B_0.}
$$

Both averaging factors matter. The [alpha tensor](../../../../../alpha-tensor.md) is real and symmetric, and this contribution vanishes when the mode [kinetic helicity densities](../../../../../kinetic-helicity-density.md) vanish.

For the two perpendicular wavevectors and common $H_1=H_2=H$, put $\alpha_0=\eta H k^4/[2(\Omega^2+\eta^2k^4)]$. Then

$$
\boxed{\boldsymbol\alpha=\alpha_0\operatorname{diag}(1,1,0).}
$$

**[Mean-field dynamo](../../../../../mean-field-dynamo.md) action is possible when $\alpha_0\ne0$ and sufficiently long mean-field wavelengths are allowed.** The missing $zz$ entry does not prevent an [alpha-squared dynamo](../../../../../alpha-squared-dynamo.md). Indeed a slowly varying mean [magnetic field](../../../../../magnetic-field.md) transverse to $z$, with dependence $e^{iKz+\lambda t}$, obeys

$$
\partial_t\overline{\mathbf B}=\nabla\times(\boldsymbol\alpha\overline{\mathbf B})+\eta\nabla^2\overline{\mathbf B},
\qquad
\lambda\begin{pmatrix}\overline B_x\\\overline B_y\end{pmatrix}
=\begin{pmatrix}-\eta K^2&-i\alpha_0K\\i\alpha_0K&-\eta K^2\end{pmatrix}\begin{pmatrix}\overline B_x\\\overline B_y\end{pmatrix}.
$$

The two growth rates are $-\eta K^2\pm\alpha_0K$, so the larger is positive if $0<|K|<|\alpha_0|/\eta$. This supplies a brief constructive reason; scale separation also requires $|K|\ll k$. A spatially uniform test field itself has zero [curl](../../../../../curl.md) of its [mean-field electromotive force](../../../../../mean-field-electromotive-force.md) and does not grow. If $H=0$, or if boundary conditions exclude all unstable long wavelengths, this particular [alpha effect](../../../../../alpha-effect.md) does not yield growth. The conclusion concerns the stated [first-order smoothing approximation](../../../../../first-order-smoothing-approximation.md); no uncomputed turbulent-diffusion correction is assumed.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 318](../../paper-318-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
