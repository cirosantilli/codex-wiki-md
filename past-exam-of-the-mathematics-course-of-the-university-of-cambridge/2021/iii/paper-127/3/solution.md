<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Because $S^n$ is simply connected for $n\geq2$, the homological [Serre spectral sequence](../../../../../serre-spectral-sequence.md) has constant coefficients and only two nonzero columns:

$$
E^2_{p,q}=H_p(S^n;H_q(F))
=\begin{cases}
H_q(F),&p=0,n,\\
0,&\text{otherwise}.
\end{cases}
$$

Its only possible nonzero differential is

$$
d_n:E^n_{n,i}\longrightarrow E^n_{0,i+n-1}.
$$

Using the orientation generator of $H_n(S^n)$ to identify both columns with $H_*(F)$ defines the [Wang homomorphism](../../../../../wang-homomorphism.md)

$$
\Delta:H_i(F)\longrightarrow H_{i+n-1}(F).
$$

The kernel and cokernel descriptions of the two surviving columns splice with the filtration of $H_*(E)$ to give the [Wang sequence over a sphere](../../../../../wang-sequence-over-a-sphere.md)

$$
\cdots\to H_j(F)\to H_j(E)\to H_{j-n}(F)
\xrightarrow{\Delta}H_{j-1}(F)\to H_{j-1}(E)\to\cdots.
$$

Let $F_m$ be the [homotopy fiber](../../../../../homotopy-fiber.md) of a degree-$m$ map $f_m:S^n\to S^n$. Apply this sequence to the fibration

$$
F_m\longrightarrow S^n\xrightarrow{f_m}S^n.
$$

At the bottom, the map between the two copies of $H_n(S^n)$ is multiplication by $m$. It follows that

$$
H_j(F_m;\mathbb Z)=
\begin{cases}
\mathbb Z,&j=0,\\
\mathbb Z/m,&j=k(n-1)\text{ for some }k\geq1,\\
0,&\text{otherwise}.
\end{cases}
$$

The first torsion group can also be seen from $\pi_{n-1}(F_m)\cong\mathbb Z/m$ and the [Hurewicz theorem](../../../../../hurewicz-theorem.md); the Wang map then propagates it periodically.

The [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md) gives

$$
H^j(F_m;\mathbb Z)=
\begin{cases}
\mathbb Z,&j=0,\\
\mathbb Z/m,&j=k(n-1)+1\text{ for some }k\geq1,\\
0,&\text{otherwise}.
\end{cases}
$$

Every product of two positive-degree classes is zero. For $n>2$, this follows immediately because the sum of two degrees of the form $k(n-1)+1$ is not of that form. For $n=2$, degree counting does not suffice, since $H^j(F_m)\cong\mathbb Z/m$ for every $j\geq2$. Use instead the multiplicative cohomological [Serre spectral sequence](../../../../../serre-spectral-sequence.md) for

$$
\Omega S^2\longrightarrow F_m\longrightarrow S^2.
$$

Its transgression in degree one is multiplication by $m$. Every positive integral cohomology class that survives lies in filtration two, while the product of two such classes lies in filtration four; the base has dimension two, so filtration four is zero. Thus the reduced cohomology is a square-zero ideal, and

$$
H^*(F_m;\mathbb Z)
=\mathbb Z\oplus\bigoplus_{k\geq1}(\mathbb Z/m)[k(n-1)+1]
$$

as a graded ring, with zero multiplication on the second summand.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 127](../../paper-127-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
