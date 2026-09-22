<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a [prime](../../../../../prime-number.md) $p$, the [divisor sum](../../../../../divisor-sum.md) defining the real weight is $\phi(0)-\phi(\log p/\log X)$. If $p>X^{1/3}$, the second term vanishes and the first is one. Thus **$F(p)=1$**, while $F(n)\geq0$ for every integer because $\phi$ is real and the sum is squared.

Put $h(x)=e^x\phi(x)$. With the [Fourier transform](../../../../../fourier-transform.md) convention in the question, [Fourier inversion](../../../../../fourier-inversion-theorem.md) gives

$$
\psi(t)=\frac1{2\pi}\int_{\mathbb R}h(x)e^{ixt}\,dx.
$$

The function $h$ is [smooth](../../../../../smooth-function.md) and has [compact support](../../../../../compact-support.md). Using [integration by parts](../../../../../integration-by-parts.md) $k$ times, with zero endpoint terms, proves

$$
|\psi(t)|\leq\frac{\|h^{(k)}\|_1}{2\pi|t|^k}.
$$

Choose an integer $k\geq A$ to obtain **$|\psi(t)|\ll_A|t|^{-A}$ for $|t|\geq1$**. In particular every polynomially weighted absolute integral of $\psi$ is finite.

For the double integral, use

$$
\frac1{2+i(t+t')}=\int_0^\infty e^{-(2+i(t+t'))u}\,du,
\qquad
\phi(u)=\int_{\mathbb R}\psi(t)e^{-(1+it)u}\,dt.
$$

Differentiating the second formula gives $\int\psi(t)(1+it)e^{-(1+it)u}\,dt=-\phi'(u)$. [absolute convergence](../../../../../absolute-convergence.md) from the rapid decay permits [Fubini's theorem](../../../../../fubini-s-theorem.md). The [derivative energy constant for a smooth sieve cutoff](../../../../../derivative-energy-constant-for-a-smooth-sieve-cutoff.md) is therefore

$$
\boxed{\iint\psi(t)\psi(t')\frac{(1+it)(1+it')}{2+i(t+t')}\,dt\,dt'
=c_\phi:=\int_0^\infty\phi'(u)^2\,du
=\int_0^{1/3}\phi'(u)^2\,du.}
$$

There is no [complex conjugate](../../../../../complex-conjugate.md) in this integral: the two factors both become $-\phi'(u)$, which is real. The constant is positive; in fact the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) applied to $\phi(1/3)-\phi(0)=-1$ gives $c_\phi\geq3$.

Here is the basic structure of the [smooth divisor-square sieve asymptotic](../../../../../smooth-divisor-square-sieve-asymptotic.md), with enough uniform estimates to specify the error. Write $L=\log X$ and $R=X^{1/3}$. Expand the square and count multiples of the [least common multiple](../../../../../least-common-multiple.md) $[d,e]$ in an arbitrary interval $I$ of length $X$:

$$
\sum_{n\in I}F(n)=X S_X+O_\phi(R^2),
\qquad
S_X=\sum_{d,e\geq1}\frac{\mu(d)\mu(e)}{[d,e]}\phi\left(\frac{\log d}L\right)\phi\left(\frac{\log e}L\right).
$$

The sum is effectively restricted to $d,e<R$. Each count is $X/[d,e]+O(1)$, independent of the interval's position, so the total error is $O_\phi(X^{2/3})$.

The [Fourier representation of a smooth Selberg weight](../../../../../fourier-representation-of-a-smooth-selberg-weight.md) reads

$$
\phi\left(\frac{\log d}L\right)=\int_{\mathbb R}\psi(t)d^{-z}\,dt,
\qquad z=\frac{1+it}L.
$$

Hence, with $z'=(1+it')/L$,

$$
S_X=\iint\psi(t)\psi(t')E(z,z')\,dt\,dt',
\qquad
E(z,z')=\prod_p(1-p^{-1-z}-p^{-1-z'}+p^{-1-z-z'}).
$$

The four local terms correspond to the [prime](../../../../../prime-number.md) dividing neither [divisor](../../../../../divisor.md), only the first, only the second, or both. This is the [Euler product for a smoothed divisor-square correlation](../../../../../euler-product-for-a-smoothed-divisor-square-correlation.md). Factor it as

$$
E(z,z')=\frac{\zeta(1+z+z')}{\zeta(1+z)\zeta(1+z')}H(z,z'),
$$

where

$$
H(z,z')=\prod_p\frac{(1-a_p-b_p+c_p)(1-c_p)}{(1-a_p)(1-b_p)},
\quad a_p=p^{-1-z},\ b_p=p^{-1-z'},\ c_p=p^{-1-z-z'}.
$$

The local factors of $H$ are $1+O(p^{-2+4\eta})$ when $|\operatorname{Re}z|,|\operatorname{Re}z'|\leq\eta$ for small fixed $\eta<1/4$. Thus $H$ is a [holomorphic function](../../../../../holomorphic-function.md) near $(0,0)$, and evaluating each local factor at zero gives exactly one. Consequently $H(0,0)=1$ and $H(z,z')=1+O(|z|+|z'|)$ there.

The pole expansion $\zeta(1+w)=w^{-1}+O(1)$ now yields

$$
E(z,z')=\frac1L\frac{(1+it)(1+it')}{2+i(t+t')}
\left(1+O\left(\frac{2+|t|+|t'|}L\right)\right)
$$

when $|t|,|t'|\leq L^{1/4}$. Integrating the error against the rapidly decreasing transforms gives $O_\phi(L^{-2})$. The complementary tails are harmless uniformly: absolute values in the original [divisor](../../../../../divisor.md) series give

$$
|E((1+it)/L,(1+it')/L)|
\leq\prod_p(1+2p^{-1-1/L}+p^{-1-2/L})
\leq\zeta(1+1/L)^3\ll L^3.
$$

Any prescribed power decay of $\int_{|t|>L^{1/4}}|\psi(t)|\,dt$ is available, so these tails and the tails of the limiting kernel are $O_\phi(L^{-2})$ after choosing sufficiently many applications of [integration by parts](../../../../../integration-by-parts.md). The same absolute bound justifies the original exchanges of infinite sums and integrals. Using the evaluated double integral,

$$
S_X=\frac{c_\phi}L+O_\phi(L^{-2}).
$$

We conclude, uniformly over all interval locations,

$$
\boxed{\sum_{n\in I}F(n)=c_\phi\frac X{\log X}
+O_\phi\left(\frac X{\log^2X}+X^{2/3}\right)
\sim c_\phi\frac X{\log X}.}
$$

This proof does not assume that the interval starts near the origin.

Finally choose this one fixed [smooth](../../../../../smooth-function.md) cutoff. [primes](../../../../../prime-number.md) above $R$ in $(X_0,X_0+X]$ contribute one each to the nonnegative weight, and at most $R$ [primes](../../../../../prime-number.md) lie below $R$. Therefore

$$
\pi(X_0+X)-\pi(X_0)\leq\sum_{X_0<n\leq X_0+X}F(n)+R
\ll\frac X{\log X}
$$

for all sufficiently large $X$, uniformly in $X_0$. The bounded range $2\leq X\leq X_1$ follows by increasing the fixed constant and using the trivial interval bound $X+1$. Thus the [short-interval prime upper bound from a smooth divisor weight](../../../../../short-interval-prime-upper-bound-from-a-smooth-divisor-weight.md) is

$$
\boxed{\pi(X_0+X)-\pi(X_0)\ll\frac X{\log X}\qquad(X_0,X\geq2).}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
