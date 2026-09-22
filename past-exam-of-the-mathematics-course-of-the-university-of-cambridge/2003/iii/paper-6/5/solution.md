<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [C-star algebra](../../../../../c-star-algebra.md) is a complex [Banach algebra](../../../../../banach-algebra-split.md) with an antilinear [algebra involution](../../../../../algebra-involution.md) satisfying $(ab)^*=b^*a^*$, $(a^*)^*=a$ and the [C-star identity](../../../../../c-star-identity.md) $\|a^*a\|=\|a\|^2$. First take a nonzero unital algebra. Its identity has [norm](../../../../../norm.md) one, since $\|1\|^2=\|1\|$. Also

$$
\|a^*\|^2=\|aa^*\|\leq\|a\|\|a^*\|,
$$

and exchanging $a,a^*$ proves $\|a^*\|=\|a\|$. Thus the [algebra involution](../../../../../algebra-involution.md) is continuous. An element $h=h^*$ is a [Hermitian C-star element](../../../../../hermitian-element-of-a-c-star-algebra.md), and an element satisfying $xx^*=x^*x$ is a [normal C-star element](../../../../../normal-element-of-a-c-star-algebra.md).

We establish the spectral facts needed for the representation, to avoid assuming the conclusion. For a [Hermitian C-star element](../../../../../hermitian-element-of-a-c-star-algebra.md) $h$, the [Banach algebra exponential](../../../../../banach-algebra-exponential.md) $u_t=e^{ith}$ is unitary: taking adjoints of its absolutely convergent series gives $u_t^*=e^{-ith}$, and multiplication gives $u_tu_t^*=1$. Hence $\|u_t\|=1$. If $\lambda\in\sigma(h)$, then $e^{it\lambda}\in\sigma(u_t)$. Indeed, the entire factorization

$$
e^{itz}-e^{it\lambda}=(z-\lambda)g_t(z)
$$

can be evaluated by its convergent power series at $h$. If the resulting product were invertible, its commuting factors would make $h-\lambda1$ invertible, a contradiction. The spectral bound therefore gives $|e^{it\lambda}|\leq1$ for every real $t$. Both signs of $t$ force $\operatorname{Im}\lambda=0$. Thus **Hermitian elements have real spectrum**.

For [completeness](../../../../../completeness.md), the [spectral radius formula](../../../../../spectral-radius-formula.md) needed below follows from the same resolvent theory. [Submultiplicativity](../../../../../submultiplicativity.md) gives

$$
\gamma=\lim_{n\to\infty}\|a^n\|^{1/n}=\inf_{n\geq1}\|a^n\|^{1/n}.
$$

For the existence of the limit, write $n=qj+r$ with $0\leq r<j$ and bound $\|a^n\|\leq\|a^j\|^q\|a^r\|$; this bounds the upper limit by every $j$th root, while the infimum bounds the lower limit. If a power vanishes, the conclusion follows directly. For $|\lambda|>\gamma$, the resolvent series converges by the root test, so $r(a)\leq\gamma$. Conversely, for any $R>r(a)$, contour integration of the resolvent gives

$$
a^n=\frac1{2\pi i}\int_{|\lambda|=R}\lambda^n(\lambda1-a)^{-1}\,d\lambda.
$$

At a larger circle this follows by termwise integration of the [Neumann series](../../../../../neumann-series.md); deformation to radius $R$ is justified by [norm](../../../../../norm.md) analyticity and scalar Cauchy theory as in Question 4. Therefore $\|a^n\|\leq R^{n+1}\sup_{|\lambda|=R}\|R_a(\lambda)\|$, so $\gamma\leq R$. Letting $R\downarrow r(a)$ proves $r(a)=\gamma$.

For a [normal C-star element](../../../../../normal-element-of-a-c-star-algebra.md) $a$, its adjoint commutes with it. The [C-star identity](../../../../../c-star-identity.md) gives

