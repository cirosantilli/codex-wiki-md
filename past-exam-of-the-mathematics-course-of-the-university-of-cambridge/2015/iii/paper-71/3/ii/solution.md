<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Leibniz rule](../../../../../../leibniz-rule.md) expands each [derivative](../../../../../../derivative.md) of a product into finitely many terms:

$$
\partial_x^\alpha\partial_\theta^\beta(a_1a_2)=\sum_{\mu\leq\alpha,\nu\leq\beta}\binom\alpha\mu\binom\beta\nu(\partial_x^\mu\partial_\theta^\nu a_1)(\partial_x^{\alpha-\mu}\partial_\theta^{\beta-\nu}a_2).
$$

The [symbol class](../../../../../../symbol-class.md) estimates bound every summand by a constant times $\langle\theta\rangle^{N_1-|\nu|+N_2-|\beta-\nu|}=\langle\theta\rangle^{N_1+N_2-|\beta|}$. Hence **symbol orders add under multiplication**:

$$
\boxed{a_1a_2\in\operatorname{Sym}(X;\mathbb R^k;N_1+N_2).}
$$

We now address the remaining unheaded requests. To define the [oscillatory integral](../../../../../../oscillatory-integral.md) as a functional on the [space of test functions](../../../../../../space-of-test-functions.md), choose $\eta\in C_c^\infty(\mathbb R^k)$ equal to one near zero and set

$$
\langle I_\Phi(a),f\rangle=\lim_{R\to\infty}\iint e^{i\Phi(x,\theta)}a(x,\theta)f(x)\eta(\theta/R)\,d\theta\,dx.
$$

The limit is not an assertion of absolute convergence of the original frequency integral. Split off a bounded-frequency part, which is smooth in $x$. At large frequency define

$$
q=|\nabla_x\Phi|^2+|\theta|^2|\nabla_\theta\Phi|^2,\qquad
L=\frac1{iq}\left(\nabla_x\Phi\cdot\nabla_x+|\theta|^2\nabla_\theta\Phi\cdot\nabla_\theta\right).
$$

Homogeneity and nonvanishing of the total phase differential imply $q\geq c_K|\theta|^2$ on each compact spatial set. Also $Le^{i\Phi}=e^{i\Phi}$. The spatial coefficients of $L$ have symbol order $-1$, and its frequency coefficients have order zero; consequently its [formal transpose of a differential operator](../../../../../../formal-transpose-of-a-differential-operator.md) $L^t$ lowers symbol order by one. After $r>N+k$ integrations by parts, the high-frequency pairing has an absolutely integrable amplitude $(L^t)^r[(1-\chi(\theta))a(x,\theta)f(x)]$, where $\chi$ is a fixed cutoff near zero. [Derivatives](../../../../../../derivative.md) of the outer cutoff yield errors bounded by $CR^{N+k-r}$ times finitely many [derivatives](../../../../../../derivative.md) of $f$, so they tend to zero. This proves [cutoff independence of an oscillatory integral](../../../../../../cutoff-independence-of-an-oscillatory-integral.md) and defines a linear map into $\mathbb C$. Its distributional continuity is permitted as an assumption, and is also visible from this finite-[derivative](../../../../../../derivative.md) estimate.

The [singular support](../../../../../../singular-support.md) of a [distribution](../../../../../../distribution-mathematical-analysis.md) is the complement of the largest open subset on which it equals a smooth [regular distribution](../../../../../../regular-distribution.md). The [stationary-direction bound for singular support](../../../../../../stationary-direction-bound-for-singular-support.md) needs [conic support of an oscillatory amplitude](../../../../../../conic-support-of-an-oscillatory-amplitude.md). Write

$$
C_a=\overline{\{(x,\theta/|\theta|):(x,\theta)\in\operatorname{supp}a,\ \theta\ne0\}}\subset X\times S^{k-1}.
$$

Its radial lift is the closed conic enlargement of the ordinary support. **The generally valid bound is**

$$
\boxed{\operatorname{sing\,supp}I_\Phi(a)\subset\{x:\exists\omega\in S^{k-1},\ (x,\omega)\in C_a,\ \nabla_\theta\Phi(x,\omega)=0\}.}
$$

If the amplitude support is conic, this is exactly the printed bound. It is also the standard interpretation when support in the frequency directions is understood conically.

