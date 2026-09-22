# Paper 47

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper47.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper47.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the unbiased [sample covariance matrix](../../../variance.md#sample-covariance-matrix)

$$
S=\frac1{n-1}\sum_{j=1}^n(X_j-\bar X)(X_j-\bar X)^T,
$$

and assume $\Sigma$ is [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form) and $n>p$, so $S$ is invertible almost surely. For a nonzero fixed direction $a$, the observations $Y_j=a^TX_j$ have mean $a^T\mu$ and [variance](../../../variance.md) $a^T\Sigma a$. Their squared [Student t-test](../../../statistical-modelling.md#student-s-t-test) statistic for the projected null mean is

$$
t_a^2=\frac{n\{a^T(\bar X-\mu_0)\}^2}{a^TSa}.
$$

Put $b=\bar X-\mu_0$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
(a^Tb)^2=\{(S^{1/2}a)^T(S^{-1/2}b)\}^2
\le(a^TSa)(b^TS^{-1}b),
$$

with equality when $a$ is proportional to $S^{-1}b$, if $b\ne0$. For $b=0$ every projected statistic is zero. Maximizing the squared discrepancy over directions therefore gives [Hotelling's T-squared statistic](../../../statistical-modelling.md#hotelling-s-t-squared-statistic):

$$
\boxed{T^2=\max_{a\ne0}t_a^2=n(\bar X-\mu_0)^TS^{-1}(\bar X-\mu_0).}
$$

This uses the squared generalized [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient). The preliminary formula on the printed cover has an unsquared numerator and is not valid as written: setting $a=tC^{-1}b$ makes that ratio $1/t$ for $b\ne0$, so it is unbounded. The displayed Cauchy-Schwarz argument supplies the needed corrected identity independently.

Under the null, let $Z=\sqrt n(\bar X-\mu_0)$ and $C=(n-1)S$. Then $Z\sim N_p(0,\Sigma)$, $C\sim W_p(n-1,\Sigma)$, and $Z,C$ are independent. To see these sample properties, apply an orthogonal transformation to the $n$ observation indices with first row $n^{-1/2}(1,\ldots,1)$. Its first centered row is $Z$; its other $n-1$ rows are independent $N_p(0,\Sigma)$ residual contrasts, independent of the first. Their outer products sum to $C$, establishing the [Wishart distribution](../../../probability-theory.md#wishart-distribution) and [independence](../../../random-variable.md#independent-random-variables).

Since $T^2=(n-1)Z^TC^{-1}Z$, use the supplied Gaussian-Wishart quadratic-form law with $k=n-1$ to obtain

$$
\boxed{\frac{n-p}{p(n-1)}T^2\sim F_{p,n-p}\quad\text{under }H_0.}
$$

Thus a level-$\eta$ test rejects when this scaled statistic exceeds the $(1-\eta)$ quantile of the [F-distribution](../../../continuous-probability-distribution.md#f-distribution). The Gaussian-Wishart law requires [independence](../../../random-variable.md#independent-random-variables); it holds here because of the orthogonal sample decomposition. Its printed use of $X$ instead of the introduced $Z$ is a notational slip. A fixed-direction Student law alone would not calibrate the maximized statistic, because its maximizing direction depends on the sample.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Transform each observation to $Y_j=A^TX_j$. If $A^T$ has full row [rank](../../../linear-algebra.md#rank-one-quadratic-form) $m$, the transformed sample is [multivariate normal](../../../probability-and-statistics.md#multivariate-normal-distribution) with mean $A^T\mu$ and [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form) [covariance matrix](../../../variance.md#covariance-matrix) $A^T\Sigma A$. Its [sample mean](../../../variance.md#sample-mean) is $A^T\bar X$ and its unbiased [sample covariance matrix](../../../variance.md#sample-covariance-matrix) is $A^TSA$. The [Hotelling test of linear hypotheses](../../../statistical-modelling.md#hotelling-test-of-linear-hypotheses) therefore uses

$$
\boxed{T_A^2=n(A^T\bar X)^T(A^TSA)^{-1}(A^T\bar X),\qquad
\frac{n-m}{m(n-1)}T_A^2\sim F_{m,n-m}\text{ under }H_0.}
$$

Here $n>m$ is required. Reject for a large scaled statistic using the relevant upper [F-distribution](../../../continuous-probability-distribution.md#f-distribution) quantile. If the rows of $A^T$ are dependent, choose a basis for their row space, use that basis as the contrast matrix, and replace $m$ by its [rank](../../../linear-algebra.md#rank-one-quadratic-form) $r$. The null hypothesis is unchanged, but redundant contrasts must not be treated as independent dimensions. [Rank](../../../linear-algebra.md#rank-one-quadratic-form) zero gives no restrictions and hence no nontrivial test.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

At equal spacing $h$, the adjacent increments of an affine mean profile are all $\beta h$. Their differences are therefore zero. Define the $(p-2)\times p$ matrix $B$ whose row associated with the interior time $i$ has coefficients $1,-2,1$ in columns $i-1,i,i+1$. Then

$$
(B\mu)_{i-1}=\mu_{i-1}-2\mu_i+\mu_{i+1}=0.
$$

Conversely these equations make all adjacent first differences equal, so $\mu_i$ is affine in $i$, equivalently affine in the equally spaced times. Thus the restriction is exactly $B\mu=0$, not just a necessary condition. Its [null space](../../../linear-algebra.md#kernel-of-a-linear-map) has basis $\mathbf1$ and $t=(t_1,\ldots,t_p)^T$, so $B$ has [rank](../../../linear-algebra.md#rank-one-quadratic-form) $r=p-2$.

For $p\ge3$ and $n>r$, the [second-difference test of a linear mean profile](../../../statistical-modelling.md#second-difference-test-of-a-linear-mean-profile) is the [Hotelling test of linear hypotheses](../../../statistical-modelling.md#hotelling-test-of-linear-hypotheses) with

$$
\boxed{T_B^2=n(B\bar X)^T(BSB^T)^{-1}(B\bar X),\qquad
\frac{n-r}{r(n-1)}T_B^2\sim F_{r,n-r}.}
$$

Reject the affine-profile hypothesis when the scaled statistic exceeds its level-$\eta$ upper [F-distribution](../../../continuous-probability-distribution.md#f-distribution) critical value. This removes the nuisance intercept and slope without estimating them separately.

For unequal ordered distinct times, put $h_i=t_{i+1}-t_i>0$ and replace each second-difference row by the adjacent-slope contrast

$$
\frac{\mu_{i+1}-\mu_i}{h_i}-\frac{\mu_i-\mu_{i-1}}{h_{i-1}}.
$$

Its three coefficients are $1/h_{i-1}$, $-(1/h_{i-1}+1/h_i)$ and $1/h_i$. Vanishing means all adjacent slopes agree, again giving [null space](../../../linear-algebra.md#kernel-of-a-linear-map) $\operatorname{span}(\mathbf1,t)$ and [rank](../../../linear-algebra.md#rank-one-quadratic-form) $p-2$. Use this new $B$ in the same statistic and null distribution. For $p\le2$, every mean profile at distinct times is affine, so there is no lack-of-linearity restriction to test.

## 2

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For an integrable real function $g$, let $R_- =\{x:g(x)<0\}$. For every measurable region $R$,

$$
\int_Rg-\int_{R_-}g
=\int_{R\setminus R_-}g-\int_{R_-\setminus R}g\ge0.
$$

The first term is nonnegative because $g\ge0$ there, and the integral subtracted in the second term is nonpositive. Hence **the negative set minimizes the integral**. Including or excluding any points where $g=0$ has no effect; changes on null sets do not matter either. This is the [minimum-integral decision region](../../../statistical-inference.md#minimum-integral-decision-region) principle. Integrability ensures the subtraction is defined, and it holds automatically for the weighted differences of [probability density functions](../../../continuous-probability-distribution.md#probability-density-function) used below.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

There are two disjoint ways to make an error: an individual from class one falls outside $R_1$, or an individual from class two falls inside $R_1$. The [law of total probability](../../../probability-theory.md#law-of-total-probability) gives

$$
\boxed{P_{\mathrm{error}}=
\pi_1\int_{R_1^c}f_1(x)\,dx+(1-\pi_1)\int_{R_1}f_2(x)\,dx.}
$$

Since $f_1$ integrates to one, this also equals

$$
\pi_1+\int_{R_1}\bigl((1-\pi_1)f_2(x)-\pi_1f_1(x)\bigr)\,dx.
$$

This form isolates the only term changed by choosing the decision region.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Apply the [minimum-integral decision region](../../../statistical-inference.md#minimum-integral-decision-region) principle to $g(x)=\pi_2f_2(x)-\pi_1f_1(x)$. The optimal [Bayes classifier](../../../statistical-inference.md#bayes-classifier) chooses class one when $\pi_1f_1(x)>\pi_2f_2(x)$, and class two for the reverse inequality. Ties can be assigned either way. An everywhere valid discriminant score is

$$
\boxed{\delta(x)=\pi_1f_1(x)-\pi_2f_2(x),\qquad\text{choose class one if }\delta(x)>0.}
$$

Where both weighted densities are positive one may equivalently use $\log(\pi_1f_1(x)/(\pi_2f_2(x)))$ and threshold zero. This chooses the largest posterior class probability, because both posterior probabilities have the same positive mixture-density denominator.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

With zero cost for correct assignments, the total expected misclassification cost is

$$
L(R_1)=c(2\mid1)\pi_1\int_{R_1^c}f_1+
 c(1\mid2)\pi_2\int_{R_1}f_2.
$$

The part depending on $R_1$ is the integral of $c(1\mid2)\pi_2f_2-c(2\mid1)\pi_1f_1$. Therefore the [cost-sensitive Bayes classifier](../../../statistical-inference.md#cost-sensitive-bayes-classifier) is

$$
\boxed{\text{choose class one when }
 c(2\mid1)\pi_1f_1(x)>c(1\mid2)\pi_2f_2(x).}
$$

For positive costs and weighted densities, the log posterior-odds score from part (ii) now has threshold $\log(c(1\mid2)/c(2\mid1))$. Larger cost of sending class one to class two expands the region assigned to class one. The weighted-density comparison also handles zero costs without taking an undefined logarithm.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For common [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form) covariance, subtracting the two Gaussian log densities cancels the quadratic term. Equal priors leave the [linear discriminant analysis](../../../statistical-modelling.md#linear-discriminant-analysis) score

$$
\delta(x)=(\mu_1-\mu_2)^T\Sigma^{-1}\left(x-\frac{\mu_1+\mu_2}{2}\right).
$$

Here

$$
\Sigma^{-1}=\begin{pmatrix}1/2&-1\\-1&3\end{pmatrix},\qquad
\Delta=\mu_1-\mu_2=\begin{pmatrix}3\\-1\end{pmatrix},\qquad
\Sigma^{-1}\Delta=\begin{pmatrix}5/2\\-6\end{pmatrix}.
$$

Thus

$$
\boxed{\delta(x)=\tfrac52x_1-6x_2+\tfrac{31}4;\quad
\text{assign class one if }10x_1-24x_2+31>0.}
$$

Assign class two if the expression is negative; a tie has zero probability under either continuous Gaussian law.

To compute the error rather than just specify the boundary, put $D^2=\Delta^T\Sigma^{-1}\Delta=27/2$. Within class one the score has mean $D^2/2=27/4$, and within class two mean $-27/4$. In both classes its [variance](../../../variance.md) is $\Delta^T\Sigma^{-1}\Sigma\Sigma^{-1}\Delta=D^2$. Hence both conditional error probabilities are $\Phi(-D/2)$, where $\Phi$ is the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution) function. Equal priors give the [equal-covariance Gaussian classification error](../../../statistical-inference.md#equal-covariance-gaussian-classification-error)

$$
\boxed{P_{\mathrm{error}}=\Phi\left(-\sqrt{27/8}\right)\approx0.0331.}
$$

For the specified observation, the score is $\delta(2,1)=27/4>0$, so **assign it to class one**.

## 3

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

[Principal component analysis](../../../statistical-learning.md#principal-component-analysis) replaces correlated measurements by uncorrelated linear compounds ordered by decreasing [variance](../../../variance.md). Keeping the leading compounds gives a low-dimensional summary that preserves as much [variance](../../../variance.md) as possible under orthonormal projection. It is an unsupervised description of variation, rather than a guarantee that the high-variance directions are best for classification or prediction.

Write $X_c=X-\mu$. For a unit loading vector $q$, the [variance](../../../variance.md) of $q^TX_c$ is $q^T\Sigma q$. The [spectral theorem](../../../hilbert-space.md#spectral-theorem) gives an orthonormal eigenbasis $q_1,\ldots,q_p$ with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda_1\ge\cdots\ge\lambda_p\ge0$. If $q=\sum_jb_jq_j$ and $\sum_jb_j^2=1$, then

$$
q^T\Sigma q=\sum_j\lambda_jb_j^2\le\lambda_1.
$$

Equality is attained at $q_1$. Requiring the next loading to be orthogonal to the first excludes its eigendirection, so the same argument gives $q_2$ and [variance](../../../variance.md) $\lambda_2$, and continues inductively. Repeated [eigenvalues](../../../linear-operator-theory.md#eigenvalue) permit any [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of the tied eigenspace. These are the [population principal components](../../../statistical-learning.md#population-principal-component).

With $Q=(q_1,\ldots,q_p)$, set $Y=Q^TX_c$. Then

$$
\boxed{\operatorname{Cov}(Y)=\Lambda=Q^T\Sigma Q
=\operatorname{diag}(\lambda_1,\ldots,\lambda_p),\qquad
\Sigma=Q\Lambda Q^T.}
$$

In particular the components are uncorrelated. They need not be independent unless, for example, $X$ is [multivariate normal](../../../probability-and-statistics.md#multivariate-normal-distribution). Finally

$$
\boxed{\sum_{j=1}^p\operatorname{Var}(Y_j)
=\sum_{j=1}^p\lambda_j
=\operatorname{tr}(\Sigma)
=\sum_{j=1}^p\operatorname{Var}(X_j).}
$$

The [trace](../../../linear-algebra.md#matrix-trace) equality follows from $Q^TQ=I$ and cyclicity of [trace](../../../linear-algebra.md#matrix-trace), so the rotation preserves total [variance](../../../variance.md). The [explained variance of a principal component](../../../statistical-learning.md#explained-variance-of-a-principal-component) is its [eigenvalue](../../../linear-operator-theory.md#eigenvalue) divided by this total.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The given [equicorrelation covariance matrix](../../../variance.md#equicorrelation-covariance-matrix) can be written

$$
\Sigma=(1-r)I_4+r\mathbf1\mathbf1^T.
$$

On $\mathbf1=(1,1,1,1)^T$, the rank-one matrix $\mathbf1\mathbf1^T$ acts as multiplication by four. On the three-dimensional orthogonal complement $\{v:\sum_jv_j=0\}$ it acts as zero. Hence the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are **$1+3r$ and $1-r$ with multiplicity three**.

For $0<r<1$, the largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is $1+3r$ and its normalized [eigenvector](../../../linear-operator-theory.md#eigenvector) is $\mathbf1/2$. Therefore the first [population principal component](../../../statistical-learning.md#population-principal-component) is

$$
\boxed{Y_1=\tfrac12\sum_{j=1}^4(X_j-\mu_j),\qquad
\operatorname{Var}(Y_1)=1+3r.}
$$

Omitting the centering merely changes the component by a constant and has no effect on its [variance](../../../variance.md). Since $\operatorname{tr}\Sigma=4$, its explained fraction is

$$
\boxed{\frac{1+3r}{4}.}
$$

It rises from one quarter towards one as the positive common correlation increases. Outside the specified range, a valid covariance requires $-1/3\le r\le1$; for negative $r$ the sum direction is no longer the leading one.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

Covariance-based [PCA](../../../statistical-learning.md#principal-component-analysis) uses centered protein measurements in their original gram units. Its total [variance](../../../variance.md) is $218.4$. Correlation-based [PCA](../../../statistical-learning.md#principal-component-analysis) first divides each centered food measurement by its sample [standard deviation](../../../variance.md#standard-deviation), giving nine unit-variance variables and total [variance](../../../variance.md) nine. Thus it is [principal component analysis on a correlation matrix](../../../statistical-learning.md#principal-component-analysis-on-a-correlation-matrix), not an equivalent rotation of the original unscaled measurements.

The [variances](../../../variance.md) of cereals and milk together account for $170.9/218.4\approx78.3\%$ of the original total. Consequently those variables have considerable influence on covariance-based [PCA](../../../statistical-learning.md#principal-component-analysis). Its first component is dominated by a cereal coefficient $-0.86$ opposed to milk $0.42$, broadly a cereal-versus-milk contrast. Its second is dominated by milk $0.83$, with cereals $0.40$ and fish $-0.29$. Its third is chiefly white meat $0.80$ versus fish $-0.52$, with a smaller negative milk term. Component signs may all be reversed without changing the analysis; the important features are relative signs and magnitudes.

After standardization, eggs and starch can contribute as strongly as large-variance foods. The first correlation-based component gives positive weight to meat, eggs, milk and starch, opposed principally to cereals and pulses/nuts; eggs now has coefficient $0.43$ despite its small raw [variance](../../../variance.md). The second emphasizes fish and fruit/vegetables negatively, opposed especially to starch and white meat. The third contrasts white meat and fruit/vegetables with milk, fish and red meat. Thus standardization changes both the emphasis and the directions, rather than just the displayed units of the same components.

The [explained variance of a principal component](../../../statistical-learning.md#explained-variance-of-a-principal-component) must use the appropriate total:

$$
\begin{array}{c|ccc|c}
\text{analysis}&\text{PC1}&\text{PC2}&\text{PC3}&\text{first three}\\\hline
\text{covariance}&71.1\%&14.1\%&7.1\%&92.3\%\\
\text{correlation}&44.6\%&18.2\%&12.6\%&75.3\%.
\end{array}
$$

Raw and standardized percentages describe different [variance](../../../variance.md) objectives and must not be compared as if one method were always superior.

**Standardize when relative patterns across variables, rather than their absolute gram-scale variation, should have equal marginal weight.** Correlation-based [PCA](../../../statistical-learning.md#principal-component-analysis) is also insensitive to changing a variable's measurement unit, which covariance-based [PCA](../../../statistical-learning.md#principal-component-analysis) is not. Here every food group already has the same units, so differing units do not force standardization. If large fluctuations in actual protein amounts are scientifically important, covariance-based [PCA](../../../statistical-learning.md#principal-component-analysis) is appropriate. If dietary composition across all food groups is the focus, correlation-based [PCA](../../../statistical-learning.md#principal-component-analysis) can be more informative. Standardization can nevertheless amplify noise in nearly constant variables; the decision should follow the scientific purpose and measurement reliability.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

The three retained covariance components explain

$$
\frac{155.2+30.7+15.6}{218.4}=0.9226\ldots,
$$

leaving only $7.7\%$ of the raw total [variance](../../../variance.md). **Three components are a reasonable covariance-based descriptive compression**, if that amount of discarded variation is acceptable for the intended use. Even two explain about $85.1\%$, so three is a useful choice rather than a uniquely forced one.

For the correlation analysis,

$$
\frac{4.01+1.64+1.13}{9}=0.7533\ldots,
$$

so three retain $75.3\%$ and discard $24.7\%$ of standardized variation. **Three can provide an interpretable summary, but the supplied information does not justify treating them as sufficient for every purpose.** Tasks requiring high standardized reconstruction accuracy may need more.

Each of the three displayed correlation [eigenvalues](../../../linear-operator-theory.md#eigenvalue) exceeds the average [eigenvalue](../../../linear-operator-theory.md#eigenvalue) one, but that alone does not show all remaining [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are below one. Their sum is $9-6.78=2.22$, and a fourth [eigenvalue](../../../linear-operator-theory.md#eigenvalue) just above one is compatible with both that sum and the ordering. A complete [eigenvalue](../../../linear-operator-theory.md#eigenvalue) sequence, a plot of successive [eigenvalues](../../../linear-operator-theory.md#eigenvalue), and the stability and interpretation of the directions would help decide the cutoff. With only 25 countries, estimated directions also have sampling uncertainty. The retained covariance and correlation dimensions should therefore be judged against their own [variance](../../../variance.md) criterion and substantive aim, not chosen solely because three columns were printed.

## 4

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For rows $x_i,x_j$, three useful choices are [Euclidean distance](../../../topological-analysis.md#euclidean-distance), [standardized Euclidean distance](../../../topological-analysis.md#standardized-euclidean-distance), and [Mahalanobis distance](../../../variance.md#mahalanobis-distance):

$$
d_E(i,j)=\sqrt{\sum_{r=1}^p(x_{ir}-x_{jr})^2},\qquad
d_S(i,j)=\sqrt{\sum_{r=1}^p\frac{(x_{ir}-x_{jr})^2}{s_r^2}},\qquad
d_M(i,j)=\sqrt{(x_i-x_j)^TS^{-1}(x_i-x_j)}.
$$

The Euclidean choice is simple, rotation invariant and appropriate when the original coordinate scales carry comparable meaning. It is sensitive to scale changes, may be dominated by a high-variance variable and gives correlated or duplicate variables repeated influence. Squared Euclidean dissimilarity is sometimes used algorithmically, but removing the square root generally loses the [triangle inequality](../../../topological-analysis.md#triangle-inequality).

The standardized Euclidean choice removes marginal units using fixed positive sample scales $s_r$. It gives equal marginal weight to variables, but ignores correlations and can magnify noise when an estimated [variance](../../../variance.md) is small. Constant variables require omission or an explicitly chosen positive external scale.

The Mahalanobis choice incorporates the full [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form) sample covariance $S$, so it is [Euclidean distance](../../../topological-analysis.md#euclidean-distance) after whitening. It accounts for both scale and redundancy and is invariant under an invertible change of coordinates when $S$ is transformed consistently. However estimating $S$ requires enough observations and can be sensitive to extreme values; inversion is unstable near singularity and unavailable when $S$ is singular. With fixed positive scales or [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form) $S$, all three square-root expressions are genuine [metrics](../../../topological-analysis.md#metric) on the measurement space. Their different geometries encode different notions of which individuals should be considered similar.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

A [metric](../../../topological-analysis.md#metric) dissimilarity must satisfy, for all $x,y,z$, the four properties

$$
\boxed{d(x,y)\ge0,\qquad d(x,y)=0\ \Longleftrightarrow\ x=y,\qquad
 d(x,y)=d(y,x),\qquad d(x,z)\le d(x,y)+d(y,z).}
$$

They are nonnegativity, identity of indiscernibles, symmetry and the [triangle inequality](../../../topological-analysis.md#triangle-inequality). The following two transformations of the [simple matching coefficient](../../../statistical-learning.md#simple-matching-coefficient) behave differently at the identity.

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

For fixed $p\ge1$, the complement of the [simple matching coefficient](../../../statistical-learning.md#simple-matching-coefficient) is the fraction of coordinates that disagree:

$$
1-S_1(x,y)=\frac1p\sum_{r=1}^p\mathbf1\{x_r\ne y_r\}.
$$

This is the [normalized Hamming distance](../../../coding-theory.md#normalized-hamming-distance). It is nonnegative, symmetric, and is zero exactly when every coordinate agrees. At each coordinate,

$$
\mathbf1\{x_r\ne z_r\}\le
\mathbf1\{x_r\ne y_r\}+\mathbf1\{y_r\ne z_r\}.
$$

Summing and dividing by $p$ proves the [triangle inequality](../../../topological-analysis.md#triangle-inequality). Therefore **$d_1$ is a [metric](../../../topological-analysis.md#metric)** on the binary vectors.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

For every binary vector $x$, $S_1(x,x)=1$, and hence

$$
\boxed{d_2(x,x)=\frac12\ne0.}
$$

Thus **$d_2$ is not a [metric](../../../topological-analysis.md#metric)**, because it fails identity of indiscernibles. It is nonnegative and symmetric. In fact it also satisfies the [triangle inequality](../../../topological-analysis.md#triangle-inequality) trivially: every value lies in $[1/2,1]$, so $d_2(x,z)\le1\le d_2(x,y)+d_2(y,z)$. That does not repair its nonzero self-distance.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

In [agglomerative hierarchical clustering](../../../statistical-learning.md#agglomerative-hierarchical-clustering), start with eight singleton groups. [Single-linkage clustering](../../../statistical-learning.md#single-linkage-clustering) uses the smallest distance between cross-pairs; [complete-linkage clustering](../../../statistical-learning.md#complete-linkage-clustering) uses the largest. Updating these cluster distances after each merge, one valid order of the tied merges gives

$$
\begin{array}{c|cc|cc}
\text{step}&\text{single cluster}&\text{height}&\text{complete cluster}&\text{height}\\\hline
1&BD&0.4&BD&0.4\\
2&AC&0.6&AC&0.6\\
3&EG&0.6&EG&0.6\\
4&ABCD&0.6&FH&1.0\\
5&EGH&0.9&ABCD&1.4\\
6&EFGH&1.0&EFGH&1.5\\
7&ABCDEFGH&1.9&ABCDEFGH&3.8
\end{array}
$$

The merges at height $0.6$ may be reordered; they give the same requested three-cluster cuts. For example, the single-link distance from $AC$ to $BD$ is $\min(1.2,1.4,0.6,0.8)=0.6$, while its complete-link distance is their maximum $1.4$. After forming $EG$, its single-link distance to $H$ is $\min(0.9,1.2)=0.9$. The complete-link distance between $EG$ and $FH$ is $\max(1.2,0.9,1.5,1.2)=1.5$. Finally the closest cross-pair between $ABCD$ and $EFGH$ is $CG$ at $1.9$, while the farthest is $BF$ at $3.8$.

At three groups the partitions are therefore

$$
\boxed{\text{single linkage: }\{A,B,C,D\},\ \{E,G,H\},\ \{F\};}
$$



$$
\boxed{\text{complete linkage: }\{A,B,C,D\},\ \{E,G\},\ \{F,H\}.}
$$

**Two groups, $\{A,B,C,D\}$ and $\{E,F,G,H\}$, are more strongly supported by the merge heights.** For single linkage the three-to-two merge is at $1.0$, close to the preceding height $0.9$, whereas the two-to-one merge is delayed until $1.9$. For complete linkage the three-to-two merge at $1.5$ is close to $1.4$, whereas the final merge jumps to $3.8$. Both methods agree on the two-group partition but split its second group differently when forced to return three groups. A three-group choice is possible if required substantively, but is not particularly compelling from these dissimilarities alone.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
