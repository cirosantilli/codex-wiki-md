# Paper 23

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_23.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_23.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [i](#3/i)
  - [ii](#3/ii)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
    - [i](#5/d/i)
      - [Solution](#5/d/i/solution)
    - [ii](#5/d/ii)
      - [Solution](#5/d/ii/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)

## 1

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [primitive Dirichlet character](../../../algebraic-number-theory.md#primitive-dirichlet-character) modulo $q$ is a [Dirichlet character](../../../algebraic-number-theory.md#dirichlet-character) which is not induced from a character of a proper divisor of $q$. To determine the inducing [primitive Dirichlet character](../../../algebraic-number-theory.md#primitive-dirichlet-character), use the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) to decompose

$$
(\mathbb Z/q\mathbb Z)^\times\cong\prod_{p^k\parallel q}(\mathbb Z/p^k\mathbb Z)^\times.
$$

On each factor choose the least exponent $c_p\in\{0,\ldots,k\}$ through whose reduction the restricted character factors. Exponent zero means the trivial unit group modulo one. Put $q_0=\prod_pp^{c_p}$ and define $\chi_0$ on the units modulo $q_0$ by these descended factors, extending by zero off the units. Every reduction of unit groups is [surjective](../../../algebra.md#surjective-function), so the descended character is unique. Its local exponents cannot be decreased, hence it is primitive. The original character is $\chi(n)=\chi_0(n)$ when $(n,q)=1$, and zero otherwise.

Any other inducing modulus must have exponent at least $c_p$ at every [prime](../../../number-theory.md#prime-number), by restriction to the corresponding local factor. Therefore $q_0$ is the unique minimal modulus, the [conductor of a Dirichlet character](../../../algebraic-number-theory.md#conductor-of-a-dirichlet-character), and $\chi_0$ is the unique [primitive Dirichlet character](../../../algebraic-number-theory.md#primitive-dirichlet-character) inducing $\chi$. The argument also explains why removing extra [prime](../../../number-theory.md#prime-number) factors can change values at [integers](../../../number-theory.md#integer) that were nonunits for $q$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use the unitary [discrete Fourier transform](../../../numerical-analysis.md#discrete-fourier-transform), with $e(x)=\exp(2\pi ix)$:

$$
\widehat f(a)=q^{-1/2}\sum_{n\bmod q}f(n)e(-an/q).
$$

For a unit $a$, substitute $m=an$ in the sum. The multiplicativity of the [Dirichlet character](../../../algebraic-number-theory.md#dirichlet-character) gives $\chi(a^{-1}m)=\overline{\chi(a)}\chi(m)$, hence

$$
\boxed{\widehat\chi(a)=\overline{\chi(a)}\widehat\chi(1).}
$$

The [complex conjugation](../../../complex-analysis.md#complex-conjugation) is present in the original PDF and lost in the converted TeX. It matters for nonreal characters.

Now let $q=p^k$ and let $\chi$ be primitive. Since it does not descend to $p^{k-1}$, there is a unit $u\equiv1\pmod{p^{k-1}}$ with $\chi(u)\ne1$. For $k=1$, reduction is to the unit group modulo one. If $p\mid a$, then $a(u-1)\equiv0\pmod q$, so multiplication of the summation variable by $u$ leaves its exponential factor unchanged. It follows that $\widehat\chi(a)=\chi(u)\widehat\chi(a)$, and therefore $\widehat\chi(a)=0$. Also $\chi(a)=0$. This proves the formula at every nonunit as well as every unit, including $a=0$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For a [primitive Dirichlet character](../../../algebraic-number-theory.md#primitive-dirichlet-character) the previous formula gives $|\widehat\chi(a)|=|\chi(a)|\,|\widehat\chi(1)|$. The [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem) for the unitary finite transform yields

$$
\varphi(q)=\sum_{n\bmod q}|\chi(n)|^2
=\sum_{a\bmod q}|\widehat\chi(a)|^2
=\varphi(q)|\widehat\chi(1)|^2.
$$

Thus $|\widehat\chi(1)|=1$, the normalized [Gauss sum of a Dirichlet character](../../../algebraic-number-theory.md#gauss-sum-of-a-dirichlet-character) magnitude.

For an imprimitive character modulo $p^k$ with $k\ge2$, its values on residues are periodic modulo $p^{k-1}$: descent preserves the values on units, and divisibility by $p$ is unchanged by that shift. Splitting the sum into these [residue classes](../../../number-theory.md#residue-class) gives a factor $\sum_{j=0}^{p-1}e(-j/p)=0$. Hence $\widehat\chi(1)=0$. If $k=1$, the only imprimitive character is principal, and its Gauss sum is $\sum_{n=1}^{p-1}e(-n/p)=-1$, giving $|\widehat\chi(1)|=p^{-1/2}$. All cases satisfy the required bound.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Every [nonprincipal Dirichlet character](../../../algebraic-number-theory.md#nonprincipal-dirichlet-character) modulo the [prime](../../../number-theory.md#prime-number) $q$ is primitive, so its finite [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) have modulus one off zero; the coefficient at zero is zero by [character orthogonality](../../../representation-theory.md#character-orthogonality). [Fourier inversion theorem](../../../fourier-analysis.md#fourier-inversion-theorem) gives

$$
\sum_{M<n\le M+N}\chi(n)
=q^{-1/2}\sum_{a=1}^{q-1}\widehat\chi(a)\sum_{M<n\le M+N}e(an/q).
$$

The finite [geometric series](../../../real-analysis.md#geometric-series) gives

$$
\left|\sum_{M<n\le M+N}e(an/q)\right|
\le\frac{2}{|1-e(a/q)|}\le C\|a/q\|_{\mathbb R/\mathbb Z}^{-1}.
$$

The printed hint omits $n$ from the exponential; its literal constant summand would not obey the bound for arbitrary $N$. The geometric-series calculation proves the needed estimate independently. Pairing $a$ with $q-a$ gives

$$
\left|\sum_{M<n\le M+N}\chi(n)\right|
\le C\sqrt q\,2\sum_{a=1}^{(q-1)/2}\frac1a
\ll\sqrt q\log q.
$$

The last sum is a [harmonic number](../../../analytic-number-theory.md#harmonic-number). This proves the [Pólya–Vinogradov inequality](../../../analytic-number-theory.md#polya-vinogradov-inequality) uniformly in $M$ and $N$; complete blocks of length $q$ also vanish by [Orthogonality of Dirichlet characters](../../../algebraic-number-theory.md#orthogonality-of-dirichlet-characters).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Let $\chi$ be the quadratic character, equivalently the [Legendre symbol](../../../number-theory.md#legendre-symbol). Zero is included among the square [residue classes](../../../number-theory.md#residue-class). For every [integer](../../../number-theory.md#integer) $n$ its square-class indicator is

$$
1_{\{n\bmod q\text{ is a square}\}}=\frac{1+\chi(n)+1_{q\mid n}}2.
$$

For a nonzero [quadratic residue](../../../number-theory.md#quadratic-residue) the right side is one, for a nonresidue it is zero, and for a multiple of $q$ it is one. Summing over the interval, the character contribution is $O(\sqrt q\log q)$ by the previous part, while the number of multiples of $q$ is $N/q+O(1)$. Thus the required count is

$$
\boxed{\frac{N(q+1)}{2q}+O(\sqrt q\log q).}
$$

This counts the [integers](../../../number-theory.md#integer) in the interval whose [residue classes](../../../number-theory.md#residue-class) are squares. When the interval exceeds one period, repeated appearances are counted; the displayed main term could not describe a count of distinct [residue classes](../../../number-theory.md#residue-class) for arbitrary $N$.

## 2

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

An [even Dirichlet character](../../../algebraic-number-theory.md#even-dirichlet-character) satisfies $\chi(-1)=1$, while an [odd Dirichlet character](../../../algebraic-number-theory.md#odd-dirichlet-character) satisfies $\chi(-1)=-1$. Write $a=0$ or $1$ for its [character parity](../../../algebraic-number-theory.md#character-parity) and, for $x>0$, define the [Dirichlet character theta function](../../../algebraic-number-theory.md#dirichlet-character-theta-function)

$$
\theta_\chi(x)=\sum_{n\in\mathbb Z}n^a\chi(n)e^{-\pi n^2x/q}.
$$

For a [primitive Dirichlet character](../../../algebraic-number-theory.md#primitive-dirichlet-character) whose [conductor of a Dirichlet character](../../../algebraic-number-theory.md#conductor-of-a-dirichlet-character) is $q>1$, the term at zero is zero. Put $\tau(\chi)=\sum_{r\bmod q}\chi(r)e(r/q)$, using the positive exponential, and $\varepsilon_\chi=\tau(\chi)/(i^a\sqrt q)$. The primitive [Gauss sum of a Dirichlet character](../../../algebraic-number-theory.md#gauss-sum-of-a-dirichlet-character) has magnitude $\sqrt q$, so $|\varepsilon_\chi|=1$. The theta transformation is

$$
\boxed{\theta_\chi(x)=\varepsilon_\chi x^{-a-1/2}\theta_{\overline\chi}(1/x).}
$$

Thus the powers are $x^{-1/2}$ in the even case and $x^{-3/2}$ in the odd case; the odd root number contains $1/i$. The conjugate character is necessary for a nonreal character. These formulas also follow by applying [Poisson summation](../../../fourier-analysis.md#poisson-summation-formula) to the [Gaussian function](../../../calculus.md#gaussian-function) on each [residue class](../../../number-theory.md#residue-class), and to its derivative for odd parity. For the primitive [principal Dirichlet character](../../../algebraic-number-theory.md#principal-dirichlet-character) whose [conductor of a Dirichlet character](../../../algebraic-number-theory.md#conductor-of-a-dirichlet-character) is one, use the ordinary [Jacobi theta function](../../../modular-function.md#jacobi-theta-function) with constant term one; its transformation has root number one.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [completed Dirichlet L-function](../../../algebraic-number-theory.md#completed-dirichlet-l-function) is

$$
\Lambda(s,\chi)=\left(\frac q\pi\right)^{(s+a)/2}\Gamma\left(\frac{s+a}{2}\right)L(s,\chi).
$$

For nonprincipal [primitive Dirichlet characters](../../../algebraic-number-theory.md#primitive-dirichlet-character), termwise [Mellin transformation](../../../analysis.md#mellin-transform) initially in $\Re s>1$ gives

$$
\Lambda(s,\chi)=\frac12\int_0^\infty\theta_\chi(x)x^{(s+a)/2}\,\frac{dx}{x}.
$$

The [Dirichlet character theta function](../../../algebraic-number-theory.md#dirichlet-character-theta-function) decays exponentially at infinity; its transformation makes it decay faster than any power at zero. Hence the integral is entire in $s$. For even parity, substitute $x=1/y$ and the theta transformation to obtain

$$
\boxed{\Lambda(s,\chi)=\varepsilon_\chi\Lambda(1-s,\overline\chi).}
$$

The same calculation with the extra $x^{-1}$ power gives the odd [functional equation](../../../analysis.md#functional-equation) with its corresponding root number.

The [gamma function](../../../complex-analysis.md#gamma-function) has no zeros and has [simple poles](../../../isolated-singularity.md#simple-pole) at nonpositive [integers](../../../number-theory.md#integer). Thus the nontrivial zeros of $L$ and $\Lambda$ coincide with multiplicities. The [trivial zeros of a Dirichlet L-function](../../../algebraic-number-theory.md#trivial-zero-of-a-dirichlet-l-function) are $0,-2,-4,\ldots$ for a nonprincipal even character, and $-1,-3,-5,\ldots$ for an odd character. They cancel the gamma [poles](../../../isolated-singularity.md#pole) and are not zeros of $\Lambda$: the [functional equation](../../../analysis.md#functional-equation) takes these points to the zero-free right-hand region, including the standard [nonvanishing of nonprincipal Dirichlet L-functions at one](../../../analytic-number-theory.md#nonvanishing-of-a-nonprincipal-dirichlet-l-function-at-one) at the even endpoint. The canceled zeros are simple.

The principal [primitive Dirichlet character](../../../algebraic-number-theory.md#primitive-dirichlet-character) has [conductor of a Dirichlet character](../../../algebraic-number-theory.md#conductor-of-a-dirichlet-character) equal to one and $L=\zeta$. In that case $\Lambda=\pi^{-s/2}\Gamma(s/2)\zeta(s)$ is [meromorphic](../../../isolated-singularity.md#meromorphic-function) with [poles](../../../isolated-singularity.md#pole) at zero and one. Its canceled trivial zeros begin at $-2$, while $\zeta(0)=-1/2$ is not zero. Multiplication by $s(s-1)/2$ produces the entire [Riemann xi function](../../../analytic-number-theory.md#riemann-xi-function) used below.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $q_0$ be the [conductor of a Dirichlet character](../../../algebraic-number-theory.md#conductor-of-a-dirichlet-character) and $\chi_0$ the inducing primitive even character. Removing the Euler factors absent from $L(s,\chi)$ gives the [imprimitive Dirichlet L-function Euler correction](../../../algebraic-number-theory.md#imprimitive-dirichlet-l-function-euler-correction)

$$
L(s,\chi)=P(s)L(s,\chi_0),\qquad
P(s)=\prod_{\substack{p\mid q\\p\nmid q_0}}(1-\chi_0(p)p^{-s}).
$$

The primitive [functional equation](../../../analysis.md#functional-equation) therefore gives

$$
L(s,\chi)=\varepsilon_{\chi_0}\left(\frac{q_0}{\pi}\right)^{1/2-s}
\frac{\Gamma((1-s)/2)}{\Gamma(s/2)}P(s)L(1-s,\overline\chi_0).
$$

Equivalently, replace the final primitive function by $L(1-s,\overline\chi)/P_{\overline\chi}(1-s)$, interpreted as a [meromorphic](../../../isolated-singularity.md#meromorphic-function) identity with removable values handled by continuation. It is the [conductor of a Dirichlet character](../../../algebraic-number-theory.md#conductor-of-a-dirichlet-character) $q_0$, rather than the possibly inflated modulus $q$, that enters the gamma factor and root number. The [complex conjugation](../../../complex-analysis.md#complex-conjugation) bar in the original PDF is lost in the converted TeX.

The zeros are those of $L(s,\chi_0)$ together with the zeros of the finite [Euler product](../../../analytic-number-theory.md#euler-product), and multiplicities add. Since $|\chi_0(p)|=1$ at each extra [prime](../../../number-theory.md#prime-number), an extra factor vanishes at the imaginary points determined by

$$
p^{-s}=\overline{\chi_0(p)}.
$$

Each extra [prime](../../../number-theory.md#prime-number) creates infinitely many such points. Its nonzero-imaginary points are not zeros of the primitive function: the [functional equation](../../../analysis.md#functional-equation) and [nonvanishing of Dirichlet L-functions on the line one](../../../algebraic-number-theory.md#nonvanishing-of-dirichlet-l-functions-on-the-line-one) exclude them. Thus the zero sets are identical precisely when every [prime](../../../number-theory.md#prime-number) dividing $q$ already divides $q_0$, making $P=1$. Increasing prime-power exponents alone can make a character imprimitive without changing its L-function. If $q_0=1$, the primitive function is zeta; the same Euler correction applies, with its [pole](../../../isolated-singularity.md#pole) at one retained.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For a [nonprincipal Dirichlet character](../../../algebraic-number-theory.md#nonprincipal-dirichlet-character), complete periods sum to zero, so its partial sums are bounded by $q$. [Partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) at $X=q(1+t)$ yields

$$
L(1-it,\overline\chi)=\sum_{n\le X}\frac{\overline\chi(n)}{n^{1-it}}+O\left(\frac{q(1+t)}X\right).
$$

The head is bounded by $1+\log X$, hence $|L(1-it,\overline\chi)|\ll\log(q+t)$. The completed [functional equation](../../../analysis.md#functional-equation) gives

$$
|L(it,\chi)|=\left(\frac q\pi\right)^{1/2}
\left|\frac{\Gamma((1-it)/2)}{\Gamma(it/2)}\right|,|L(1-it,\overline\chi)|.
$$

The stated gamma bounds make the ratio $O(t^{1/2})$: their exponential factors cancel, and their powers differ by $1/2$. Apply them directly for $t\ge4$; the compact interval $2\le t\le4$ is absorbed into the constant. Therefore

$$
\boxed{|L(it,\chi)|\ll\sqrt{qt}\,\log(q+t).}
$$

For the conductor-one principal case, Euler summation for zeta at $1-it$, truncated at $X=t^2$, gives a harmonic-size head, a [pole](../../../isolated-singularity.md#pole) term of size $1/t$, and remainder $O((1+t)/X)$. It gives the same $O(\log t)$ bound before applying the zeta [functional equation](../../../analysis.md#functional-equation).

## 3

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Riemann xi function](../../../analytic-number-theory.md#riemann-xi-function) is the [entire function](../../../complex-analysis.md#entire-function)

$$
\xi(s)=\frac12s(s-1)\pi^{-s/2}\Gamma(s/2)\zeta(s),\qquad \xi(0)=\xi(1)=\frac12,
$$

with $\xi(s)=\xi(1-s)$. Its [Hadamard factorization](../../../complex-analysis.md#hadamard-factorization-theorem) is

$$
\xi(s)=\frac12e^{Bs}\prod_{\rho}\left(1-\frac{s}{\rho}\right)e^{s/\rho},
\qquad B=\frac{\xi'(0)}{\xi(0)},
$$

where the [Nontrivial zeros of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) are repeated by multiplicity and the factors are canonical genus-one factors.

Here is the growth estimate needed for the [Jensen zero-count bound](../../../complex-analysis.md#jensen-zero-count-bound). For $|s|\le2T$, functional symmetry reduces to $\Re s\ge1/2$. Euler summation truncated at $T^2$ bounds $(s-1)\zeta(s)$ by a fixed power of $T$, uniformly in that region; the multiplication cancels the [pole](../../../isolated-singularity.md#pole) at one. The logarithmic gamma estimate bounds $\log|\Gamma(s/2)|$ by $O(T\log T)$, including the bounded small-$s$ part separately. The remaining elementary factors obey the same bound. Thus

$$
\max_{|s|\le2T}\log|\xi(s)|\le C T\log T.
$$

For a zero with $|\rho|\le T$, its contribution in [Jensen's formula](../../../complex-analysis.md#jensen-s-formula) on radius $2T$ is at least $\log2$. Consequently

$$
n_\xi(T)\log2\le\frac1{2\pi}\int_0^{2\pi}\log|\xi(2Te^{i\theta})|\,d\theta-\log|\xi(0)|
\ll T\log T.
$$

If a zero lies on the integration circle, use nearby radii and [continuity](../../../calculus.md#continuous-function) of the zero-count estimate. Hence $n_\xi(T)=O(T\log T)$ for $T>2$. The growth also gives order at most one and justifies the stated [Hadamard factorization](../../../complex-analysis.md#hadamard-factorization-theorem); the zero-count bound gives convergence of its genus-one factors.

The printed logarithmic Stirling hint drops the term $-\tfrac12\log z$. The correct expansion is $(z-\tfrac12)\log z-z+\tfrac12\log(2\pi)+O(|z|^{-1})$ in a fixed sector. Its consequence $\log|\Gamma(z)|=O(|z|\log(2+|z|))$ is all that the argument needs.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $s=\sigma+it$ fixed, with $\xi(s)\ne0$. The zeros satisfy $0<\beta<1$. For $|\gamma|>2(|t|+1)$,

$$
\left|\frac{\sigma-\beta}{(\sigma-\beta)^2+(t-\gamma)^2}\right|
\le\frac{4(|\sigma|+1)}{\gamma^2}.
$$

The previous bound gives at most $O(2^j j)$ zeros in each dyadic ordinate band $2^j\le|\gamma|<2^{j+1}$, so its total majorant is $O(j2^{-j})$. That series converges. There are only finitely many zeros in the remaining bounded bands, and none has the forbidden denominator zero at the specified nonzero point of $\xi$. Thus the real [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) sum converges absolutely. This proves the [absolute convergence of the real xi logarithmic derivative](../../../analytic-number-theory.md#absolute-convergence-of-the-real-xi-logarithmic-derivative) without claiming [absolute convergence](../../../real-analysis.md#absolute-convergence) of the unpaired complex sums of $1/(s-\rho)$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Evaluate the supplied real [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) at $2+it$. Since $1<2-\beta<2$, its positive summand is bounded above and below by constant multiples of $(1+|t-\gamma|^2)^{-1}$. On the other hand, differentiating the defining xi expression gives

$$
\frac{\xi'}{\xi}(s)=\frac1s+\frac1{s-1}-\frac12\log\pi
+\frac12\frac{\Gamma'}{\Gamma}(s/2)+\frac{\zeta'}{\zeta}(s).
$$

At real part two the last term is bounded by the [absolutely convergent](../../../real-analysis.md#absolute-convergence) series $\sum\Lambda(n)n^{-2}$; the gamma [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) is $O(\log t)$. Therefore

$$
\boxed{\sum_\rho\frac1{1+|t-\gamma|^2}=O(\log t).}
$$

For $\gamma\in[T,T+1]$, use $t=T$: each term in the displayed sum is at least $1/2$. Hence the number of zeros in that unit ordinate interval, counted with multiplicities, is $O(\log T)$. These are the [local zeta zero-count bound](../../../analytic-number-theory.md#local-zero-count-for-the-riemann-zeta-function) and the corresponding smoothed bound.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Under the [Riemann hypothesis](../../../analytic-number-theory.md#riemann-hypothesis), every $\beta=1/2$, so for $\sigma>1/2$ the [absolutely convergent](../../../real-analysis.md#absolute-convergence) formula gives

$$
\frac{\partial}{\partial\sigma}\log|\xi(\sigma+it)|
=\sum_\rho\frac{\sigma-1/2}{(\sigma-1/2)^2+(t-\gamma)^2}>0.
$$

The zero set is nonempty: otherwise [Hadamard factorization](../../../complex-analysis.md#hadamard-factorization-theorem) would make $\xi$ an exponential of a linear [polynomial](../../../polynomial.md), and its functional symmetry would force it to be constant, contrary to gamma growth on the positive real axis. Thus the inequality is strict in the open right half-plane. [Continuity](../../../calculus.md#continuous-function) at $\sigma=1/2$, including at boundary zeros, proves the claimed increasing modulus on the closed half-line.

Conversely, suppose the modulus is nondecreasing for every fixed $t$. If a zero $\beta+i\gamma$ had $\beta>1/2$, then nonnegativity and monotonicity would force $|\xi(\sigma+i\gamma)|=0$ throughout $1/2\le\sigma\le\beta$. The [identity theorem](../../../complex-analysis.md#identity-theorem) would make $\xi$ identically zero, a contradiction. A zero left of the line reflects to one right of the line by the [functional equation](../../../analysis.md#functional-equation) and [complex conjugation](../../../complex-analysis.md#complex-conjugation) symmetry. Hence every zero lies on the [critical line](../../../analytic-number-theory.md#critical-line). This proves the [xi modulus criterion for the Riemann hypothesis](../../../analytic-number-theory.md#xi-modulus-criterion-for-the-riemann-hypothesis). The two following roman headers refer to supplied asymptotic assumptions, not further questions, and require no Solution sections.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

## 4

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For $\sigma>1$, the [Euler product positivity for L-function nonvanishing](../../../analytic-number-theory.md#euler-product-positivity-for-l-function-nonvanishing) gives

$$
\zeta(\sigma)^3|L(\sigma+it,\chi)|^4|L(\sigma+2it,\chi^2)|\ge1.
$$

Indeed the logarithm expands into terms proportional to $3+4\cos\theta+\cos2\theta=2(1+\cos\theta)^2\ge0$. At [primes](../../../number-theory.md#prime-number) dividing $q$, the character terms vanish and the remaining zeta term is positive. For a nonreal character, $\chi^2$ is nonprincipal, so its L-function is entire, even if imprimitive.

If $L(1+it,\chi)$ vanished to order $m\ge1$, the product would be $O((\sigma-1)^{4m-3})$ as $\sigma\downarrow1$: zeta has a [simple pole](../../../isolated-singularity.md#simple-pole), the last factor is bounded, and the middle factor has the asserted vanishing. The product would tend to zero, contradicting its lower bound one. This proves nonvanishing for every real $t$, including zero.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The Dirichlet-series coefficients are

$$
a_n=\sum_{d\mid n}\chi_D(d).
$$

They are multiplicative. At a [prime power](../../../number-theory.md#prime-power), their values are $k+1$ if $\chi_D(p)=1$, one for even $k$ and zero for odd $k$ if $\chi_D(p)=-1$, and one if $\chi_D(p)=0$. Thus every $a_n$ is nonnegative. In particular $a_{m^2}\ge1$. This is the [nonnegative zeta-times-real-L coefficients](../../../algebraic-number-theory.md#nonnegative-zeta-times-real-l-coefficients) identity. The same Euler expansion gives $-\zeta'/\zeta(\sigma)-L'/L(\sigma,\chi_D)\ge0$ for $\sigma>1$, with coefficients $\Lambda(n)(1+\chi_D(n))\ge0$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Put $D_0=|D|$. The reference to part (c) in the printed hint is a reference to the positive-coefficient function from part (b). For $\sigma>1$ close to one, the preceding positivity and the supplied partial-fraction expansion give

$$
0\le\frac1{\sigma-1}+C\log D_0-\sum_{\substack{\beta\text{ real}\text{near }1}}\frac1{\sigma-\beta}.
$$

All omitted zero terms have nonnegative real parts because their real parts are at most one. The $O(1)$ zeta-pole remainder is included in $C\log D_0$, increasing the absolute constant if needed; a nonprincipal primitive real [conductor of a Dirichlet character](../../../algebraic-number-theory.md#conductor-of-a-dirichlet-character) is at least three.

Suppose there were two real zeros, counted with multiplicity, with $\beta\ge1-c/\log D_0$. Set $\sigma=1+a/\log D_0$. Division by $\log D_0$ gives

$$
0\le\frac1a+C-\frac2{a+c}.
$$

Choose $C\ge1$, $a=1/(4C)$ and $c=a/4$. The right side is strictly negative. Thus

$$
\boxed{\text{at most one real zero, necessarily simple, in }[1-c/\log|D|,1].}
$$

This is the [uniqueness of a possible exceptional real Dirichlet zero](../../../analytic-number-theory.md#uniqueness-of-a-possible-exceptional-real-dirichlet-zero). It proves uniqueness, rather than existence of such a zero.

## 5

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The quotient-circle norm is $\|x\|_{\mathbb R/\mathbb Z}=\min_{m\in\mathbb Z}|\widetilde x-m|$, independent of the chosen lift $\widetilde x$. A finite set is $\delta$-well-spaced when every two distinct points satisfy $\|x_r-x_s\|\ge\delta$. This is separation in the [circle metric](../../../lie-theory.md#circle-metric), including the distance across the identified endpoints.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For the matrix $A_{r,n}=e(nx_r)$, [operator norm duality](../../../continuous-dual-space.md#operator-norm-duality) gives $\|A\|=\|A^*\|$. Thus the [analytic large sieve inequality](../../../analytic-number-theory.md#exponential-sum-large-sieve)

$$
\sum_r\left|\sum_{M<n\le M+N}a_ne(nx_r)\right|^2
\le C(N+\delta^{-1})\sum_n|a_n|^2
$$

is equivalent to the dual bound with the roles of $a_n$ and $b_r$ exchanged and the conjugate exponential. The absolute constant is independent of all the parameters.

Here is a [Fejér-kernel proof of the analytic large sieve](../../../analytic-number-theory.md#fejer-kernel-proof-of-the-analytic-large-sieve). Choose an [integer](../../../number-theory.md#integer) center $c$ of the summation interval and an [integer](../../../number-theory.md#integer) $m\asymp N+1$ large enough that the triangular weights $w_n=(1-|n-c|/m)_+$ are at least $1/2$ throughout it. Their Fourier kernel is $e(c\theta)F_m(\theta)$, with

$$
F_m(\theta)=\frac1m\left(\frac{\sin\pi m\theta}{\sin\pi\theta}\right)^2
\le C\min\left(m,\frac1{m\|\theta\|^2}\right),\qquad F_m(0)=m.
$$

For fixed $r$, spacing allows at most a bounded number of points at each successive distance $j\delta$. Splitting at $j\asymp1/(m\delta)$ gives the row bound

$$
\sum_s|F_m(x_r-x_s)|\le C(m+\delta^{-1}).
$$

In detail the near terms contribute at most $Cm/(m\delta)=C/\delta$, and the square-decay tail contributes $C/(m\delta^2)\sum_{j>1/(m\delta)}j^{-2}\le C/\delta$; when $m\delta\ge1$, the tail is bounded directly by $C/\delta$.

Expand the weighted dual square sum. Its matrix entries have the kernel just estimated. The symmetric row bound, or $2|b_rb_s|\le|b_r|^2+|b_s|^2$, bounds the [quadratic form](../../../linear-algebra.md#quadratic-form) by $C(m+\delta^{-1})\sum|b_r|^2$. The weights majorize half the desired interval, proving the dual inequality and hence the primal inequality. This supplies the sieve estimate with an absolute constant, including the technical interaction between close pairs and the kernel's decaying tail.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Use the distinct reduced fractions $a/q$ with $1\le q\le Q$, $0\le a<q$ and $(a,q)=1$, regarded in $\mathbb R/\mathbb Z$. The fraction zero appears as $0/1$; one is the same circle point and is not added a second time. For two distinct such points, the ordinary difference and its possible wrapped complement are nonzero [integer](../../../number-theory.md#integer) multiples of $1/(qq')$. Hence

$$
\boxed{\|a/q-a'/q'\|_{\mathbb R/\mathbb Z}\ge1/(qq')\ge Q^{-2}.}
$$

This proves the required separation of the [Farey fractions](../../../number-theory.md#farey-fraction).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

The standard primitive-character [multiplicative large sieve inequality](../../../analytic-number-theory.md#character-large-sieve) is

$$
\sum_{q\le Q}\frac q{\varphi(q)}\sum_{\chi\bmod q}^{*}
\left|\sum_{M<n\le M+N}a_n\chi(n)\right|^2
\le C(N+Q^2)\sum_n|a_n|^2,
$$

where the star restricts to [primitive Dirichlet characters](../../../algebraic-number-theory.md#primitive-dirichlet-character). This is the form used in analytic arguments for [Linnik's theorem](../../../analytic-number-theory.md#linnik-s-theorem). The prime-power Gauss identities extend to arbitrary primitive conductors by the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem). Thus the [primitive Dirichlet character](../../../algebraic-number-theory.md#primitive-dirichlet-character) sum is, up to a factor of modulus $q^{-1/2}$, the character-weighted sum of the additive values $A(a/q)=\sum_na_ne(an/q)$ over units $a$. [Orthogonality of Dirichlet characters](../../../algebraic-number-theory.md#orthogonality-of-dirichlet-characters), extending the primitive-character summation to all characters, gives

$$
\frac q{\varphi(q)}\sum_{\chi\bmod q}^{*}|\sum_na_n\chi(n)|^2
\le\sum_{(a,q)=1}|A(a/q)|^2.
$$

The additive sieve on the $Q^{-2}$-spaced Farey points proves the displayed bound.

For both prime-interval applications, use the following [large sieve upper bound for sifted intervals](../../../analytic-number-theory.md#large-sieve-upper-bound-for-sifted-intervals). Suppose $S$ is in an interval of length $H$ and avoids one residue modulo every [prime](../../../number-theory.md#prime-number) $p\le Q$ not dividing a fixed $q$. Then

$$
|S|\le\frac{C(H+Q^2)}{\mathcal L_q(Q)},\qquad
\mathcal L_q(Q)=\sum_{\substack{d\le Q\\(d,q)=1}}\frac{\mu^2(d)}{\varphi(d)}.
$$

To prove it, choose the forbidden [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) residue $r_d$ for each [squarefree](../../../number-theory.md#squarefree-integer) $d$. The [Ramanujan sum](../../../algebra.md#ramanujan-sum) $c_d(n-r_d)$ equals $\mu(d)$ on $S$, since $n-r_d$ is a unit modulo $d$. Therefore [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\sum_{(a,d)=1}\left|\sum_{n\in S}e(an/d)\right|^2\ge\frac{|S|^2}{\varphi(d)}.
$$

Indeed the linear combination with coefficients $e(-ar_d/d)$ has value $\mu(d)|S|$, and these coefficients have squared norm $\varphi(d)$. Sum over the allowed [squarefree](../../../number-theory.md#squarefree-integer) $d$, apply the additive large sieve, and cancel $|S|$; the empty set is immediate.

Finally $\mathcal L_1(Q)\ge c\log(2Q)$. [Squarefree integers](../../../number-theory.md#squarefree-integer) have a positive elementary lower density: the nonsquarefree [integers](../../../number-theory.md#integer) up to $X$ are covered by multiples of $k^2$, and $\sum_{k\ge2}k^{-2}\le3/4$. [Partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) turns this density into the [harmonic](../../../partial-differential-equation.md#harmonic-function) lower bound. Splitting each [squarefree](../../../number-theory.md#squarefree-integer) $d$ into its factors supported on [primes](../../../number-theory.md#prime-number) dividing $q$ and its coprime part gives

$$
\mathcal L_1(Q)\le\prod_{p\mid q}\left(1+\frac1{p-1}\right)\mathcal L_q(Q)
=\frac q{\varphi(q)}\mathcal L_q(Q).
$$

Consequently $\mathcal L_q(Q)\ge c\,\varphi(q)\log(2Q)/q$, uniformly in $q$ and $Q$.

<h4 id="5/d/i">i</h4>

↑ **Parent:** [D](#5/d)

<h5 id="5/d/i/solution">Solution</h5>

↑ **Parent:** [I](#5/d/i)

Take $S$ to be the [primes](../../../number-theory.md#prime-number) in the interval and $Q=\max(2,\lfloor\sqrt N\rfloor)$. Every such [prime](../../../number-theory.md#prime-number) exceeds $M>N\ge Q$ apart from harmless bounded small cases, so it avoids zero modulo each [prime](../../../number-theory.md#prime-number) up to $Q$. The sifted-interval bound with $H=N$ and $q=1$ gives

$$
\boxed{\pi(M+N)-\pi(M)\ll N/\log N.}
$$

Since $Q^2=O(N)$ and $\log(2Q)\asymp\log N$, the implied constant is absolute. The choice of strict or inclusive endpoint in the prime-counting convention changes at most two terms, absorbed by the bound for $N\ge2$.

<h4 id="5/d/ii">ii</h4>

↑ **Parent:** [D](#5/d)

<h5 id="5/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/d/ii)

Write the progression [integers](../../../number-theory.md#integer) as $n=a+qm$. Their $m$ values lie in an interval of length at most $N/q+1$. For every [prime](../../../number-theory.md#prime-number) $p\nmid q$, primality forbids the unique residue $m\equiv-aq^{-1}\pmod p$; [primes](../../../number-theory.md#prime-number) dividing $q$ impose no restriction because $(a,q)=1$.

Choose $Q=\max(2,\lfloor\sqrt{N/q}\rfloor)$. The selected [primes](../../../number-theory.md#prime-number) exceed $M>N$, hence exceed these sieving [primes](../../../number-theory.md#prime-number). The uniform coprime-denominator estimate just proved yields

$$
|S|\ll\frac{N/q+Q^2+1}{(\varphi(q)/q)\log(2Q)}
\ll\frac{N}{\varphi(q)\log(N/q)}.
$$

The assumption $N\ge q^{2+\delta}$ implies $\log(N/q)\ge\frac{1+\delta}{2+\delta}\log N\ge\frac12\log N$. Therefore

$$
\boxed{\pi(M+N;q,a)-\pi(M;q,a)\ll\frac{N}{\varphi(q)\log N}.}
$$

Endpoint and bounded small-parameter corrections are again absorbed. The proof supplies the more informative short-interval progression bound before using the given size hypothesis.

## 6

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

The [Riemann hypothesis](../../../analytic-number-theory.md#riemann-hypothesis) says that every [Nontrivial zero of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) of $\zeta$ has real part $1/2$. The [Lindelöf hypothesis](../../../analytic-number-theory.md#lindelof-hypothesis) says that, for every $\varepsilon>0$,

$$
|\zeta(1/2+it)|\ll_\varepsilon(1+|t|)^\varepsilon.
$$

The exponent may be arbitrarily small; the implied constant may depend on that exponent. The next part proves the implication from the first hypothesis to the second.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Assume [Riemann hypothesis](../../../analytic-number-theory.md#riemann-hypothesis). First fix $0<\delta<1/4$ and work on $\sigma_0=1/2+\delta$. We prove the [subpower zeta bound to the right of the critical line](../../../analytic-number-theory.md#subpower-zeta-bound-to-the-right-of-the-critical-line), then move back to the line by the [functional equation](../../../analysis.md#functional-equation) and [Phragmén–Lindelöf principle](../../../complex-analysis.md#phragmen-lindelof-principle).

Put $x=\log t$ for large positive $t$ and integrate the supplied smoothed [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) identity horizontally from $\sigma_0$ to two. There are no zeros on this path under [Riemann hypothesis](../../../analytic-number-theory.md#riemann-hypothesis), so the Euler-product logarithm at $2+it$ continues along it. Each prime-power term contributes at most $\Lambda(n)n^{-\sigma_0}/\log n\le n^{-\sigma_0}$, and the smoothing weights are at most one. Hence the integrated [prime](../../../number-theory.md#prime-number) terms are bounded by

$$
C_\delta\sum_{n\le x^2}n^{-\sigma_0}\ll_\delta x^{1-2\delta}=o(\log t).
$$

All zeros have $\rho=1/2+i\gamma$. The local zero-count estimate from Question 3, with its reflected version for negative ordinates, gives uniformly for $\sigma_0\le\sigma\le2$

$$
\sum_\rho\frac1{|\rho-\sigma-it|^2}\le C_\delta\log t.
$$

To see the uniformity, sum the $O(\log(2+|\gamma|))$ zeros in successive unit ordinate intervals against $(\delta^2+|t-\gamma|^2)^{-1}$; the distant dyadic tails are summable. The zero-term numerator has modulus at most $x^{-2\delta}+x^{-\delta}$. Its integrated contribution is therefore at most $C_\delta x^{-\delta}\log t/\log x=o(\log t)$. The integrated supplied remainder is $O(x^{-1-\delta}\log t/\log x)$, also $o(\log t)$. Since $\log\zeta(2+it)$ is bounded, we obtain

$$
|\log\zeta(1/2+\delta+it)|=o_\delta(\log t).
$$

Thus for every fixed $\delta>0$ and $\eta>0$, $|\zeta(1/2+\delta+it)|\ll_{\delta,\eta}t^\eta$. Negative $t$ follow by [complex conjugation](../../../complex-analysis.md#complex-conjugation).

The zeta [functional equation](../../../analysis.md#functional-equation) and the gamma ratio give $|\zeta(1/2-\delta+it)|\ll_{\delta,\eta}t^{\delta+\eta}$. Zeta is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) throughout this strip, since its [pole](../../../isolated-singularity.md#pole) at one is outside it, and Euler summation supplies [polynomial](../../../polynomial.md) vertical growth. The strip convexity conclusion of [Phragmén–Lindelöf principle](../../../complex-analysis.md#phragmen-lindelof-principle) therefore gives at the midpoint

$$
|\zeta(1/2+it)|\ll_{\delta,\eta}(1+|t|)^{\delta/2+\eta}.
$$

For a prescribed $\varepsilon>0$, choose $\delta$ and $\eta$ with $\delta/2+\eta<\varepsilon$; the bounded $t$ range is harmless. This proves

$$
\boxed{\text{Riemann hypothesis}\ \Longrightarrow\ \text{Lindelöf hypothesis}.}
$$

The explicit-formula estimate is deliberately first made a fixed distance to the right of the [critical line](../../../analytic-number-theory.md#critical-line). No divergent zero bound at $\sigma=1/2$ is used.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
