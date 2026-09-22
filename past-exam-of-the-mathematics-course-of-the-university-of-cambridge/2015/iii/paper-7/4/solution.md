<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Identify $G$ with the [Boolean hypercube](../../../../../boolean-hypercube.md) $\{-1,1\}^d$, with coordinatewise multiplication and normalized [Haar measure](../../../../../haar-measure.md) assigning mass $2^{-d}$ to each point. Its [Bernoulli function](../../../../../bernoulli-function-hypercube.md) $\epsilon_i(\omega)=\omega_i$ is a [Rademacher random variable](../../../../../rademacher-distribution.md). The [Walsh functions on a hypercube](../../../../../walsh-character.md) are the [Walsh characters](../../../../../walsh-character.md) $w_A=\prod_{i\in A}\epsilon_i$, indexed by all subsets $A\subseteq\{1,\ldots,d\}$, including $w_\varnothing=1$. Independence of the sign coordinates gives $\langle w_A,w_B\rangle=\mathbb E w_{A\triangle B}=\mathbf1_{A=B}$. There are $2^d$ characters, equal to the dimension of $L^2(G)$, so they form an [orthonormal basis](../../../../../orthonormal-basis.md).

Flipping coordinate $i$ negates $w_A$ exactly when $i\in A$. Thus the [coordinate-flip generator on a hypercube](../../../../../coordinate-flip-generator-on-a-hypercube.md) satisfies

$$
\boxed{Lw_A=-|A|w_A,\qquad\sigma(L)=\{0,-1,\ldots,-d\},\qquad\text{multiplicity of }-j=\binom dj.}
$$

For $f=\sum_A\widehat f(A)w_A$, [Parseval identity](../../../../../parseval-identity.md) gives $\langle f,Lf\rangle=-\sum_A|A||\widehat f(A)|^2\leq0$. Equivalently its [Dirichlet form of a Markov chain](../../../../../dirichlet-form-of-a-markov-chain.md) is

$$
\mathcal E(f)=-\mathbb E[fLf]=\frac14\sum_{i=1}^d\mathbb E\bigl(f(\omega^{(i)})-f(\omega)\bigr)^2,
$$

where $\omega^{(i)}$ flips coordinate $i$.

Set $S(\omega)=\sum_i a_i\epsilon_i(\omega)$ and $F(\omega)=\|S(\omega)\|$. Since $F(-\omega)=F(\omega)$, its Walsh expansion contains only sets $A$ of even size. Every nonconstant such set has $|A|\geq2$, giving the [even-function spectral gap on a hypercube](../../../../../even-function-spectral-gap-on-a-hypercube.md)

$$
2\operatorname{Var}(F)\leq\mathcal E(F).
$$

At each $S(\omega)$ the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) supplies a real supporting linear functional $\ell$ of [norm](../../../../../norm.md) at most one with $\ell(S)=\|S\|$; for a complex normed space use the real part of a complex norming functional. At $S=0$ take $\ell=0$. Convexity of the [norm](../../../../../norm.md) gives $F(\omega^{(i)})-F(\omega)\geq\ell(S(\omega^{(i)})-S(\omega))$. Since $LS=-S$, sum these inequalities to get $LF\geq-F$. Therefore $\mathcal E(F)=-\mathbb E[FLF]\leq\mathbb EF^2$. Combining the two bounds yields the [sharp Rademacher second-moment inequality](../../../../../sharp-rademacher-second-moment-inequality.md)

$$
\boxed{\mathbb E\left\|\sum_i a_i\epsilon_i\right\|^2\leq2\left(\mathbb E\left\|\sum_i a_i\epsilon_i\right\|\right)^2.}
$$

No smoothness of the [norm](../../../../../norm.md) is required. The constant $2$ is sharp: two equal nonzero real coefficients give modulus $0$ or $2|a|$ with equal probabilities. This is the second-versus-first moment case of the [Kahane-Khintchine inequality](../../../../../kahane-khintchine-inequality.md) for arbitrary [normed vector spaces](../../../../../normed-vector-space.md).

For the complex-circle assertion, write each independent [Steinhaus random variable](../../../../../steinhaus-random-variable.md) as $\eta_i=\epsilon_i\cos\theta_i+i\delta_i\sin\theta_i$, where $\theta_i$ is uniform on $[0,\pi/2]$ and all quadrant signs $\epsilon_i,\delta_i$ are independent. Conditional on the angles, $\sum_i a_i\eta_i$ is a [Rademacher sum](../../../../../rademacher-sum.md) with $2d$ complex coefficients $a_i\cos\theta_i$ and $ia_i\sin\theta_i$. Its conditional second moment is $\sum_i|a_i|^2$, independent of the angles. The preceding inequality gives its conditional first moment at least $\sqrt{\frac12\sum_i|a_i|^2}$. Average over the angles and square to obtain the [Steinhaus first-moment lower bound](../../../../../steinhaus-first-moment-lower-bound.md)

$$
\boxed{\sum_i|a_i|^2\leq2\left(\mathbb E\left|\sum_i a_i\eta_i\right|\right)^2.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
