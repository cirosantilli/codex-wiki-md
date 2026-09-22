<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Repeated [Smith normal form](../../../../../smith-normal-form.md) puts a chain complex of finitely generated free abelian groups into its [elementary decomposition of a finite free chain complex](../../../../../elementary-decomposition-of-a-finite-free-chain-complex.md): one-term summands $\mathbb Z$ and two-term summands $0\to\mathbb Z\xrightarrow{m}\mathbb Z\to0$. Applying $\operatorname{Hom}_{\mathbb Z}(-,\mathbb Z)$ reverses a two-term summand but keeps the same multiplication by $m$. Reading its homology gives the [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md)

$$
0\longrightarrow\operatorname{Ext}_{\mathbb Z}^1(H_{n-1}(C),\mathbb Z)
\longrightarrow H^n(C;\mathbb Z)
\longrightarrow\operatorname{Hom}_{\mathbb Z}(H_n(C),\mathbb Z)
\longrightarrow0,
$$

split noncanonically. Thus if $H_n(C)\cong\mathbb Z^{b_n}\oplus T_n$ with $T_n$ finite, then

$$
H^n(C;\mathbb Z)\cong\mathbb Z^{b_n}\oplus T_{n-1}.
$$

The [universal coefficient theorem for homology](../../../../../universal-coefficient-theorem-for-homology.md) with $\mathbb F_p$ coefficients gives

$$
0\to H_n(C;\mathbb Z)\otimes\mathbb F_p\to H_n(C;\mathbb F_p)\to\operatorname{Tor}_1^{\mathbb Z}(H_{n-1}(C;\mathbb Z),\mathbb F_p)\to0.
$$

If the middle group vanishes for every prime $p$, so does the tensor term. Any nonzero free summand survives for every $p$, and any nonzero finite summand survives for a prime dividing its order. Since integral homology is finitely generated, it must vanish in every degree. This is [detection of integral acyclicity modulo primes](../../../../../detection-of-integral-acyclicity-modulo-primes.md).

For the displayed complex, write

$$
d_M(c,d)=(-d_Cc,-f_\#c+d_Dd).
$$

Using $f_\#d_C=d_Df_\#$, one obtains

$$
d_M^2(c,d)=\bigl(0,f_\#d_Cc-d_Df_\#c\bigr)=0.
$$

Thus $M$ is the [mapping cone](../../../../../mapping-cone-homological-algebra.md) of $f_\#$ in this sign convention. Its [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md) shows that $f_*$ is an isomorphism exactly when $H_*(M)=0$. If $f_*$ is an isomorphism with $\mathbb F_p$ coefficients for every prime, then $M\otimes\mathbb F_p$ is acyclic for every $p$. Prime-field detection makes $M$ integrally acyclic, so the integral long exact sequence gives

$$
\boxed{f_*:H_*(C;\mathbb Z)\xrightarrow{\sim}H_*(D;\mathbb Z).}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