$$
\|a^2\|^2=\|(a^*)^2a^2\|=\|(a^*a)^2\|=\|a^*a\|^2=\|a\|^4,
$$

where the middle [norm](../../../../../norm.md) equality uses the identity for the Hermitian element $a^*a$. Every power is again normal, so $\|a^{2^j}\|=\|a\|^{2^j}$. The spectral-radius formula yields

$$
\boxed{r(a)=\|a\|\quad\text{for every normal }a}.
$$

This derives the [spectral radius norm equality for normal elements](../../../../../spectral-radius-norm-equality-for-normal-elements.md) from the axioms.

Now let $A$ be commutative and unital. Its [character space of an algebra](../../../../../character-space-of-an-algebra.md) $\Delta(A)$ is compact Hausdorff in the [weak-star topology](../../../../../weak-star-topology.md). Every [algebra character](../../../../../character-of-an-algebra.md) has [norm](../../../../../norm.md) at most one by the argument in Question 4, and this space is the weak-star closed subset of the dual [unit ball](../../../../../unit-ball.md) defined by $\phi(1)=1$ and $\phi(ab)=\phi(a)\phi(b)$. [Compactness](../../../../../compact-space.md) follows from the [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md); weak-star separation makes it Hausdorff.

We also need the full character-spectrum correspondence, not just one inclusion. Every proper ideal is contained in a maximal ideal. Such a maximal ideal $M$ is closed: if its closure contained one, it would contain an element within [norm](../../../../../norm.md) distance less than one of the identity, which is invertible by the [Neumann series](../../../../../neumann-series.md), contradicting properness. Its closure is therefore proper and maximality gives equality. The quotient $A/M$ is a complex Banach division algebra. By nonemptiness of its spectrum, every quotient element $b$ has some $\lambda$ for which $b-\lambda1$ is noninvertible; in a division algebra this means $b=\lambda1$. Thus the quotient is the scalars, proving the needed [Gelfand-Mazur theorem](../../../../../gelfand-mazur-theorem.md) conclusion directly and producing a [algebra character](../../../../../character-of-an-algebra.md) with kernel $M$.

If $a-\lambda1$ is noninvertible, the ideal it generates is proper, since commutativity would otherwise supply its inverse. A containing maximal ideal therefore supplies a [algebra character](../../../../../character-of-an-algebra.md) with $\phi(a)=\lambda$. The converse inclusion was already proved. Hence

$$
\sigma_A(a)=\{\phi(a):\phi\in\Delta(A)\}.
$$

The [Gelfand transform](../../../../../gelfand-representation.md) $a\mapsto\widehat a$, $\widehat a(\phi)=\phi(a)$, is a unital [algebra homomorphism](../../../../../algebra-homomorphism-over-a-field.md) into $C(\Delta(A))$. If $h=h^*$, the reality of its spectrum makes $\phi(h)$ real. Writing $a=h+ik$ with [Hermitian C-star elements](../../../../../hermitian-element-of-a-c-star-algebra.md) $h,k$ gives $\phi(a^*)=\overline{\phi(a)}$. Thus the transform respects the [algebra involution](../../../../../algebra-involution.md). Every element of a commutative [C-star algebra](../../../../../c-star-algebra.md) is normal, and therefore

$$
\|\widehat a\|_\infty=\max_{\lambda\in\sigma(a)}|\lambda|=r(a)=\|a\|.
$$

It is a [linear isometry](../../../../../linear-isometry-of-hilbert-spaces.md), hence injective and with closed image because $A$ is complete. The image contains constants, separates [algebra characters](../../../../../character-of-an-algebra.md) by their definition, and is closed under [complex conjugation](../../../../../complex-conjugation.md). The complex [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) makes that image dense in $C(\Delta(A))$, and closedness makes it all of that space. We have proved the [Commutative Gelfand--Naimark theorem](../../../../../commutative-gelfand-naimark-theorem.md):

