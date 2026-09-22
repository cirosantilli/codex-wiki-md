# Paper 4

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2005/PaperIB_4.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2005/PaperIB_4.pdf)

**Table of contents**

- [1B](#1b)
  - [Solution](#1b/solution)
- [2C](#2c)
  - [Solution](#2c/solution)
- [3B](#3b)
  - [Solution](#3b/solution)
- [4A](#4a)
  - [Solution](#4a/solution)
  - [a](#4a/a)
    - [Solution](#4a/a/solution)
  - [b](#4a/b)
    - [Solution](#4a/b/solution)
  - [c](#4a/c)
    - [Solution](#4a/c/solution)
- [5H](#5h)
  - [Solution](#5h/solution)
- [6G](#6g)
  - [Solution](#6g/solution)
- [7H](#7h)
  - [Solution](#7h/solution)
- [8F](#8f)
  - [Solution](#8f/solution)
- [9D](#9d)
  - [Solution](#9d/solution)
- [10B](#10b)
  - [i](#10b/i)
    - [Solution](#10b/i/solution)
  - [ii](#10b/ii)
    - [Solution](#10b/ii/solution)
- [11C](#11c)
  - [Solution](#11c/solution)
- [12A](#12a)
  - [Solution](#12a/solution)
- [13B](#13b)
  - [Solution](#13b/solution)
- [14A](#14a)
  - [Solution](#14a/solution)
- [15F](#15f)
  - [Solution](#15f/solution)
- [16H](#16h)
  - [Solution](#16h/solution)
- [17G](#17g)
  - [Solution](#17g/solution)
- [18E](#18e)
  - [Solution](#18e/solution)
- [19D](#19d)
  - [i](#19d/i)
    - [Solution](#19d/i/solution)
  - [ii](#19d/ii)
    - [Solution](#19d/ii/solution)
  - [iii](#19d/iii)
    - [Solution](#19d/iii/solution)
  - [iv](#19d/iv)
    - [Solution](#19d/iv/solution)
- [20D](#20d)
  - [Solution](#20d/solution)

## 1B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1b/solution">Solution</h3>

↑ **Parent:** [1B](#1b)

Use the standard complex [inner product](../../../linear-algebra.md#inner-product) $\langle u,v\rangle=u^*v$, conjugate-linear in its first argument. A [unitary matrix](../../../linear-operator-theory.md#unitary-matrix) satisfies $U^*U=I$, and a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) satisfies $H^*=H$, where $*$ is conjugate transpose.

If $Hv=\lambda v$ with $v\ne0$, then

$$
\lambda\langle v,v\rangle=\langle v,Hv\rangle=\langle Hv,v\rangle=\overline\lambda\langle v,v\rangle.
$$

Positivity of $\langle v,v\rangle$ proves $\boxed{\lambda\in\mathbb R}$. If $Uv=\lambda v$, preservation of the [norm](../../../functional-analysis.md#norm) gives $\|v\|^2=\|Uv\|^2=|\lambda|^2\|v\|^2$, so $\boxed{|\lambda|=1}$.

For [eigenvectors](../../../linear-operator-theory.md#eigenvector) $Hv=\lambda v$ and $Hw=\mu w$, the [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) identity gives $\langle v,Hw\rangle=\langle Hv,w\rangle$. The already established reality of the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) therefore implies $(\mu-\lambda)\langle v,w\rangle=0$. Thus **distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) have orthogonal [eigenvectors](../../../linear-operator-theory.md#eigenvector)**.

## 2C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2c/solution">Solution</h3>

↑ **Parent:** [2C](#2c)

The [Eisenstein criterion](../../../commutative-algebra.md#eisenstein-criterion) says that a primitive integer [polynomial](../../../polynomial.md) $P(x)=a_mx^m+\cdots+a_0$ is irreducible over $\mathbb Q$ if some [prime number](../../../number-theory.md#prime-number) $p$ divides every $a_j$ for $j<m$, does not divide $a_m$, and $p^2$ does not divide $a_0$. By [Gauss lemma for polynomials](../../../commutative-algebra.md#gauss-lemma-for-polynomials), this gives irreducibility in $\mathbb Z[x]$ as well.

For prime $n=p$, translate the variable in $P_p(x)=(x^p-1)/(x-1)$:

$$
P_p(x+1)=\frac{(x+1)^p-1}{x}=\sum_{j=1}^p\binom pj x^{j-1}.
$$

Its leading coefficient is one, all other coefficients are divisible by $p$, and its constant coefficient is exactly $p$. The [Eisenstein criterion](../../../commutative-algebra.md#eisenstein-criterion) proves this translated [polynomial](../../../polynomial.md) irreducible. Since $x\mapsto x+1$ is an invertible substitution in $\mathbb Z[x]$, $P_p$ is irreducible too.

If $n=ab$ with $a,b>1$, then

$$
P_n(x)=(1+x+\cdots+x^{a-1})(1+x^a+\cdots+x^{(b-1)a}).
$$

Both factors have positive degree and integer coefficients, proving reducibility. Consequently $\boxed{1+x+\cdots+x^{n-1}\text{ is irreducible exactly when }n\text{ is prime}.}$

## 3B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3b/solution">Solution</h3>

↑ **Parent:** [3B](#3b)

The integral is finite and nonnegative because $|f|$ is [continuous](../../../calculus.md#continuous-function) on a compact interval. If it vanishes and $f(x_*)\ne0$, continuity gives a relative interval of positive length on which $|f|\geq|f(x_*)|/2$, a contradiction. Thus the integral is zero only for $f=0$. For a real scalar $a$, $\|af\|=|a|\|f\|$, and the pointwise [triangle inequality](../../../topological-analysis.md#triangle-inequality) $|f+g|\leq|f|+|g|$ integrates to $\|f+g\|\leq\|f\|+\|g\|$. These are all the [norm](../../../functional-analysis.md#norm) axioms.

The given sequence satisfies

$$
\boxed{\|f_n-0\|=\int_0^1e^{-nx}\,dx=\frac{1-e^{-n}}n\longrightarrow0.}
$$

Hence **it converges to the zero function in this integral [norm](../../../functional-analysis.md#norm)**. Although $f_n(0)=1$ for all $n$, an isolated endpoint contributes no integral. The pointwise limit is discontinuous, and the sequence does not converge in the [uniform norm](../../../functional-analysis.md#supremum-norm); neither fact obstructs convergence in the stated [norm](../../../functional-analysis.md#norm).

## 4A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4a/solution">Solution</h3>

↑ **Parent:** [4A](#4a)

For a closed piecewise continuously differentiable [path](../../../geometry-and-topology.md#continuous-path) avoiding $a$, the [winding number](../../../complex-analysis.md#winding-number) is

$$
\boxed{n(\gamma,a)=\frac1{2\pi i}\oint_\gamma\frac{dz}{z-a}=\frac1{2\pi i}\int_0^1\frac{\gamma'(t)}{\gamma(t)-a}\,dt.}
$$

Break the parameter interval at the finitely many derivative discontinuities when evaluating this integral. Translating the curve gives $n(\gamma,a)=n(\gamma-a,0)$, which will also be used below.

<h3 id="4a/a">a</h3>

↑ **Parent:** [4A](#4a)

<h4 id="4a/a/solution">Solution</h4>

↑ **Parent:** [A](#4a/a)

Where both derivatives exist, the ordinary product rule gives

$$
\frac{(\gamma_1\gamma_2)'}{\gamma_1\gamma_2}=\frac{\gamma_1'}{\gamma_1}+\frac{\gamma_2'}{\gamma_2}.
$$

Neither denominator vanishes. Integrate over a common piecewise-smooth subdivision and use the contour characterization of the [winding number](../../../complex-analysis.md#winding-number):

$$
\boxed{n(\gamma_1\gamma_2,0)=n(\gamma_1,0)+n(\gamma_2,0).}
$$

<h3 id="4a/b">b</h3>

↑ **Parent:** [4A](#4a)

<h4 id="4a/b/solution">Solution</h4>

↑ **Parent:** [B](#4a/b)

On the right half-plane a single-valued [holomorphic logarithm](../../../complex-analysis.md#holomorphic-logarithm) is $\operatorname{Log}z=\log|z|+i\operatorname{Arg}z$, with $-\pi/2<\operatorname{Arg}z<\pi/2$, and its derivative is $1/z$. Thus

$$
\oint_\eta\frac{dz}{z}=\operatorname{Log}\eta(1)-\operatorname{Log}\eta(0)=0,
\qquad \boxed{n(\eta,0)=0.}
$$

This proves the conclusion directly from the integral definition of the [winding number](../../../complex-analysis.md#winding-number), without appealing to its homotopy invariance.

<h3 id="4a/c">c</h3>

↑ **Parent:** [4A](#4a)

<h4 id="4a/c/solution">Solution</h4>

↑ **Parent:** [C](#4a/c)

Put $\eta=(\gamma_2-a)/(\gamma_1-a)$. The strict inequality gives $|\eta-1|<1$, so $\operatorname{Re}\eta>0$. This is a closed piecewise-smooth curve in the right half-plane, and part (b) gives $n(\eta,0)=0$. Since $\gamma_2-a=(\gamma_1-a)\eta$, part (a) yields

$$
n(\gamma_2,a)=n(\gamma_1,a)+n(\eta,0),
\qquad \boxed{n(\gamma_2,a)=n(\gamma_1,a).}
$$

This is the [dominated perturbation preserves winding number](../../../complex-analysis.md#dominated-perturbation-preserves-winding-number) principle, here derived by logarithmic differentiation.

## 5H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5h/solution">Solution</h3>

↑ **Parent:** [5H](#5h)

Take characteristic coordinates $\xi=ct-x$ and $\eta=ct+x$. Then $c^{-2}y_{tt}-y_{xx}=4y_{\xi\eta}$. The [wave equation](../../../wave-equation.md) is therefore $y_{\xi\eta}=0$, whose general twice-differentiable solution is

$$
\boxed{y(x,t)=f(ct-x)+g(ct+x).}
$$

The first fixed-end boundary gives $f(s)=-g(s)$. The second gives $g(s+L)=g(s-L)$, hence $g(s+2L)=g(s)$; $f$ has the same period. Thus $y=g(ct+x)-g(ct-x)$ with a $2L$-periodic function $g$.

Let $A=g'(ct+x)$ and $B=g'(ct-x)$. Then $y_t=c(A-B)$ and $y_x=A+B$, so the quadratic energy density reduces to $\tfrac12[(A-B)^2+(A+B)^2]=A^2+B^2$. Changing $x$ to $-x$ in the second integral proves

$$
\boxed{\frac12\int_0^L(c^{-2}y_t^2+y_x^2)\,dx=\int_{-L}^L g'(ct+x)^2\,dx.}
$$

The right side integrates a periodic function over one full period and is independent of its starting point. More explicitly its time derivative is $c[g'(ct+L)^2-g'(ct-L)^2]=0$. This is **conservation of the fixed-end wave energy**.

## 6G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6g/solution">Solution</h3>

↑ **Parent:** [6G](#6g)

The [operator commutator](../../../vector-space.md#operator-commutator) is $[A,B]=AB-BA$, acting on a common domain where both products are defined. Use the [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation) $[x_i,p_j]=i\hbar\delta_{ij}$, with positions mutually commuting and momenta mutually commuting. On smooth test functions the only nonzero terms in the expansion are

$$
[yp_z,zp_x]=-i\hbar yp_x,\qquad [zp_y,xp_z]=i\hbar xp_y.
$$

Thus the [orbital angular momentum commutation relations](../../../quantum-mechanics.md#orbital-angular-momentum-commutation-relations) give

$$
\boxed{[L_x,L_y]=i\hbar(xp_y-yp_x)=i\hbar L_z,\qquad [L_i,L_j]=i\hbar\epsilon_{ijk}L_k.}
$$

The product rule for a [operator commutator](../../../vector-space.md#operator-commutator) gives

$$
[L^2,L_w]=\sum_i\big(L_i[L_i,L_w]+[L_i,L_w]L_i\big)
=i\hbar\sum_{i,k}\epsilon_{iwk}(L_iL_k+L_kL_i)=0,
$$

because the last operator expression is symmetric in $i,k$, whereas $\epsilon_{iwk}$ is antisymmetric. Hence $\boxed{[L^2,L_w]=0}$ for every component.

Write $r=\sqrt{x^2+y^2+z^2}$ and $P=x+y+z$. The differential [angular momentum operator](../../../quantum-mechanics.md#angular-momentum-operator) $L=-i\hbar\,x\times\nabla$ annihilates every radial function, so $L_i(Pe^{-r})=e^{-r}L_iP$ and the same holds for its square. For example $L_xx=0$, $L_y^2x=\hbar^2x$ and $L_z^2x=\hbar^2x$. Cyclic symmetry gives $L^2y=2\hbar^2y$ and $L^2z=2\hbar^2z$ as well. Therefore

$$
\boxed{L^2\psi=e^{-r}L^2P=2\hbar^2\psi.}
$$

The wavefunction is an $l=1$ [orbital angular momentum](../../../quantum-mechanics.md#orbital-angular-momentum) state; its nontrivial radial factor does not change its angular [eigenvalue](../../../linear-operator-theory.md#eigenvalue). The calculation holds away from the origin and defines the same angular-operator identity in the square-integrable state space.

## 7H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7h/solution">Solution</h3>

↑ **Parent:** [7H](#7h)

For static fields, the [Maxwell equations](../../../electromagnetism.md#maxwell-equations) give $\nabla\times B=\mu_0J$ and $\nabla\cdot B=0$. Write $B=\nabla\times A$. A [gauge transformation](../../../electromagnetism.md#gauge-transformation) $A\mapsto A+\nabla\chi$ leaves $B$ unchanged; choose $\Delta\chi=-\nabla\cdot A$ to impose the [Coulomb gauge](../../../electromagnetism.md#coulomb-gauge). Then

$$
\nabla\times(\nabla\times A)=\nabla(\nabla\cdot A)-\Delta A=\mu_0J,
\qquad \boxed{-\Delta A=\mu_0J.}
$$

For a localized conserved current with the potential chosen to vanish at infinity, the supplied fundamental solution gives the [magnetic vector potential](../../../electromagnetism.md#magnetic-vector-potential)

$$
A(x)=\frac{\mu_0}{4\pi}\int\frac{J(r)}{|x-r|}\,d^3r.
$$

Its divergence vanishes by integration by parts and $\nabla\cdot J=0$. For a filamentary loop the current integral becomes $I\oint_Ldr$, so

$$
\boxed{A(x)=\frac{\mu_0I}{4\pi}\oint_L\frac{dr}{|x-r|}.}
$$

For $R=|x|$ much larger than the fixed loop size, expand $|x-r|^{-1}=R^{-1}+(x\cdot r)R^{-3}+O(R^{-3})$. The leading constant term integrates to zero because $\oint dr=0$. Therefore

$$
A(x)=\frac{\mu_0I}{4\pi R^3}\oint(x\cdot r)\,dr+O(R^{-3}).
$$

The vector triple-product identity gives $x\times(r\times dr)=r(x\cdot dr)-(x\cdot r)dr$. Integrating the derivative of $(x\cdot r)r$ around the closed loop shows $\oint r(x\cdot dr)=-\oint(x\cdot r)dr$. Consequently

$$
\boxed{A(x)=-\frac{\mu_0I}{4\pi R^3}\oint\frac12x\times(r\times dr)+O(R^{-3}).}
$$

Equivalently, $A=\mu_0m\times x/(4\pi R^3)+O(R^{-3})$, where $m=(I/2)\oint r\times dr$ is the [magnetic dipole moment](../../../electromagnetism.md#magnetic-dipole-moment). The leading displayed potential is of order $R^{-2}$; the remainder is smaller by a factor $R^{-1}$.

## 8F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8f/solution">Solution</h3>

↑ **Parent:** [8F](#8f)

An $n$-node [Gaussian quadrature](../../../numerical-analysis.md#gaussian-quadrature) formula chooses nodes and weights for an integral with a positive weight so that every [polynomial](../../../polynomial.md) of degree at most $2n-1$ is integrated exactly. Its nodes are the zeros of the degree-$n$ [orthogonal polynomial](../../../numerical-analysis.md#orthogonal-polynomial) for that weight.

For the even weight $w(x)=1-x^2$, the monic orthogonal quadratic has the form $p_2(x)=x^2-d$. Orthogonality to $x$ follows from oddness; orthogonality to one gives

$$
d=\frac{\int_{-1}^1x^2(1-x^2)dx}{\int_{-1}^1(1-x^2)dx}=\frac{4/15}{4/3}=\frac15.
$$

The nodes are $\pm1/\sqrt5$. The equal weights sum to $4/3$, hence each is $2/3$. The [two-node Gaussian quadrature with quadratic weight](../../../numerical-analysis.md#two-node-gaussian-quadrature-with-quadratic-weight) is therefore

$$
\boxed{\int_{-1}^1(1-x^2)f(x)dx\simeq\frac23\left[f(-1/\sqrt5)+f(1/\sqrt5)\right].}
$$

To verify cubic exactness, divide any cubic as $P=p_2Q+R$ with $\deg Q,\deg R\leq1$. Orthogonality removes $p_2Q$ from the integral and its nodal values vanish; linear interpolation integrates $R$ exactly. This also proves the Gaussian property rather than merely matching two moments.

## 9D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9d/solution">Solution</h3>

↑ **Parent:** [9D](#9d)

Let $S_m$ be the [simple symmetric random walk](../../../probability-theory.md#simple-symmetric-random-walk) started at the origin. Odd-time returns are impossible by parity. A return in $2n$ steps requires equal numbers of positive and negative steps along each axis. If these paired counts are $i,j,k$ with $i+j+k=n$, counting the possible step arrangements gives

$$
p_{2n}:=P(S_{2n}=0)=\frac{(2n)!}{6^{2n}}\sum_{i+j+k=n}\frac1{i!^2j!^2k!^2}.
$$

Define $q_{ijk}=n!/(3^ni!j!k!)$. These are [multinomial distribution](../../../discrete-probability-distribution.md#multinomial-distribution) probabilities and sum to one. Rearranging the return formula gives

$$
p_{2n}=\frac{\binom{2n}{n}}{4^n}\sum_{i+j+k=n}q_{ijk}^2
\leq\frac{\binom{2n}{n}}{4^n}\max_{i+j+k=n}q_{ijk}.
$$

The maximum occurs when the three counts differ by at most one: if $i\geq j+2$, replacing $(i,j)$ by $(i-1,j+1)$ multiplies $q$ by $i/(j+1)>1$. At balanced counts, [Stirling's formula](../../../real-analysis.md#stirling-formula) gives $\max q=O(n^{-1})$; the exponential factors cancel because each count is $n/3+O(1)$, and the square-root factorial factors leave one inverse power of $n$. The same formula gives $\binom{2n}{n}/4^n\sim(\pi n)^{-1/2}$. Hence

$$
\boxed{p_{2n}=O(n^{-3/2}),\qquad \sum_{m\geq0}P(S_m=0)<\infty.}
$$

This is the [multinomial collision proof of three-dimensional walk transience](../../../probability-theory.md#multinomial-collision-proof-of-three-dimensional-walk-transience). The sum is the expected total number of visits to the origin. If the probability of returning after departure were one, the [Strong Markov property](../../../markov-process.md#strong-markov-property) at successive returns would make every successive return finite almost surely, giving infinitely many visits and contradicting that finite expectation. Thus the origin is a [transient state](../../../markov-process.md#transient-state). Translation invariance gives the same conclusion at every lattice point: **the three-dimensional walk is transient**.

## 10B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10b/i">i</h3>

↑ **Parent:** [10B](#10b)

<h4 id="10b/i/solution">Solution</h4>

↑ **Parent:** [I](#10b/i)

Apply the [Gram-Schmidt process](../../../linear-algebra.md#gram-schmidt-process) explicitly. Start with $f_1=e_1/\|e_1\|$, and for $i\geq2$ set

$$
v_i=e_i-\sum_{j=1}^{i-1}\langle e_i,f_j\rangle f_j,\qquad f_i=v_i/\|v_i\|.
$$

Assume inductively that the previous $f_j$ form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) for the span of $e_1,\ldots,e_{i-1}$. [Inner products](../../../linear-algebra.md#inner-product) give $\langle v_i,f_j\rangle=0$ for every $j<i$. Moreover $v_i\ne0$: otherwise $e_i$ would lie in the span of its predecessors, contradicting that the $e_j$ form a [basis](../../../vector-space.md#basis). Thus $f_i$ is well defined and has unit [norm](../../../functional-analysis.md#norm). The definition expresses $f_i$ in the span of $e_1,\ldots,e_i$, and also expresses $e_i$ in the span of $f_1,\ldots,f_i$. The two spans therefore agree at each stage. Induction proves **the required orthonormal, span-preserving basis**.

<h3 id="10b/ii">ii</h3>

↑ **Parent:** [10B](#10b)

<h4 id="10b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10b/ii)

The symmetric coefficient [matrix](../../../vector-space.md#matrix) of the [quadratic form](../../../linear-algebra.md#quadratic-form) is

$$
Q_a=\begin{pmatrix}a&1/2&1/2\\1/2&0&1/2\\1/2&1/2&0\end{pmatrix},\qquad \det Q_a=\frac{1-a}{4}.
$$

Thus $\boxed{q_a\text{ is nondegenerate if and only if }a\ne1.}$ To obtain its [signature](../../../linear-algebra.md#signature-of-a-quadratic-form), put $u=(y+z)/2$ and $v=(y-z)/2$. Completing the square yields

$$
q_a=(u+x)^2-v^2+(a-1)x^2.
$$

The transformation from $(x,y,z)$ to $(u+x,v,x)$ is invertible. The [inertia of a bilinear form](../../../linear-algebra.md#inertia-of-a-bilinear-form) is consequently

$$
\boxed{(n_+,n_-)=\begin{cases}(2,1)&a>1,\\(1,2)&a<1.\end{cases}}
$$

If signature means the signed difference $n_+-n_-$, its value is $+1$ for $a>1$ and $-1$ for $a<1$. At $a=1$ the diagonal form has one zero direction, confirming degeneracy.

## 11C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11c/solution">Solution</h3>

↑ **Parent:** [11C](#11c)

Let $\pi$ be a [prime element](../../../commutative-algebra.md#prime-element) of the [Gaussian integers](../../../commutative-algebra.md#gaussian-integer). Its [norm](../../../functional-analysis.md#norm) $\pi\overline\pi$ is a positive integer greater than one, so $\pi$ divides some ordinary positive [prime number](../../../number-theory.md#prime-number) in its integer prime factorization. It cannot divide two distinct such primes $p,q$: an integer Bézout identity $up+vq=1$ would imply $\pi\mid1$, contrary to its being a nonunit. This proves existence and uniqueness of the rational prime lying below $\pi$.

Up to associates, the complete list of Gaussian [prime elements](../../../commutative-algebra.md#prime-element) is: $1+i$; the positive rational primes $p\equiv3\pmod4$; and, for every rational prime $p\equiv1\pmod4$, the two nonassociate elements $a+bi$ and $a-bi$, where $a,b>0$ and $p=a^2+b^2$. Representatives related by multiplication by one of $\pm1,\pm i$ are associates. The last pair accounts for both factors of a split prime.

Every residue class modulo $p$ has a unique representative $a+bi$ with $0\leq a,b<p$, since $p\mid(a-a')+(b-b')i$ means both coordinate differences are divisible by $p$. Hence $\boxed{|R/pR|=p^2}$ and

$$
R/pR\cong\mathbb F_p[X]/(X^2+1).
$$

For $p=2$, the class of $1+i$ is nonzero but its square is $2i=0$; thus the [quotient ring](../../../commutative-algebra.md#quotient-ring) is not a [field](../../../algebra.md#field). For $p\equiv3\pmod4$, a root $r^2=-1$ would imply $r^{p-1}=(-1)^{(p-1)/2}=-1$, contradicting [Fermat's little theorem](../../../number-theory.md#fermat-little-theorem). The quadratic $X^2+1$ is therefore irreducible and its quotient is a [field](../../../algebra.md#field) with $p^2$ elements.

For $p\equiv1\pmod4$, choose a generator $g$ of the cyclic group $\mathbb F_p^\times$. Then $r=g^{(p-1)/4}$ satisfies $r^2=-1$. The two nonzero classes $i-r$ and $i+r$ have product zero in $R/pR$. Thus

$$
\boxed{R/pR\text{ is a field exactly for rational primes }p\equiv3\pmod4.}
$$

For $p\equiv1\pmod4$ it is instead isomorphic to $\mathbb F_p\times\mathbb F_p$, by the distinct linear factors and the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem).

## 12A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12a/solution">Solution</h3>

↑ **Parent:** [12A](#12a)

At $P=\sigma(u,v)$, regularity makes $\sigma_u,\sigma_v$ linearly independent. The [tangent space](../../../differential-geometry.md#tangent-space) is $T_PU=\operatorname{span}\{\sigma_u,\sigma_v\}$, and an oriented unit [normal vector](../../../differential-geometry.md#normal-vector) is

$$
\boldsymbol n=\frac{\sigma_u\times\sigma_v}{|\sigma_u\times\sigma_v|}.
$$

Reversing its sign chooses the opposite orientation. The [first fundamental form](../../../differential-geometry.md#first-fundamental-form) is the squared length of a tangent displacement:

$$
|\sigma_u\,du+\sigma_v\,dv|^2=E\,du^2+2F\,du\,dv+G\,dv^2,
$$

where $E=\sigma_u\cdot\sigma_u$, $F=\sigma_u\cdot\sigma_v$, $G=\sigma_v\cdot\sigma_v$. Its determinant $EG-F^2=|\sigma_u\times\sigma_v|^2$ is positive.

Use $N_{\rm II}=\sigma_{vv}\cdot\boldsymbol n$ to distinguish the scalar coefficient of the [second fundamental form](../../../second-fundamental-form.md) from the [normal vector](../../../differential-geometry.md#normal-vector). Since $\boldsymbol n\cdot\boldsymbol n=1$, its derivatives are perpendicular to it and hence tangent. Write $\boldsymbol n_u=a\sigma_u+b\sigma_v$ and $\boldsymbol n_v=c\sigma_u+d\sigma_v$. Differentiating $\boldsymbol n\cdot\sigma_u=\boldsymbol n\cdot\sigma_v=0$ gives

$$
\boldsymbol n_u\cdot\sigma_u=-L,\quad \boldsymbol n_u\cdot\sigma_v=-M,\quad
\boldsymbol n_v\cdot\sigma_u=-M,\quad \boldsymbol n_v\cdot\sigma_v=-N_{\rm II}.
$$

Substitution of the tangent expansions proves

$$
\boxed{-\begin{pmatrix}L&M\\M&N_{\rm II}\end{pmatrix}=\begin{pmatrix}a&b\\c&d\end{pmatrix}\begin{pmatrix}E&F\\F&G\end{pmatrix}.}
$$

The [shape operator](../../../second-fundamental-form.md#shape-operator) is $-d\boldsymbol n$; its [matrix](../../../vector-space.md#matrix) in the parametrized tangent basis is the negative transpose of the coefficient [matrix](../../../vector-space.md#matrix) shown. Its determinant, the product of the principal curvatures, is therefore

$$
\boxed{ad-bc=\frac{LN_{\rm II}-M^2}{EG-F^2}=K,}
$$

the [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature). Transposition and the two minus signs do not change this determinant.

## 13B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="13b/solution">Solution</h3>

↑ **Parent:** [13B](#13b)

The [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) shows that the differential initial-value problem is equivalent to

$$
x(t)=x_0+\int_0^tF(s,x(s))\,ds.
$$

In one direction integrate $x'=F(t,x(t))$ from zero. In the other, continuity of the integrand makes the right side continuously differentiable with precisely that derivative and initial value.

Consider the closed subset $\mathcal X=\{x\in C([-b,b]):\|x-x_0\|_\infty\leq r\}$ of the complete space with the [uniform norm](../../../functional-analysis.md#supremum-norm). It is complete: a uniformly Cauchy sequence has a uniform continuous limit, and the closed range constraint passes to the limit. Define

$$
(Tx)(t)=x_0+\int_0^tF(s,x(s))\,ds.
$$

The bound $|F|\leq C$ gives $\|Tx-x_0\|_\infty\leq bC<r$, so $T$ maps $\mathcal X$ into itself. The uniform [Lipschitz condition](../../../real-analysis.md#lipschitz-continuity) gives

$$
\boxed{\|Tx-Ty\|_\infty\leq bK\|x-y\|_\infty,\qquad q:=bK<1.}
$$

Here negative $t$ changes only the orientation of the integral; its length is still at most $b$.

Construct $x^{(0)}(t)=x_0$ and $x^{(m+1)}=Tx^{(m)}$. Induction gives $\|x^{(m+1)}-x^{(m)}\|_\infty\leq q^m\|x^{(1)}-x^{(0)}\|_\infty$. Summing this geometric bound proves uniform Cauchy convergence to some $x\in\mathcal X$. The same contraction estimate shows $Tx^{(m)}\to Tx$, so $x=Tx$. The integral equation now makes $x$ a $C^1$ solution. If another solution $y$ existed, it would also be fixed, and $\|x-y\|_\infty\leq q\|x-y\|_\infty$ would force equality. This proves **existence and uniqueness on the entire stated interval**, implementing the [contraction mapping theorem](../../../analysis.md#contraction-mapping-theorem) rather than just invoking it.

If $C=0$, the vector field is zero and the solution is constant. If $K=0$, the vector field is independent of the space variable and the integral solves the problem directly. The divisions by zero in the printed interval bound are naturally interpreted as imposing no restriction from the corresponding term.

## 14A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="14a/solution">Solution</h3>

↑ **Parent:** [14A](#14a)

For nonempty $F$, the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives $d(x,z)\leq d(x,y)+d(y,z)$ for every $z\in F$. Taking the infimum yields $d(x,F)\leq d(x,y)+d(y,F)$. Interchanging $x,y$ proves

$$
\boxed{|d(x,F)-d(y,F)|\leq d(x,y).}
$$

Thus the [distance to a set](../../../topological-analysis.md#distance-to-a-set) is a [Lipschitz function](../../../real-analysis.md#lipschitz-continuity), hence continuous. If $x\notin F$ and $F$ is closed, its open complement contains a ball $B(x,\epsilon)$; every point of $F$ is at least $\epsilon$ away. Hence $\boxed{d(x,F)>0}$ for $x\notin F$.

For two nonempty disjoint closed sets, let $h(x)=d(x,F_1)-d(x,F_2)$. It is continuous, negative on $F_1$ and positive on $F_2$. The disjoint open sets $U_1=\{h<0\}$ and $U_2=\{h>0\}$ contain them. Empty sets cause no difficulty, using an empty neighborhood for the empty set. This proves **every metric space is a [normal topological space](../../../topology.md#normal-space)**.

In any normal space, a closed $F$ contained in an open $U$ can be separated from $X\setminus U$: choose disjoint open $W\supset F$ and $V\supset X\setminus U$. Because $X\setminus V$ is closed and contains $W$, $\overline W\subset X\setminus V\subset U$. First choose disjoint open $U_1,U_2$ around $F_1,F_2$, then apply this argument separately to each pair $F_i\subset U_i$. It gives $\overline W_i\subset U_i$, and therefore $\boxed{\overline W_1\cap\overline W_2=\varnothing}$. This is [closed-neighborhood shrinking in a normal space](../../../topology.md#closed-neighborhood-shrinking-in-a-normal-space).

For the two specified hyperbola branches, explicit choices are

$$
\boxed{W_1=\{(x,y):x<0,\ xy<-1/2\},\qquad W_2=\{(x,y):x>0,\ xy>1/2\}.}
$$

They are open and contain the branches with products $-1$ and $1$. Their closures lie respectively in $\{x\leq0,xy\leq-1/2\}$ and $\{x\geq0,xy\geq1/2\}$. Any common point would have $x=0$, making both product inequalities impossible. Thus their closures are disjoint even though the original branches can approach one another arbitrarily closely at large height.

## 15F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="15f/solution">Solution</h3>

↑ **Parent:** [15F](#15f)

The function is odd, so its [Fourier series](../../../fourier-series.md) has no constant or cosine terms. If $\lambda=m\in\mathbb Z$, it is already a Fourier basis function: for $m>0$ the only sine coefficient is $b_m=1$; for $m<0$ it is $b_{|m|}=-1$; for $m=0$ the function is zero.

For real noninteger $\lambda$, the product-to-sum identity gives

$$
b_n=\frac2\pi\int_0^\pi\sin(\lambda x)\sin(nx)\,dx
=\frac1\pi\left[\frac{\sin((\lambda-n)\pi)}{\lambda-n}-\frac{\sin((\lambda+n)\pi)}{\lambda+n}\right].
$$

Since both numerator sines equal $(-1)^n\sin(\pi\lambda)$, the [Fourier series of a noninteger-frequency sine](../../../fourier-series.md#fourier-series-of-a-noninteger-frequency-sine) is

$$
\boxed{\sin(\lambda x)\sim\sum_{n\geq1}\frac{2(-1)^{n+1}n\sin(\pi\lambda)}{\pi(n^2-\lambda^2)}\sin(nx).}
$$

It equals the function for $-\pi<x<\pi$. At either periodic endpoint it equals the average of the two one-sided limits, namely zero; the noninteger-frequency function has a jump in its periodic extension there. Equality also holds in the square-integral sense on the full interval.

For $\lambda=1/2$, $b_n=8(-1)^{n+1}n/[\pi(4n^2-1)]$ and $\int_{-\pi}^\pi\sin^2(x/2)\,dx=\pi$. The [Parseval identity](../../../fourier-analysis.md#parseval-identity) for a real sine series is $(1/\pi)\int_{-\pi}^\pi f^2=\sum_{n\geq1}b_n^2$. Hence

$$
1=\frac{64}{\pi^2}\sum_{n\geq1}\frac{n^2}{(4n^2-1)^2},\qquad
\boxed{\sum_{n\geq1}\frac{n^2}{(4n^2-1)^2}=\frac{\pi^2}{64}.}
$$

## 16H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="16h/solution">Solution</h3>

↑ **Parent:** [16H](#16h)

An [isotropic tensor](../../../linear-algebra.md#isotropic-tensor) has unchanged components under every proper orthogonal change of basis: $T_{i_1\ldots i_n}=R_{i_1j_1}\cdots R_{i_nj_n}T_{j_1\ldots j_n}$ for every $R\in SO(3)$. Orthogonality gives $R_{ia}R_{jb}\delta_{ab}=\delta_{ij}$, so the [Kronecker delta](../../../linear-algebra.md#kronecker-delta) is isotropic. The determinant identity gives $R_{ia}R_{jb}R_{kc}\epsilon_{abc}=(\det R)\epsilon_{ijk}=\epsilon_{ijk}$, so the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) is isotropic too. If reflections are included, this last object is a pseudotensor: it changes sign. The question's isotropy convention therefore refers to proper rotations.

For the sphere moment $T_{i_1\ldots i_n}=\int_{S^2}\hat x_{i_1}\cdots\hat x_{i_n}\,dS$, change variables to $R\hat x$. Rotations preserve the sphere and its area measure; inserting the component transformation proves that $T$ is an [isotropic tensor](../../../linear-algebra.md#isotropic-tensor). For the second moment, half-turns about coordinate axes kill the off-diagonal components, while rotations interchanging axes make the diagonal entries equal. Thus it is a multiple $a\delta_{ij}$. Contracting the indices gives $3a=\int_{S^2}|\hat x|^2dS=4\pi$. Odd moments vanish by $\hat x\mapsto-\hat x$, including the third moment. The supplied general fourth-rank form and symmetry under every permutation of the four indices make its three coefficients equal. A double contraction then gives $4\pi=b(9+3+3)$. Thus

$$
\boxed{\int\hat x_i\hat x_j\,dS=\frac{4\pi}{3}\delta_{ij},\qquad \int\hat x_i\hat x_j\hat x_k\,dS=0,}
$$



$$
\boxed{\int\hat x_i\hat x_j\hat x_k\hat x_l\,dS=\frac{4\pi}{15}(\delta_{ij}\delta_{kl}+\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}).}
$$

To explain the weighted volume integrals, put $v=(1,i,0)$; its bilinear square is $v\cdot v=1+i^2=0$, without complex conjugation. Separating radial and angular factors gives

$$
\int_{|x|<1}(x_1+ix_2)^nf(|x|)\,d^3x
=\left(\int_0^1r^{n+2}f(r)\,dr\right)\int_{S^2}(v\cdot\hat x)^n\,dS.
$$

For $n=2$ the angular factor is $(4\pi/3)v\cdot v=0$. For $n=3$ it is zero by oddness. For $n=4$ it is $(4\pi/15)3(v\cdot v)^2=0$. Therefore **all three requested integrals vanish**, assuming the radial integrals exist. More generally the [null-vector cancellation of radial moments](../../../geometry-and-topology.md#null-vector-cancellation-of-radial-moments) follows from rotation about the third axis, which multiplies the integral by $e^{in\phi}$ without otherwise changing it.

## 17G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="17g/solution">Solution</h3>

↑ **Parent:** [17G](#17g)

Assume homogeneous space and time, isotropic space, inertial frames related linearly, the relativity principle and a common isotropic speed $c$ for light. Take coincident origins at zero and parallel axes, with $S'$ moving at $v$ along $x$. The primed origin requires $x'=A(x-vt)$. Write $t'=Bx+Dt$; mapping each light ray $x=\pm ct$ into $x'=\pm ct'$ gives $D=A$ and $B=-Av/c^2$. Rotational symmetry about the boost axis gives a common transverse scale $B(v)$; reversing the boost direction by spatial isotropy gives $B(v)=B(-v)$. Reciprocity then gives $B(v)^2=1$, and continuity and the common orientation select $B(v)=1$. Thus transverse directions are unchanged. Reciprocity requires the inverse to have the same scale $A$ with $v$ replaced by $-v$. Composing gives $A^2(1-v^2/c^2)=1$; continuity from $A=1$ at $v=0$ selects the positive root. Hence the [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) is

$$
\boxed{x'=\gamma(x-vt),\quad t'=\gamma(t-vx/c^2),\quad y'=y,\quad z'=z,\qquad \gamma=(1-v^2/c^2)^{-1/2}.}
$$

The printed wavelength formula uses the angle of the line of sight from observer towards star, opposite to photon propagation. Choose the transverse axis so the ray lies in the $xy$ plane. With that directed-angle convention the photon [four-momentum](../../../special-relativity.md#four-momentum) is

$$
\boxed{p'^\mu=\frac{h\nu'}c(1,-\cos\theta',-\sin\theta',0),\qquad p^\mu=\frac{h\nu}c(1,-\cos\theta,-\sin\theta,0).}
$$

The inverse coordinate boost takes a rest-frame four-vector to $S$, giving $p^0=\gamma(p'^0+\beta p'^1)$ and $p^1=\gamma(p'^1+\beta p'^0)$, where $\beta=v/c$. Thus $\nu=\gamma\nu'(1-\beta\cos\theta')$, and the [aberration of light](../../../physics.md#relativistic-aberration) relation is $\cos\theta=(\cos\theta'-\beta)/(1-\beta\cos\theta')$. More directly, the boost from $S$ to $S'$ gives $p'^0=\gamma(p^0-\beta p^1)$, hence $\nu'=\gamma\nu(1+\beta\cos\theta)$. Since wavelength is $c/\nu$, the [relativistic Doppler effect](../../../physics.md#relativistic-doppler-effect) gives

$$
\boxed{\lambda=\lambda'\gamma(1+\beta\cos\theta).}
$$

If the angle were instead measured along the actual photon momentum, both cosine signs would reverse and the same physical relation would have a minus sign. Specifying this orientation avoids confusing the two versions.

For $\cos\theta=1$, $\lambda/\lambda'=\sqrt{(1+\beta)/(1-\beta)}$: a receding star is redshifted. For $\cos\theta=-1$, the ratio is $\sqrt{(1-\beta)/(1+\beta)}$: an approaching star is blueshifted. For $\cos\theta=0$, $\boxed{\lambda/\lambda'=\gamma}$: the transverse redshift is the time-dilation effect. This transverse condition refers to the observer's angle, not $\theta'=\pi/2$ in the source frame.

## 18E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="18e/solution">Solution</h3>

↑ **Parent:** [18E](#18e)

Use the standard ideal-fluid assumptions underlying the stated relation: both fluids are incompressible, inviscid and unbounded away from the interface, with no surface tension. An [irrotational flow](../../../fluid-mechanics.md#irrotational-flow) has $u_j=\nabla\phi_j$, and [incompressibility](../../../fluid-mechanics.md#incompressible-flow) gives $\Delta\phi_j=0$ in each fluid. The unsteady [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) is

$$
\phi_{j,t}+\tfrac12|\nabla\phi_j|^2+\frac{p_j}{\rho_j}+gz=C_j(t),
$$

where the arbitrary time functions can be absorbed into the potentials. On $z=\zeta(x,t)$ the material-interface and normal-stress conditions are

$$
\zeta_t+\phi_{j,x}\zeta_x=\phi_{j,z}\quad(j=1,2),\qquad p_1=p_2.
$$

Disturbance velocities decay as $z\to\pm\infty$. The equilibrium pressures are $p_*-\rho_jgz$.

Linearize at the resting flat interface. The equations become $\Delta\phi_j=0$, $\zeta_t=\phi_{j,z}$ on $z=0$, and

$$
\rho_1(\phi_{1,t}+g\zeta)=\rho_2(\phi_{2,t}+g\zeta).
$$

For $k>0$, write $\zeta=\eta e^{i(kx-\omega t)}$. Decay selects $\phi_1=A_1e^{-kz}e^{i(kx-\omega t)}$ above and $\phi_2=A_2e^{kz}e^{i(kx-\omega t)}$ below. The kinematic conditions give $A_1=i\omega\eta/k$ and $A_2=-i\omega\eta/k$. Substituting into the dynamic condition gives

$$
\rho_1(\omega^2/k+g)\eta=\rho_2(-\omega^2/k+g)\eta,
\qquad \boxed{\omega^2=\frac{\rho_2-\rho_1}{\rho_2+\rho_1}gk.}
$$

For a signed wave number replace $k$ by $|k|$. A heavier lower fluid gives stable [interfacial gravity waves](../../../gravity-wave.md#interfacial-gravity-wave); a heavier upper fluid gives $\omega^2<0$ and [Rayleigh-Taylor instability](../../../continuum-mechanics.md#rayleigh-taylor-instability). The density ordering is not silently assumed positive in the derivation.

## 19D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="19d/i">i</h3>

↑ **Parent:** [19D](#19d)

<h4 id="19d/i/solution">Solution</h4>

↑ **Parent:** [I](#19d/i)

Assume $S_{xx}=\sum_i x_i^2>0$, which is necessary to identify the slope in [linear regression through the origin](../../../statistical-modelling.md#linear-regression-through-the-origin). The joint normal likelihood has logarithm, apart from a constant,

$$
\ell(\beta,\sigma^2)=-\frac n2\log\sigma^2-\frac1{2\sigma^2}\sum_i(Y_i-\beta x_i)^2.
$$

Complete the square in $\beta$. With $\widehat\beta=\sum_i x_iY_i/S_{xx}$ and $\mathrm{RSS}=\sum_i(Y_i-\widehat\beta x_i)^2$,

$$
\sum_i(Y_i-\beta x_i)^2=\mathrm{RSS}+S_{xx}(\beta-\widehat\beta)^2.
$$

The [maximum likelihood estimation](../../../statistical-modelling.md#maximum-likelihood-estimation) therefore first minimizes at $\widehat\beta$; differentiating in $\sigma^2$ then maximizes at

$$
\boxed{\widehat\beta=\frac{\sum_i x_iY_i}{S_{xx}},\qquad \widehat\sigma^2=\frac{\mathrm{RSS}}n.}
$$

This is a genuine finite maximum when $\mathrm{RSS}>0$. If all $x_i=0$, the slope is unidentifiable. If $\mathrm{RSS}=0$, the likelihood is unbounded as $\sigma^2\downarrow0$, so no positive-variance maximum exists. For nonzero design and $n\geq2$, zero residual has probability zero under the stated positive-variance model.

<h3 id="19d/ii">ii</h3>

↑ **Parent:** [19D](#19d)

<h4 id="19d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#19d/ii)

The [least-squares estimator](../../../statistical-modelling.md#ordinary-least-squares-estimators) satisfies

$$
\widehat\beta=\beta+\frac{\sum_i x_i\epsilon_i}{S_{xx}}.
$$

A linear combination of independent [normal random variables](../../../probability-theory.md#gaussian-random-variable) is normal; its mean is $\beta$ and its variance is $\sigma^2\sum_i x_i^2/S_{xx}^2$. Hence

$$
\boxed{\widehat\beta\sim N\left(\beta,\frac{\sigma^2}{S_{xx}}\right).}
$$

<h3 id="19d/iii">iii</h3>

↑ **Parent:** [19D](#19d)

<h4 id="19d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#19d/iii)

Let $x$ and $\epsilon$ denote the design and error vectors, and put $P=xx^T/S_{xx}$. The residual vector is $r=(I-P)\epsilon$, while $\widehat\beta-\beta=x^T\epsilon/S_{xx}$. Since $(I-P)x=0$,

$$
\operatorname{Cov}(r,\widehat\beta)=\frac{\sigma^2}{S_{xx}}(I-P)x=0.
$$

These are jointly Gaussian linear functions of $\epsilon$, so the entire residual vector is independent of $\widehat\beta$, not merely uncorrelated with it. Choose an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) whose first vector is $x/\sqrt{S_{xx}}$. In that basis $\epsilon/\sigma$ has independent standard normal coordinates, and the residual keeps exactly the remaining $n-1$ coordinates. Therefore

$$
\boxed{\widehat\beta\ \perp\!\!\!\perp\ \widehat\sigma^2,\qquad
\frac{n\widehat\sigma^2}{\sigma^2}=\frac{\mathrm{RSS}}{\sigma^2}\sim\chi^2_{n-1}.}
$$

Together with part (ii), this specifies the joint distribution as the product of the slope's normal law and the scaled [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution). In particular $E\widehat\sigma^2=(n-1)\sigma^2/n$: the variance maximum-likelihood estimator is biased downward.

<h3 id="19d/iv">iv</h3>

↑ **Parent:** [19D](#19d)

<h4 id="19d/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#19d/iv)

For $n\geq2$, use the unbiased residual variance $s^2=\mathrm{RSS}/(n-1)=n\widehat\sigma^2/(n-1)$. Under the null hypothesis, $(\widehat\beta-\beta_0)\sqrt{S_{xx}}/\sigma$ is standard normal and independent of $\mathrm{RSS}/\sigma^2\sim\chi^2_{n-1}$. Hence

$$
\boxed{T=\frac{(\widehat\beta-\beta_0)\sqrt{S_{xx}}}{s}\sim t_{n-1}\quad\text{under }H_0.}
$$

For a chosen significance level $\alpha$, reject the null in favor of the two-sided alternative exactly when $|T|>t_{n-1,1-\alpha/2}$, the stated upper quantile of the [Student t-distribution](../../../continuous-probability-distribution.md#student-s-t-distribution). The exact two-sided p-value is $2P(t_{n-1}\geq|T_{\rm obs}|)$. This [hypothesis test](../../../statistical-modelling.md#statistical-hypothesis-test) does not substitute the biased MLE for $s^2$ without correcting its factor and does not use a normal critical value when variance is unknown.

## 20D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="20d/solution">Solution</h3>

↑ **Parent:** [20D](#20d)

Start with a feasible [network flow](../../../graph-theory.md#flow), meaning capacity bounds and flow conservation at every vertex other than source and sink. Its [residual network](../../../graph-theory.md#residual-network) has, for an arc with capacity $c$ and current flow $f$, a forward residual capacity $c-f$ and a reverse residual capacity $f$. A reverse arc allows earlier flow to be cancelled. The [Ford-Fulkerson algorithm](../../../graph-theory.md#ford-fulkerson-algorithm) repeatedly finds a residual source-to-sink [augmenting path](../../../graph-theory.md#augmenting-path), takes the smallest residual capacity $\delta$ on it, and augments by $\delta$, increasing forward flows and decreasing reverse flows as appropriate. Feasibility is preserved and the total flow increases by $\delta$.

For rational capacities and initial flows, choose one common denominator $D$ and scale all quantities by $D$. Every residual capacity and augmentation is then integral; each augmentation increases the integer-valued flow by at least one. The flow value is bounded by the finite sum of capacities out of the source, so termination occurs after finitely many augmentations. When no residual path remains, let $U$ be the vertices reachable from the source. Every original arc leaving $U$ is saturated and every original arc entering $U$ carries zero flow, or its reverse arc would extend reachability. Conservation then makes the flow value equal to the capacity of the cut $(U,U^c)$. Every feasible flow is bounded by that cut capacity. Thus **the terminating flow is globally optimal**, proving the needed [max-flow min-cut theorem](../../../graph-theory.md#max-flow-min-cut-theorem) conclusion.

For the given directed graph, begin at zero. One valid sequence of augmentations is:

| Residual path | Added flow | Cumulative value |
| --- | --- | --- |
| S–A–B–T | 6 | 6 |
| S–D–C–T | 10 | 16 |
| S–A–B–H–J–T | 3 | 19 |
| S–A–G–H–J–T | 3 | 22 |
| S–F–G–H–J–T | 2 | 24 |
| S–F–E–K–C–T | 5 | 29 |
| S–F–E–K–J–T | 1 | 30 |

Each amount is the current path bottleneck. The resulting nonzero arc flows are

$$
\begin{gathered}
SA=12,\ SF=8,\ SD=10,\ AB=9,\ AG=3,\ FG=2,\ FE=6,\ DC=10,\\
EK=6,\ GH=5,\ BH=3,\ BT=6,\ HJ=8,\ KJ=1,\ KC=5,\ JT=9,\ CT=15;
\end{gathered}
$$

every other arc has zero flow. Directly summing incoming and outgoing flows verifies conservation, and every displayed flow is at most its printed capacity. A minimum-cut certificate is

$$
U=\{S,A,B,E,F,G,H\},\qquad U^c=\{D,K,J,C,T\}.
$$

Its only outgoing arcs are $SD$, $EK$, $HJ$ and $BT$, with capacities $10,6,8,6$. Therefore

$$
\boxed{\text{maximum flow}=10+6+8+6=30.}
$$

The matching feasible flow and cut prove optimality independently of the augmenting-path choices.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