To prove the bound, take a point outside its right-hand side. Closedness of $C_a$ and compactness of the sphere give a neighborhood $U$ and $c>0$ with $|\nabla_\theta\Phi|\geq c$ on the amplitude's directions over $U$. On a slightly larger directional neighborhood use

$$
L_\theta=\frac{\nabla_\theta\Phi\cdot\nabla_\theta}{i|\nabla_\theta\Phi|^2},\qquad L_\theta e^{i\Phi}=e^{i\Phi}.
$$

The [formal transpose of a differential operator](../../../../../../formal-transpose-of-a-differential-operator.md) $L_\theta^t$ lowers symbol order by one, using frequency [derivatives](../../../../../../derivative.md) only. An $x$ [derivative](../../../../../../derivative.md) of order $l$ of the oscillatory integrand has symbol order at most $N+l$. Choosing more than $N+l+k$ integrations by parts makes that [derivative](../../../../../../derivative.md) absolutely integrable, uniformly on smaller compact subsets of $U$. This works for every $l$, so $I_\Phi(a)$ is smooth on $U$.

The [ordinary amplitude support can miss a singular-support limit](../../../../../../ordinary-amplitude-support-can-miss-a-singular-support-limit.md) phenomenon requires a qualification here: **with unrestricted ordinary support the printed inclusion is false.** An explicit counterexample uses $X=\mathbb R^2$, $x=(s,t)$, one frequency variable and $\Phi(s,t,\theta)=s\theta$. Choose $t_j=1/j$, $w_j=1/(10j^2)$ and $\chi\in C_c^\infty((-1/4,1/4))$ with $\chi(0)=1$. Its translates $\chi_j(t)=\chi((t-t_j)/w_j)$ have disjoint supports. Choose an even [smooth function](../../../../../../smooth-function.md) $\rho$ that is zero for $|\theta|\leq1$ and one for $|\theta|\geq2$, and put

$$
a(s,t,\theta)=\sum_{j\geq1}e^{-j^2}\chi_j(t)\rho(\theta/2^j).
$$

This is a symbol of order zero. All spatial [derivative](../../../../../../derivative.md) bounds follow from $\sum_j e^{-j^2}w_j^{-l}<\infty$; frequency [derivatives](../../../../../../derivative.md) have the required decay because the $j$th cutoff [derivative](../../../../../../derivative.md) is supported where $|\theta|\asymp2^j$. Near every point $(s,0,\theta)$ with finite $\theta$, all large-$j$ terms vanish through the frequency cutoff and all remaining terms vanish in a small $t$ neighborhood. Thus no point $(0,0,\theta)$ lies in its ordinary support.

Nevertheless its oscillatory integral is

$$
I_\Phi(a)=2\pi B(t)\delta_0(s)-G(s,t),\qquad B(t)=\sum_j e^{-j^2}\chi_j(t),
$$

where $G$ is smooth. Indeed, its $j$th term is the ordinary Fourier integral of $1-\rho(\theta/2^j)$ times $e^{-j^2}\chi_j(t)$; [derivatives](../../../../../../derivative.md) of order $l$ in $s$ and $m$ in $t$ are bounded by a constant times $e^{-j^2}2^{j(l+1)}w_j^{-m}$, a summable sequence. Since $B(t_j)\ne0$, each $(0,t_j)$ is singular. Closedness of [singular support](../../../../../../singular-support.md) forces $(0,0)$ to be singular too, although the literal ordinary-support right-hand side omits it. The closed conic support includes this limiting point and resolves the defect.

Finally use [Fourier inversion](../../../../../../fourier-inversion-theorem.md) distributionally. The constant amplitude gives $(2\pi)^{-n}\int e^{ix\cdot\theta}d\theta=\delta_0$, and differentiation of the exponential supplies a factor $i\theta$. Thus **the polynomial-amplitude integral is a delta [derivative](../../../../../../derivative.md)**:

$$
\boxed{\frac1{(2\pi)^n}\int\theta^\alpha e^{ix\cdot\theta}\,d\theta=i^{-|\alpha|}\partial^\alpha\delta_0=D^\alpha\delta_0.}
$$

Its action on a [test function](../../../../../../test-function.md) $f$ is $i^{|\alpha|}\partial^\alpha f(0)$, confirming both the sign and the normalization. This is the [delta derivatives from polynomial oscillatory amplitudes](../../../../../../delta-derivatives-from-polynomial-oscillatory-amplitudes.md) identity.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
