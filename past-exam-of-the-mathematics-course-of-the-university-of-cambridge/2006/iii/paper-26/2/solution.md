<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Half exponents in an odd-order [root of unity](../../../../../root-of-unity.md) group mean multiplication by the inverse of two modulo its order. This uniquely defines $\zeta_n^{a/2}$ inside $K_n$, and the definitions are compatible as $n$ varies. Put $d_a(z)=z^{-a/2}(1-z^a)$ on these roots. The [symmetric cyclotomic unit](../../../../../symmetric-cyclotomic-unit.md) is $c_n(a,b)=d_a(\zeta_n)/d_b(\zeta_n)$. Complex conjugation replaces each $d_a$ by $-d_a$, so the ratio is real. It is a global [unit](../../../../../unit-in-a-ring.md): choosing positive representatives for $a,b$ modulo $p^{n+1}$ gives geometric-series expressions for $(1-\zeta_n^a)/(1-\zeta_n)$ and its inverse, and similarly for $b$. The remaining factor is a [root of unity](../../../../../root-of-unity.md).

The conjugates of $\zeta_n$ over $K_{n-1}$ are $\xi\zeta_n$ with $\xi\in\mu_p$. Because $p\nmid a$, multiplication by $a$ permutes $\mu_p$, and

$$
N_{n,n-1}(1-\zeta_n^a)=\prod_{\xi\in\mu_p}(1-\xi^a\zeta_n^a)=1-\zeta_{n-1}^a.
$$

Also $\prod_{\xi\in\mu_p}\xi=1$ for odd $p$, so $N_{n,n-1}(\zeta_n)=\zeta_{n-1}$. Applying the compatible half power proves $N_{n,n-1}(d_a(\zeta_n))=d_a(\zeta_{n-1})$. Dividing the analogous identities for $a,b$ proves

$$
\boxed{N_{n,n-1}(c_n(a,b))=c_{n-1}(a,b)\qquad(n\ge1).}
$$

Embed the [fields](../../../../../field.md) into the p-adic cyclotomic tower. Its interpolating [Coleman power series](../../../../../coleman-power-series.md) is

$$
f_{a,b}(T)=(1+T)^{(b-a)/2}\frac{1-(1+T)^a}{1-(1+T)^b}\in\mathbb Z_p[[T]]^\times.
$$

Here $(b-a)/2\in\mathbb Z_p$, and binomial expansion defines the half power. Both numerator and denominator vanish to order one at $T=0$, with coefficients $-a$ and $-b$, so cancellation gives an integral [unit](../../../../../unit-in-a-ring.md) with $f_{a,b}(0)=a/b$. This applies also to negative integers $a,b$. Evaluation at $\zeta_n-1$ gives $c_n(a,b)$; the same root-product calculation shows $\mathcal N f_{a,b}=f_{a,b}$ for the [Coleman norm operator](../../../../../coleman-norm-operator.md).

For clarity, the normalization of the [higher logarithmic derivative](../../../../../cyclotomic-higher-logarithmic-derivative.md) is

$$
\delta_k(c)=\left.D^{k-1}\left(\frac{Df_c}{f_c}\right)\right|_{T=0},\qquad
D=(1+T)\frac{d}{dT},\qquad k\ge1.
$$

In the formal coordinate $T=e^z-1$, $D=d/dz$ and

$$
f_{a,b}(e^z-1)=\frac{e^{-az/2}-e^{az/2}}{e^{-bz/2}-e^{bz/2}}
=\frac{\sinh(az/2)}{\sinh(bz/2)}.
$$

Only the derivative of the logarithm is needed, so no choice of its constant term is involved. Differentiating gives the regular-at-zero expression

$$
\frac{d}{dz}\log f_{a,b}(e^z-1)
=\frac a2\coth\frac{az}{2}-\frac b2\coth\frac{bz}{2}.
$$

Using the [Bernoulli numbers](../../../../../bernoulli-number.md) defined by $z/(e^z-1)=\sum_{r\ge0}B_rz^r/r!$, with $B_1=-1/2$, gives

$$
\frac a2\coth\frac{az}{2}=\frac1z+\sum_{r\ge1}\frac{B_{2r}a^{2r}}{(2r)!}z^{2r-1}.
$$

The two poles cancel. Taking $k-1$ further derivatives and evaluating at zero therefore yields all the requested values:

$$
\boxed{\delta_k(c(a,b))=
\begin{cases}
0,&k\text{ odd},\\
\displaystyle\frac{B_k}{k}(a^k-b^k),&k\text{ even}.
\end{cases}}
$$

In particular $\delta_1=0$, $\delta_2=(a^2-b^2)/12$, and $\delta_4=-(a^4-b^4)/120$. The odd case includes $k=1$; substituting $B_1$ into the even-index formula would incorrectly lose the symmetric normalization. All the displayed values lie in $\mathbb Z_p$, directly from the integral [Coleman power series](../../../../../coleman-power-series.md) definition, even when the rational Bernoulli expression has an apparent p-adic denominator. For even $k\ge2$ the same answer is $-(a^k-b^k)\zeta(1-k)$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
