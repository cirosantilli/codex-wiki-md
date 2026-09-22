<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $d\gamma_1(x)=(2\pi)^{-1/2}e^{-x^2/2}\,dx$. On the dense [polynomial](../../../../../polynomial-split.md) algebra in $L^2(\gamma_1)$, the [Gaussian creation and annihilation operators](../../../../../gaussian-creation-and-annihilation-operators.md) are

$$
\boxed{a^-f=f',\qquad a^+f=xf-f'.}
$$

[Gaussian integration by parts](../../../../../stein-s-lemma-probability.md) gives $\langle a^-f,g\rangle=\langle f,a^+g\rangle$. Their closed realizations are adjoints. More explicitly, for the [orthonormal basis](../../../../../orthonormal-basis.md) $h_n=\operatorname{He}_n/\sqrt{n!}$ of normalized [Probabilists' Hermite polynomials](../../../../../probabilists-hermite-polynomial.md),

$$
a^-h_n=\sqrt n\,h_{n-1},\qquad a^+h_n=\sqrt{n+1}\,h_{n+1}.
$$

Thus the closed annihilation operator has domain $\{\sum c_nh_n:\sum n|c_n|^2<\infty\}$, and the closed creation operator has domain $\{\sum c_nh_n:\sum(n+1)|c_n|^2<\infty\}$. These describe the same set of $L^2$ functions, the [Gaussian Sobolev space](../../../../../gaussian-sobolev-space.md), though the two operators differ. Directly on [polynomials](../../../../../polynomial-split.md), $[a^-,a^+]=I$, and

$$
\boxed{Lf=-a^+a^-f=f''-xf'.}
$$

Use the standard [carré du champ operator](../../../../../carre-du-champ-operator.md) convention $\Gamma(f,g)=\tfrac12(L(fg)-fLg-gLf)$. The product rule for this [semigroup generator](../../../../../infinitesimal-generator-of-a-semigroup.md) gives

$$
L(fg)-fLg-gLf=2f'g',
$$

so the requested squared-gradient and [joint energy](../../../../../joint-energy-of-a-symmetric-markov-semigroup.md) formulas, for real functions in the standard algebra, are

$$
\boxed{\Gamma(f,g)=f'g',\qquad
\mathcal E_{\gamma_1}(f,g)=-\int fLg\,d\gamma_1=\int f'g'\,d\gamma_1.}
$$

For complex functions the [joint energy](../../../../../joint-energy-of-a-symmetric-markov-semigroup.md) is sesquilinear, with $\overline{g'}$ in the second factor. If “squared gradient” is defined without the factor $1/2$ in the product-rule expression, its value is instead $2f'g'$ and the [joint energy](../../../../../joint-energy-of-a-symmetric-markov-semigroup.md) is one half of its integral; the [joint energy](../../../../../joint-energy-of-a-symmetric-markov-semigroup.md) and logarithmic Sobolev constant used here remain as displayed.

For the [Gaussian logarithmic Sobolev inequality](../../../../../gaussian-logarithmic-sobolev-inequality.md), first take smooth bounded $f$ with bounded first and second [derivatives](../../../../../derivative.md), bounded away from zero. The [Mehler formula for the Ornstein-Uhlenbeck semigroup](../../../../../mehler-formula-for-the-ornstein-uhlenbeck-semigroup.md) is

$$
P_tf(x)=\int_{\mathbb R}f\left(e^{-t}x+\sqrt{1-e^{-2t}}\,y\right)\,d\gamma_1(y).
$$

It preserves $\gamma_1$ and differentiating in $x$ gives the [Ornstein-Uhlenbeck gradient commutation identity](../../../../../ornstein-uhlenbeck-gradient-commutation-identity.md)

$$
(P_tf)'=e^{-t}P_t(f').
$$

Put $u_t=P_tf$. Differentiate its [entropy functional](../../../../../entropy-functional.md). Since $\int u_t\,d\gamma_1=\int f\,d\gamma_1$ is constant, and [Gaussian integration by parts](../../../../../stein-s-lemma-probability.md) applies,

$$
\frac d{dt}\operatorname{Ent}_{\gamma_1}(u_t)
=\int (1+\log u_t)Lu_t\,d\gamma_1
=-\int\frac{|u_t'|^2}{u_t}\,d\gamma_1.
$$

For such data, Mehler's formula and dominated convergence give $P_tf(x)\to\int f\,d\gamma_1$ as $t\to\infty$. The uniform positive upper and lower bounds justify integrating this limit inside the entropy, whose limit is zero. Hence

$$
\operatorname{Ent}_{\gamma_1}(f)
=\int_0^\infty\int\frac{|(P_tf)'|^2}{P_tf}\,d\gamma_1\,dt.
$$

Apply the allowed weighted [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) with $g=f'$:

$$
\frac{|(P_tf)'|^2}{P_tf}
=e^{-2t}\frac{(P_tf')^2}{P_tf}
\leq e^{-2t}P_t\left(\frac{|f'|^2}{f}\right).
$$

After integration, invariance of $\gamma_1$ gives

$$
\int\frac{|(P_tf)'|^2}{P_tf}\,d\gamma_1
\leq e^{-2t}\int\frac{|f'|^2}{f}\,d\gamma_1.
$$

Integrating in $t$ yields

$$
\operatorname{Ent}_{\gamma_1}(f)\leq\frac12\int\frac{|f'|^2}{f}\,d\gamma_1.
$$

For a real smooth compactly supported $g$, take $f=g^2+\epsilon$. Then

$$
\frac{|f'|^2}{f}
=\frac{4g^2|g'|^2}{g^2+\epsilon}\leq4|g'|^2.
$$

Letting $\epsilon\downarrow0$ proves

$$
\boxed{\operatorname{Ent}_{\gamma_1}(g^2)\leq
2\int|g'|^2\,d\gamma_1=2\mathcal E_{\gamma_1}(g).}
$$

Smooth approximation and cutoff in the Gaussian Sobolev [norm](../../../../../norm.md) extend this to the full form domain. The entropy is lower semicontinuous under the resulting $L^2$ convergence: the square densities converge in $L^1$, their masses converge, and, along an almost-everywhere convergent subsequence, Fatou's lemma applies to $h\log h$ after adding the bound $1/e$. The same inequality for complex $g$ follows by applying it to $|g|$ and using the weak-derivative bound $|(|g|)'|\leq|g'|$. Thus the constant is at most $2$.

For [sharpness of the Gaussian logarithmic Sobolev constant](../../../../../sharpness-of-the-gaussian-logarithmic-sobolev-constant.md), take $g_s(x)=e^{sx/2}$ with real $s\ne0$. These functions belong to the [Gaussian Sobolev space](../../../../../gaussian-sobolev-space.md). The [Gaussian moment-generating function](../../../../../moment-generating-function-of-a-normal-distribution.md) gives

$$
\int g_s^2\,d\gamma_1=e^{s^2/2},\qquad
\int x e^{sx}\,d\gamma_1=s e^{s^2/2}.
$$

Therefore

$$
\operatorname{Ent}_{\gamma_1}(g_s^2)
=s^2e^{s^2/2}-e^{s^2/2}\frac{s^2}{2}
=\frac{s^2}{2}e^{s^2/2},
\qquad
\mathcal E_{\gamma_1}(g_s)=\frac{s^2}{4}e^{s^2/2}.
$$

The entropy-to-energy ratio is exactly $2$, so no smaller constant can work. Combining this lower bound with the proved inequality gives

$$
\boxed{c_{\mathrm{LS}}(\gamma_1)=2.}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
