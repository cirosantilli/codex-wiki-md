<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Put $v_p(u)=(1,u,\ldots,u^p)^T$ and $w_i(x)=K((x_i-x)/h)$, where $p$ is a nonnegative integer and $h$ is the [smoothing bandwidth](../../../../../smoothing-bandwidth.md). The [local polynomial estimator](../../../../../local-polynomial-regression.md) is the intercept of the [weighted least squares](../../../../../weighted-least-squares.md) fit

$$
\widehat\beta(x)=\mathop{\operatorname{argmin}}_{\beta\in\mathbb R^{p+1}}
\sum_{i=1}^nw_i(x)\{Y_i-\beta^Tv_p((x_i-x)/h)\}^2,
\qquad \widehat m_h(x;p)=\widehat\beta_0(x).
$$

When the [local polynomial Gram matrix](../../../../../local-polynomial-gram-matrix.md) $G_p(x)=\sum_iw_i(x)v_p((x_i-x)/h)v_p((x_i-x)/h)^T$ is invertible, the [normal equations](../../../../../normal-equation.md) give

$$
\boxed{\widehat m_h(x;p)=e_0^TG_p(x)^{-1}\sum_{i=1}^nw_i(x)v_p((x_i-x)/h)Y_i.}
$$

A singular [local polynomial Gram matrix](../../../../../local-polynomial-gram-matrix.md) requires a selection convention and may leave the intercept unidentified; an arbitrary nonnegative [regression kernel](../../../../../kernel-for-nonparametric-regression.md) alone does not guarantee uniqueness. At $p=0$, provided $\sum_iw_i(x)>0$, the [Nadaraya–Watson estimator](../../../../../nadaraya-watson-estimator.md) is

$$
\boxed{\widehat m_h(x)=\frac{\sum_iK((x_i-x)/h)Y_i}{\sum_iK((x_i-x)/h)}.}
$$

Multiplying every weight by $1/h$ changes neither fit.

For the [uniform kernel](../../../../../uniform-smoothing-kernel.md), let $I_x=\{i:|i/n-x|\leq h\}$ and $N_x=|I_x|$. Then $\widehat m_h(x)=N_x^{-1}\sum_{i\in I_x}Y_i$. For $0<h<1/2$ and $x\in[h,1-h]$, the interval $[x-h,x+h]$ is inside $[0,1]$, and the regular design has

$$
N_x\geq\lfloor2nh\rfloor\geq2nh-1\geq nh\qquad(nh\geq1).
$$

The same lower bound holds when the interval starts at zero, despite the absence of the design point zero. In particular the [Nadaraya–Watson estimator](../../../../../nadaraya-watson-estimator.md) is defined throughout the integration interval.

For every [Lipschitz continuous](../../../../../lipschitz-continuity.md) mean function in $\Theta_L$, the [bias of an estimator](../../../../../bias-of-an-estimator.md) and [variance](../../../../../variance-split.md) satisfy

$$
\left|\mathbb E_m\widehat m_h(x)-m(x)\right|
\leq\frac L{N_x}\sum_{i\in I_x}|i/n-x|\leq Lh,
\qquad \operatorname{Var}_m\widehat m_h(x)=\frac{\sigma^2}{N_x}\leq\frac{\sigma^2}{nh}.
$$

Here the [variance](../../../../../variance-split.md) uses the [independence](../../../../../independent-random-variables.md) of the errors in the [fixed-design nonparametric regression](../../../../../fixed-design-nonparametric-regression.md) model. The [bias-variance decomposition of mean squared error](../../../../../bias-variance-decomposition-of-mean-squared-error.md) and [Tonelli theorem](../../../../../tonelli-theorem.md) give a slightly stronger [integrated mean squared error](../../../../../integrated-mean-squared-error.md) bound than required:

$$
\begin{aligned}
\sup_{m\in\Theta_L}\mathbb E_m\int_h^{1-h}\{\widehat m_h(x)-m(x)\}^2\,dx
&\leq(1-2h)\left(L^2h^2+\frac{\sigma^2}{nh}\right)\\
&\leq L^2h^2+\frac{3\sigma^2}{2nh}.
\end{aligned}
$$

Thus

$$
\boxed{\sup_{m\in\Theta_L}\mathbb E_m\int_h^{1-h}\{\widehat m_h(x)-m(x)\}^2\,dx\leq L^2h^2+\frac{3\sigma^2}{2nh}.}
$$

The printed integration interval represents a nonnegative [risk function](../../../../../risk-function.md) for $h\leq1/2$. For $1/2<h\leq1$, the written integral has reversed limits and is nonpositive, making the displayed upper bound trivial; it should not be interpreted as an [integrated mean squared error](../../../../../integrated-mean-squared-error.md) in that range. For $h>1$, evaluation outside $[0,1]$ would additionally require a specified extension of the mean function. The subsequent optimization restricts to $h<1/3$.

Minimizing the stated right side gives

