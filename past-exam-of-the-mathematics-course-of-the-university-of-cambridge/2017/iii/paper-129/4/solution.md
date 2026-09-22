<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Uniform [expectations](../../../../../expected-value.md) require nonempty [finite sets](../../../../../finite-set.md); assume this throughout the analytic argument. For [real-valued functions](../../../../../real-valued-function.md) on $X\times Y$, define the [box norm](../../../../../box-norm.md) by

$$
\boxed{\|f\|_{\square}=
\left(\mathbb E_{x_0,x_1\in X\atop y_0,y_1\in Y}
\prod_{i,j=0}^1f(x_i,y_j)\right)^{1/4}.}
$$

All four variables are sampled as [independent random variables](../../../../../independent-random-variables.md) with replacement, so repeated coordinates are included. The defining fourth power equals

$$
\mathbb E_{y_0,y_1}\left(\mathbb E_xf(x,y_0)f(x,y_1)\right)^2\geq0.
$$

If it vanishes, every summand vanishes. In particular, the terms $y_0=y_1=y$ give $\mathbb E_x f(x,y)^2=0$ for each $y$, so $f=0$. [Absolute homogeneity of a norm](../../../../../absolute-homogeneity-of-a-norm.md) follows directly: $\|af\|_{\square}=|a|\|f\|_{\square}$.

For the [triangle inequality](../../../../../triangle-inequality.md), prove the mixed [box Cauchy-Schwarz inequality](../../../../../box-cauchy-schwarz-inequality.md). Write

$$
\Lambda(f_{00},f_{01},f_{10},f_{11})=
\mathbb E_{x_0,x_1,y_0,y_1}\prod_{i,j=0}^1f_{ij}(x_i,y_j).
$$

Separating the two $y$ averages and applying the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) in $(x_0,x_1)$ gives

$$
|\Lambda|\leq A(f_{00},f_{10})^{1/2}A(f_{01},f_{11})^{1/2},
\quad A(f,g)=\mathbb E_{x,x'}\left(\mathbb E_y f(x,y)g(x',y)\right)^2.
$$

Expanding the square and reversing the order of finite sums,

$$
A(f,g)=\mathbb E_{y,y'}
\left(\mathbb E_xf(x,y)f(x,y')\right)
\left(\mathbb E_xg(x,y)g(x,y')\right)
\leq\|f\|_{\square}^2\|g\|_{\square}^2,
$$

by a second [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). Thus $|\Lambda|\leq\prod_{i,j}\|f_{ij}\|_{\square}$. Expand $\Lambda(f+g,f+g,f+g,f+g)$ into its sixteen multilinear terms and apply this bound to each term. Their upper bounds sum to $(\|f\|_{\square}+\|g\|_{\square})^4$. Taking fourth roots yields the [triangle inequality](../../../../../triangle-inequality.md). Together with [definiteness of a norm](../../../../../definiteness-of-a-norm.md) and [absolute homogeneity of a norm](../../../../../absolute-homogeneity-of-a-norm.md), this proves **the [box norm](../../../../../box-norm.md) is a [norm](../../../../../norm.md).** Complex [functions](../../../../../function-split.md) require conjugates and are outside the printed real-valued convention.

For the [bilinear correlation bound for the box norm](../../../../../bilinear-correlation-bound-for-the-box-norm.md), use the normalized [L2 norm](../../../../../l2-norm.md): let $B=\mathbb E_{x,y}f(x,y)u(x)v(y)$ and $\|u\|_2^2=\mathbb E_xu(x)^2$, $\|v\|_2^2=\mathbb E_yv(y)^2$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) in $y$ gives

$$
|B|^2\leq\|v\|_2^2\mathbb E_y\left(\mathbb E_x f(x,y)u(x)\right)^2.
$$

The remaining factor is $\mathbb E_{x,x'}u(x)u(x')\mathbb E_y f(x,y)f(x',y)$. By the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) in $(x,x')$, its magnitude is at most

$$
\left(\mathbb E_{x,x'}u(x)^2u(x')^2\right)^{1/2}
\left(\mathbb E_{x,x'}\left(\mathbb E_yf(x,y)f(x',y)\right)^2\right)^{1/2}
=\|u\|_2^2\|f\|_{\square}^2.
$$

Taking square roots proves

$$
\boxed{|\mathbb E_{x,y}f(x,y)u(x)v(y)|\leq\|f\|_{\square}\|u\|_2\|v\|_2.}
$$

For the [tripartite graph](../../../../../tripartite-graph.md), assume its parts are nonempty and write $g_{XY},g_{YZ},g_{XZ}$ for its adjacency [indicator functions](../../../../../indicator-function.md). Let $f=g_{XY}-\alpha$, so $\|f\|_{\square}\leq c$. The normalized [triangle count](../../../../../triangle-count.md) is

$$
\tau=\mathbb E_{x,y,z}(\alpha+f(x,y))g_{YZ}(y,z)g_{XZ}(x,z).
$$

The constant-degree hypothesis is exactly $\mathbb E_y g_{YZ}(y,z)=\beta$ for each $z$. Therefore the contribution of the constant $\alpha$ is

$$
\alpha\mathbb E_z\left(\mathbb E_y g_{YZ}(y,z)\right)
\left(\mathbb E_x g_{XZ}(x,z)\right)=\alpha\beta\gamma.
$$

For fixed $z$, apply the [bilinear correlation bound for the box norm](../../../../../bilinear-correlation-bound-for-the-box-norm.md) with $u_z(x)=g_{XZ}(x,z)$ and $v_z(y)=g_{YZ}(y,z)$. Since these are [indicator functions](../../../../../indicator-function.md), $\|v_z\|_2^2=\beta$ and $\|u_z\|_2^2=d_X(z)$, the fraction of $X$ adjacent to $z$. Averaging and applying the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) in $z$ gives the sharper [triangle counting with one box-uniform pair and constant opposite degree](../../../../../triangle-counting-with-one-box-uniform-pair-and-constant-opposite-degree.md) estimate

$$
|\tau-\alpha\beta\gamma|
\leq c\sqrt\beta\,\mathbb E_z\sqrt{d_X(z)}
\leq c\sqrt{\beta\,\mathbb E_zd_X(z)}
=c\sqrt{\beta\gamma}\leq c.
$$

Multiplying by $|X||Y||Z|$ yields

$$
\boxed{\bigl|T(G)-\alpha\beta\gamma\,|X|\,|Y|\,|Z|\bigr|
\leq c\sqrt{\beta\gamma}\,|X||Y||Z|
\leq3c|X||Y||Z|.}
$$

The middle bound also handles $\beta=0$ or $\gamma=0$, when the [triangle count](../../../../../triangle-count.md) is zero.

To connect explicitly with the suggested expansion, put $f_2=g_{YZ}-\beta$, $f_3=g_{XZ}-\gamma$. Both have overall mean zero, and $\mathbb E_y f_2(y,z)=0$ for every $z$. Consequently $\mathbb E_{x,y,z}f_2(y,z)f_3(x,z)=0$; all terms with constant $\alpha$ reduce to $\alpha\beta\gamma$. The terms containing $f$ combine into the single error just estimated. This is where the exact degree assumption is used. If any part is empty the [triangle count](../../../../../triangle-count.md) itself is zero, but the printed uniform [expectations](../../../../../expected-value.md) and [edge density of a bipartite graph](../../../../../edge-density-of-a-bipartite-graph.md) values would be undefined; the nonempty-parts convention must therefore be stated rather than dividing by zero.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 129](../../paper-129-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