$$
\boxed{A\cong C(\Delta(A))\text{ isometrically as unital star algebras}}.
$$

These steps show exactly how [completeness](../../../../../completeness.md), the [algebra involution](../../../../../algebra-involution.md) and the C-star [norm](../../../../../norm.md) identity enter the theorem. A general [Banach algebra](../../../../../banach-algebra-split.md) need not have an injective or norm-preserving [Gelfand transform](../../../../../gelfand-representation.md).

The general commutative theorem also has a nonunital form. Here is an elementary construction of the necessary [C-star unitization](../../../../../unitization-of-a-c-star-algebra.md), without assuming the representation theorem. Left multiplication $L_a$ on $A$ is isometric in [operator norm](../../../../../operator-norm.md): the upper bound is [submultiplicativity](../../../../../submultiplicativity.md), and testing on $a^*/\|a\|$ proves the reverse bound for nonzero $a$. If $A$ is nonunital, adjoin the identity operator to the closed algebra $L(A)$ inside the bounded operators on the [Banach space](../../../../../banach-space-split.md) $A$. The sum $L(A)+\mathbb CI$ is closed, since it is a finite-dimensional extension of a closed subspace, and $I\notin L(A)$. A left identity in a [C-star algebra](../../../../../c-star-algebra.md) would, by taking adjoints, give a right identity; the two coincide, so $I\in L(A)$ would contradict nonunitality.

For the formal element $z=a+\lambda1$, define its [algebra involution](../../../../../algebra-involution.md) by $z^*=a^*+\overline\lambda1$ and [norm](../../../../../norm.md) by $\|L_z\|$. For every $b\in A$,

$$
\|zb\|^2=\|b^*z^*zb\|\leq\|b\|\|L_{z^*z}b\|.
$$

Taking suprema over the [unit ball](../../../../../unit-ball.md) and using [submultiplicativity](../../../../../submultiplicativity.md) gives $\|L_z\|^2\leq\|L_{z^*z}\|\leq\|L_{z^*}\|\|L_z\|$. Apply the same inequalities to $z^*$ to obtain $\|L_z\|=\|L_{z^*}\|$ and then the [C-star identity](../../../../../c-star-identity.md). This is the [C-star unitization by left multiplication](../../../../../c-star-unitization-by-left-multiplication.md). The original algebra is a closed ideal in it.

For commutative nonunital $A$, apply the proved unital theorem to $\widetilde A$. The scalar quotient [algebra character](../../../../../character-of-an-algebra.md) $\varepsilon(a+\lambda1)=\lambda$ identifies $A=\ker\varepsilon$ with the continuous functions on $\Delta(\widetilde A)$ that vanish at $\varepsilon$. Removing this one [algebra character](../../../../../character-of-an-algebra.md) gives a locally [compact Hausdorff space](../../../../../compact-hausdorff-space.md); those functions are exactly its continuous functions vanishing at infinity. Restriction and extension of nonzero [algebra characters](../../../../../character-of-an-algebra.md) identify this space with $\Delta(A)$: a [algebra character](../../../../../character-of-an-algebra.md) extends uniquely by $\widetilde\phi(a+\lambda1)=\phi(a)+\lambda$, and every [algebra character](../../../../../character-of-an-algebra.md) other than $\varepsilon$ restricts nontrivially. Thus the full nonunital conclusion is $A\cong C_0(\Delta(A))$.

Return to a [normal C-star element](../../../../../normal-element-of-a-c-star-algebra.md) $x$ in a unital [C-star algebra](../../../../../c-star-algebra.md), possibly noncommutative. Let $B=C^*(1,x)$, the closed unital star algebra generated by $x$ and $x^*$. It is commutative because the two generators commute. We first prove the [spectral permanence for C-star algebras](../../../../../spectral-permanence-for-c-star-algebras.md) needed to use the ambient spectrum rather than a potentially larger subalgebra spectrum.