$$
 h_* =\left(\frac{3\sigma^2}{4nL^2}\right)^{1/3},\qquad
 L^2h_*^2+\frac{3\sigma^2}{2nh_*}
 =3\left(\frac34\right)^{2/3}\left(\frac{L\sigma^2}{n}\right)^{2/3}.
$$

For sufficiently large $n$, $nh_*\geq1$ and $h_*<1/3$. For example take $n_0=1+\lceil\max\{1,2L/(\sqrt3\sigma),81\sigma^2/(4L^2)\}\rceil$. Therefore the upper bound holds with

$$
\boxed{C=3\left(\frac34\right)^{2/3}.}
$$

For the lower bound, the PDF has the [mean squared error](../../../../../mean-squared-error.md) $\mathbb E_m[(\widetilde m(x_0)-m(x_0))^2]$; the TeX erroneously moves the square outside the [expected value](../../../../../expected-value.md). The PDF's suggested [smooth bump function](../../../../../smooth-bump-function.md) is $\exp(-1/(1-t^2))\mathbf1_{\{|t|\leq1\}}$, with value zero at the endpoints, rather than the corrupted TeX formula. A triangular alternative suffices because only [Lipschitz continuity](../../../../../lipschitz-continuity.md) is needed.

The [Le Cam two-point lemma](../../../../../le-cam-two-point-lemma.md) says that for two data laws $P_0,P_1$ with parameter separation $\Delta=|\theta_1-\theta_0|$, every estimator $T$ satisfies

$$
\boxed{\max_{j=0,1}\mathbb E_j(T-\theta_j)^2\geq\frac{\Delta^2}{8}\{1-\|P_0-P_1\|_{\mathrm{TV}}\}.}
$$

Indeed, classify according to the nearer parameter value. Misclassification incurs [squared-error loss](../../../../../squared-error-loss.md) at least $\Delta^2/4$, and the sum of the two error probabilities is at least one minus the [total variation distance](../../../../../total-variation-distance.md). Averaging the two [risk functions](../../../../../risk-function.md) proves the stated form.

Let $d=\min(x_0,1-x_0)>0$, $m_0=0$, and use the [two-point lower bound with a triangular bump](../../../../../two-point-lower-bound-with-a-triangular-bump.md)

$$
m_1(x)=L(h-|x-x_0|)_+,
\qquad h=\left(\frac{\sigma^2}{8nL^2}\right)^{1/3}.
$$

Both functions are in $\Theta_L$, and $\Delta=Lh$. Assume first that $h\leq d$ and $nh\geq1$. At most $2nh+1$ design points meet the bump's support. The [Kullback-Leibler divergence between normal distributions](../../../../../kullback-leibler-divergence-between-normal-distributions.md) and [chain rule for relative entropy](../../../../../chain-rule-for-relative-entropy.md) give

$$
D_{\mathrm{KL}}(P_1\Vert P_0)
=\frac1{2\sigma^2}\sum_{i=1}^nm_1(i/n)^2
\leq\frac{L^2h^2(2nh+1)}{2\sigma^2}
\leq\frac{3nL^2h^3}{2\sigma^2}=\frac3{16}.
$$

The [Pinsker's inequality](../../../../../pinsker-s-inequality.md) therefore gives $\|P_1-P_0\|_{\mathrm{TV}}\leq\sqrt{3/32}<1/2$. The [Le Cam two-point lemma](../../../../../le-cam-two-point-lemma.md) yields the [pointwise minimax rate for Lipschitz regression](../../../../../pointwise-minimax-rate-for-lipschitz-regression.md)

$$
\boxed{\inf_{\widetilde m}\sup_{m\in\Theta_L}\mathbb E_m[(\widetilde m(x_0)-m(x_0))^2]
\geq\frac1{64}\left(\frac{L\sigma^2}{n}\right)^{2/3}.}
$$

This universal constant is valid for $n\geq N:=\lceil\max\{1,\sigma^2/(8L^2d^3),2\sqrt2L/\sigma\}\rceil$.

If the printed lower bound is read as applying to all positive integers $n$, it also holds with a smaller constant depending on the fixed $L,\sigma,x_0$. For $n<N$, use the constant mean functions $m_0=0$ and $m_1=\sigma/\sqrt n$. They have [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) $1/2$, so [Pinsker's inequality](../../../../../pinsker-s-inequality.md) and the [Le Cam two-point lemma](../../../../../le-cam-two-point-lemma.md) give [minimax risk](../../../../../minimax-risk.md) at least $\sigma^2/(16n)$. Combining the two ranges gives the explicit all-$n$ choice

$$
\boxed{c=\min\left\{\frac1{64},\ \frac1{16}\left(\frac{\sigma^2}{NL^2}\right)^{1/3}\right\}>0.}
$$

The universal asymptotic constant and this parameter-dependent all-$n$ constant are distinct conventions; the latter supplies the assertion without inserting an unstated large-$n$ restriction.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