If $h=h^*\in B$, both its ambient and subalgebra spectra are real. The complement of the compact real set $\sigma_A(h)$ is connected. Within this complement, the set of $\lambda$ for which $(\lambda1-h)^{-1}\in B$ is nonempty by the large-parameter [Neumann series](../../../../../neumann-series.md); it is open by a local inverse series in $B$ and closed by continuous inversion in $A$ and closedness of $B$. It is therefore the entire complement, proving $\sigma_B(h)=\sigma_A(h)$. If a general $b\in B$ is invertible in $A$, then $b^*b$ and $bb^*$ are invertible Hermitian elements, whose inverses lie in $B$. The elements $(b^*b)^{-1}b^*$ and $b^*(bb^*)^{-1}$ give a left and a right inverse for $b$ inside $B$, and these inverses coincide. Applying this to every $b-\lambda1$ proves $\sigma_B(b)=\sigma_A(b)$ for all $b\in B$.

By the proved commutative theorem, $B\cong C(\Delta(B))$. The map

$$
\Delta(B)\longrightarrow\sigma_A(x),\qquad \phi\longmapsto\phi(x)
$$

is onto by the character-spectrum correspondence and spectral permanence. It is injective because [algebra characters](../../../../../character-of-an-algebra.md) respect adjoints and are determined by their values on the [star polynomials in one normal element](../../../../../star-polynomial-in-one-normal-element.md), which are dense in $B$. It is a continuous bijection from a [compact space](../../../../../compact-space.md) to a [Hausdorff space](../../../../../hausdorff-space.md), hence a homeomorphism. Consequently the inverse [Gelfand transform](../../../../../gelfand-representation.md), under this identification, supplies

$$
\boxed{\theta_x:C(\sigma_A(x))\longrightarrow A,\qquad \theta_x(Z)=x,\qquad \|\theta_x(f)\|=\|f\|_\infty}.
$$

It is a continuous unital star homomorphism and a [linear isometry](../../../../../linear-isometry-of-hilbert-spaces.md). Its image is exactly $B$. If another such map sends $Z$ to $x$, it sends $\overline Z$ to $x^*$ and agrees on every polynomial in $Z,\overline Z$. These functions contain constants, separate points of the compact spectrum and are closed under conjugation; Stone-Weierstrass gives their uniform density. Continuity proves uniqueness on all of $C(\sigma_A(x))$. This is the requested [continuous functional calculus](../../../../../continuous-functional-calculus.md), including its isometry and image assertion.

Two conventions in the printed statement need to be made explicit. A unital map into $A$ requires $A$ to have an identity. If nonunital [C-star algebras](../../../../../c-star-algebra.md) are allowed, for example $A=C_0(\mathbb R)$, the asserted unital map into $A$ does not exist in general; the unital construction instead has target $\widetilde A$. Also the image above is the closed unital star algebra $C^*(1,x)$, not necessarily the smallest nonunital algebra generated by $x,x^*$. For $x=0$ in $A=\mathbb C$, the former is $\mathbb C1$ and the latter is $\{0\}$. Thus the intended assertion is correct if “generated” includes the identity; without that convention, this is a counterexample. The distinction is the [unital versus nonunital generation by a normal element](../../../../../unital-versus-nonunital-generation-by-a-normal-element.md).

For a nonunital $A$, take $\sigma(x)$ in $\widetilde A$ and construct the unital calculus there. The scalar quotient [algebra character](../../../../../character-of-an-algebra.md) sends $x$ to zero, so it sends $f(x)$ to $f(0)$. Functions with $f(0)=0$ therefore give elements of $A$. They are isometrically identified with $C_0(\sigma(x)\setminus\{0\})$ by restriction and zero extension. Approximating them by star polynomials and subtracting the constant value at zero proves that their image is exactly $C^*(x)$, with no identity adjoined. This proves the [nonunital continuous functional calculus](../../../../../nonunital-continuous-functional-calculus.md) as well as specifying the corrected form of the original claim.

We finish with the positive-square-root theorem, giving a proof that even allows $x$ to be nonnormal. Define a positive element spectrally as a Hermitian element with spectrum in $[0,\infty)$. The calculus of a Hermitian element shows its square is positive. Positivity is closed under sums: for positive $p,q$, let $s=\|p\|+\|q\|$. The calculus gives $\|\|p\|1-p\|\leq\|p\|$ and the analogous bound for $q$, hence $\|s1-p-q\|\leq s$. Since $p+q$ has real spectrum, the spectral [norm](../../../../../norm.md) bound forces it into $[0,2s]$. The cone is proper: an element positive and negative has spectrum in $\{0\}$ and therefore [norm](../../../../../norm.md) zero.

To establish positivity of an arbitrary adjoint product, put $b=x^*x=b^*$. Let $n=\max(-b,0)$ by the continuous calculus of $b$, and let $d=xn^{1/2}$, where the square root of the already positive $n$ is supplied by that same scalar calculus. Multiplicativity gives

$$
d^*d=n^{1/2}bn^{1/2}=-n^2.
$$

Thus $d^*d$ has nonpositive spectrum. The nonzero spectra of $d^*d$ and $dd^*$ agree: for general products $uv,vu$ and $\lambda\ne0$, direct multiplication verifies

$$
(\lambda1-vu)^{-1}=\lambda^{-1}\left[1+v(\lambda1-uv)^{-1}u\right]
$$

whenever the inverse on the right exists, and the converse follows on exchanging $u,v$. Hence $dd^*$ is also nonpositive. Write $d=u+iv$ with [Hermitian C-star elements](../../../../../hermitian-element-of-a-c-star-algebra.md) $u,v$. Then

$$
d^*d+dd^*=2(u^2+v^2)
$$

is positive, as a sum of Hermitian squares, and nonpositive, as a sum of the two nonpositive elements. Properness makes it zero. Therefore $d^*d=-dd^*$ is both positive and nonpositive, hence zero. The [C-star identity](../../../../../c-star-identity.md) gives $d=0$, and $n^2=0$ then implies $n=0$. Thus $b=x^*x$ is positive. This proof does not use positivity of adjoint products in establishing an earlier step.

Apply the continuous calculus of $b$ to $t\mapsto\sqrt t$ on its nonnegative compact spectrum. It gives a positive [Hermitian C-star element](../../../../../hermitian-element-of-a-c-star-algebra.md)

$$
\boxed{h=(x^*x)^{1/2},\qquad h^2=x^*x,\qquad \sigma_A(h)\subseteq[0,\infty)}.
$$

For the originally normal $x$, the equivalent direct formula is $h=\theta_x(z\mapsto|z|)$. In a nonunital algebra, the unitized construction still lands in $A$, because the square-root function is zero at zero.

For uniqueness, suppose $h'=h'^*$ has nonnegative spectrum and $(h')^2=b$. It commutes with $b$, and hence with $h$, which is a [norm](../../../../../norm.md) limit of polynomials in $b$. The unital [C-star algebra](../../../../../c-star-algebra.md) generated by $h,h'$ is therefore commutative. Its [Gelfand transform](../../../../../gelfand-representation.md), together with spectral permanence, gives two nonnegative continuous functions whose squares are equal. Pointwise uniqueness of the nonnegative real square root makes the functions equal, and injectivity of the transform gives $h=h'$. This proves the [positive square root in a C-star algebra](../../../../../positive-square-root-in-a-c-star-algebra.md) in full, without an unwarranted cancellation by $h+h'$ when zero lies in its spectrum. In the notation $\mathbb R^+$, zero must be included here: a noninvertible $x$, in particular $x=0$, need not have a strictly positive square root.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
