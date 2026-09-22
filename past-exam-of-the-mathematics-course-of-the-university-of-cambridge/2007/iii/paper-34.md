# Paper 34

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper34.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper34.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use base-two [logarithms](../../../calculus.md#logarithm), so [Von Neumann entropy](../../../von-neumann-entropy.md) is measured in bits, and set $0\log0=0$. Write $D(\rho\Vert\sigma)=\operatorname{Tr}\rho(\log_2\rho-\log_2\sigma)$ for the [quantum relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy), the quantity denoted $S(\rho\Vert\sigma)$ in the paper. It is $+\infty$ unless the [support of a positive operator](../../../hilbert-space.md#support-of-a-positive-operator) $\rho$ lies within that of $\sigma$.

We first establish [nonnegativity of quantum relative entropy](../../../von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy), including its equality condition. Let $\rho=\sum_{i:r_i>0}r_i|u_i\rangle\langle u_i|$ and $\sigma=\sum_js_j|v_j\rangle\langle v_j|$, and suppose the support condition holds. Put $q_i=\langle u_i|\sigma|u_i\rangle>0$. Concavity of the scalar logarithm gives

$$
\langle u_i|\log\sigma|u_i\rangle=\sum_j|\langle u_i|v_j\rangle|^2\log s_j\leq\log q_i.
$$

Terms with $s_j=0$ have zero weight here. Working first with natural logarithms, the inequality $-\ln x\geq1-x$ yields

$$
(\ln2)D(\rho\Vert\sigma)\geq\sum_{i:r_i>0}r_i\ln\frac{r_i}{q_i}\geq\sum_{i:r_i>0}(r_i-q_i)\geq0,
$$

since the $q_i$ sum to at most $\operatorname{Tr}\sigma=1$. Equality forces $q_i=r_i$ for every positive-weight eigenvector, no remaining weight of $\sigma$ outside their span, and equality in the logarithm's strict concavity. The latter makes each $u_i$ an eigenvector of $\sigma$ with eigenvalue $q_i$. Thus **$D(\rho\Vert\sigma)=0$ exactly when $\rho=\sigma$**.

For the bipartite [density operator](../../../quantum-theory.md#density-matrix),

$$
\operatorname{supp}\rho_{AB}\subseteq\operatorname{supp}\rho_A\otimes\operatorname{supp}\rho_B.
$$

Indeed, a projector onto the kernel of $\rho_A$, tensored with $I_B$, has zero expectation in $\rho_{AB}$. Positivity implies that $\rho_{AB}$ annihilates its range: $\operatorname{Tr}(\rho_{AB}P)=\|\rho_{AB}^{1/2}P\|_{\mathrm{HS}}^2=0$. The same argument applies to $B$. Hence the [quantum relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy) below is finite. On this support,

$$
\log(\rho_A\otimes\rho_B)=(\log\rho_A)\otimes I_B+I_A\otimes\log\rho_B.
$$

Using the [partial trace](../../../quantum-theory.md#partial-trace) to evaluate the two local terms gives

$$
D(\rho_{AB}\Vert\rho_A\otimes\rho_B)=S(\rho_A)+S(\rho_B)-S(\rho_{AB})\geq0.
$$

This proves [Subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#subadditivity-of-von-neumann-entropy):

$$
\boxed{S(\rho_{AB})\leq S(\rho_A)+S(\rho_B).}
$$

The proof also identifies equality exactly with the product state $\rho_{AB}=\rho_A\otimes\rho_B$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Introduce an orthonormal classical-label basis $|i\rangle$ and the [classical-quantum state](../../../quantum-information-theory.md#classical-quantum-state)

$$
\Gamma_{XA}=\sum_ip_i|i\rangle\langle i|\otimes\rho_i.
$$

Its [reduced density operators](../../../bell-state.md#reduced-density-matrix) are $\Gamma_X=\sum_ip_i|i\rangle\langle i|$ and $\Gamma_A=\overline\rho=\sum_ip_i\rho_i$. If $\lambda_{ij}$ are the eigenvalues of $\rho_i$, the eigenvalues of $\Gamma_{XA}$ are $p_i\lambda_{ij}$. Thus the [entropy of an orthogonal quantum mixture](../../../von-neumann-entropy.md#entropy-of-an-orthogonal-quantum-mixture) is

$$
S(\Gamma_{XA})=H(p)+\sum_ip_iS(\rho_i),\qquad S(\Gamma_X)=H(p),
$$

where $H(p)=-\sum_ip_i\log_2p_i$ is the [Shannon entropy](../../../information-theory.md#information-entropy). Apply the proved [Subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#subadditivity-of-von-neumann-entropy) to $X$ and $A$ and cancel $H(p)$. This gives [Concavity of Von Neumann entropy](../../../von-neumann-entropy.md#concavity-of-von-neumann-entropy):

$$
\boxed{S\left(\sum_ip_i\rho_i\right)\geq\sum_ip_iS(\rho_i).}
$$

Zero-probability terms may simply be omitted. The equality condition from the preceding solution implies that equality holds precisely when all the positive-probability states are the same: the block equations $p_i\rho_i=p_i\overline\rho$ follow from $\Gamma_{XA}=\Gamma_X\otimes\Gamma_A$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Omit indices of probability zero. The [support of a positive operator](../../../hilbert-space.md#support-of-a-positive-operator) of every remaining $\rho_i$ lies within that of $\overline\rho$, because $\overline\rho$ is a positive sum containing $p_i\rho_i$. Thus $D(\rho_i\Vert\overline\rho)$ is finite.

First suppose $\operatorname{supp}\overline\rho\subseteq\operatorname{supp}\sigma$, so all quantities are finite. Expand the trace definitions of [quantum relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy):

$$
\begin{aligned}
\sum_ip_iD(\rho_i\Vert\sigma)-\sum_ip_iD(\rho_i\Vert\overline\rho)
&=\sum_ip_i\operatorname{Tr}\rho_i(\log_2\overline\rho-\log_2\sigma)\\
&=\operatorname{Tr}\overline\rho(\log_2\overline\rho-\log_2\sigma)\\
&=D(\overline\rho\Vert\sigma).
\end{aligned}
$$

Therefore [Donald's identity](../../../von-neumann-entropy.md#donald-s-identity) is

$$
\boxed{\sum_ip_iD(\rho_i\Vert\sigma)=\sum_ip_iD(\rho_i\Vert\overline\rho)+D(\overline\rho\Vert\sigma).}
$$

If the support condition on $\sigma$ fails, at least one positive-weight $\rho_i$ also fails it. The left side and the final term on the right are then $+\infty$, while the first right-hand sum remains finite. The equality is valid in this extended sense, without taking any undefined difference of infinities.

## 2

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A compression scheme consists of [quantum channels](../../../quantum-information-theory.md#quantum-channel)

$$
\mathcal C_n:\mathcal B(\mathcal H^{\otimes n})\to\mathcal B(\mathcal K_n),\qquad\mathcal D_n:\mathcal B(\mathcal K_n)\to\mathcal B(\mathcal H^{\otimes n}),
$$

where each is a [CPTP map](../../../quantum-information-theory.md#quantum-channel). The [Hilbert space](../../../hilbert-space.md) $\mathcal K_n$ is the compressed register. Its block rate in qubits per source qubit is $R_n=n^{-1}\log_2\dim\mathcal K_n$, with asymptotic rate $R=\limsup_nR_n$ (or the limit when it exists).

Use the [squared quantum fidelity](../../../quantum-information-theory.md#squared-quantum-fidelity) convention for the ensemble overlap:

$$
\boxed{F_n=\sum_kp_k^{(n)}\langle\Psi_k^{(n)}|\mathcal D_n\mathcal C_n(|\Psi_k^{(n)}\rangle\langle\Psi_k^{(n)}|)|\Psi_k^{(n)}\rangle.}
$$

This definition tests preservation of the emitted vectors themselves, including nonorthogonal ones; preserving only their classical labels would be a different task. **The scheme is reliable when $F_n\to1$ as $n\to\infty$.** This is the ensemble-average criterion for [reliable quantum source compression](../../../quantum-information-theory.md#reliable-quantum-source-compression). A square root is not taken in this definition, even though an unsquared convention is also used for [quantum fidelity](../../../quantum-information-theory.md#fidelity-of-quantum-states).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Write the spectral decomposition of the one-qubit [density operator](../../../quantum-theory.md#density-matrix) as $\pi=\sum_{j=0}^1\lambda_j|e_j\rangle\langle e_j|$. For a word $\mathbf j=(j_1,\ldots,j_n)$, the [tensor product](../../../linear-algebra.md#tensor-product) vector

$$
|e_{\mathbf j}\rangle=|e_{j_1}\rangle\otimes\cdots\otimes|e_{j_n}\rangle
$$

is an eigenvector of $\pi^{\otimes n}$, with eigenvalue

$$
\boxed{\lambda_{\mathbf j}=\lambda_{j_1}\cdots\lambda_{j_n}.}
$$

These product vectors form an orthonormal [eigenbasis](../../../linear-operator-theory.md#eigenbasis), allowing arbitrary orthonormal choices within degeneracies. Using $\sum_j\lambda_j=1$ and $0\log0=0$,

$$
\begin{aligned}
S(\pi^{\otimes n})
&=-\sum_{j_1,\ldots,j_n}\left(\prod_{s=1}^n\lambda_{j_s}\right)\sum_{s=1}^n\log_2\lambda_{j_s}\\
&=n\left(-\sum_j\lambda_j\log_2\lambda_j\right).
\end{aligned}
$$

Thus the [Von Neumann entropy](../../../von-neumann-entropy.md) is

$$
\boxed{S(\rho^{(n)})=nS(\pi).}
$$

This calculation uses the spectral ensemble of the [memoryless quantum information source](../../../quantum-information-theory.md#memoryless-quantum-information-source); the originally emitted vectors need not equal these eigenvectors.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For fixed $\varepsilon>0$, let the [quantum typical subspace](../../../quantum-information-theory.md#quantum-typical-subspace) $\mathcal T_\varepsilon^{(n)}$ be spanned by the product eigenvectors with nonzero eigenvalues satisfying

$$
2^{-n(S(\pi)+\varepsilon)}\leq\lambda_{\mathbf j}\leq2^{-n(S(\pi)-\varepsilon)}.
$$

Equivalently their spectral information $-n^{-1}\log_2\lambda_{\mathbf j}$ lies within $\varepsilon$ of $S(\pi)$. Denote its [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) by $P_\varepsilon^{(n)}$.

The [typical subspace theorem](../../../quantum-information-theory.md#typical-subspace-theorem) states that for every $\delta>0$ there is $n_0$ such that for $n\geq n_0$,

$$
\boxed{\operatorname{Tr}(\pi^{\otimes n}P_\varepsilon^{(n)})\geq1-\delta,\qquad
(1-\delta)2^{n(S(\pi)-\varepsilon)}\leq\dim\mathcal T_\varepsilon^{(n)}\leq2^{n(S(\pi)+\varepsilon)}.}
$$

Also the operator bounds on its range are

$$
2^{-n(S(\pi)+\varepsilon)}P_\varepsilon^{(n)}\leq P_\varepsilon^{(n)}\pi^{\otimes n}P_\varepsilon^{(n)}\leq2^{-n(S(\pi)-\varepsilon)}P_\varepsilon^{(n)}.
$$

To see the concentration statement, sample $j_s$ independently with probabilities $\lambda_j$. The mean of $-\log_2\lambda_{j_s}$ is $S(\pi)$, so the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) gives typical probability tending to one. Zero-eigenvalue letters have probability zero and are excluded. The dimension bounds follow by summing the upper and lower typical eigenvalue bounds and using the typical mass between $1-\delta$ and $1$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For a block with nonzero typical dimension, write $P=P_\varepsilon^{(n)}$ and $Q=I-P$. Let the compressed register be a copy of the typical space plus a one-dimensional orthogonal failure flag. Choose an isometry $V:P\mathcal H^{\otimes n}\to\mathcal K_n$ onto the successful code sector, extended by zero on $Q$, and a normalized flag $|f\rangle$ orthogonal to its range. Choose any normalized vector $|\varphi\rangle$ in the source [Hilbert space](../../../hilbert-space.md). Define

$$
\mathcal C_n(X)=VPXPV^\dagger+\operatorname{Tr}(QX)|f\rangle\langle f|,
$$



$$
\mathcal D_n(Y)=V^\dagger YV+\langle f|Y|f\rangle|\varphi\rangle\langle\varphi|.
$$

These are [CPTP maps](../../../quantum-information-theory.md#quantum-channel): the first performs the projective test and either encodes or prepares a flag; the second embeds the successful sector and prepares a fixed state on failure. Their trace identities follow from $V^\dagger V=P$ and $VV^\dagger+|f\rangle\langle f|=I_{\mathcal K_n}$. Thus [typical-subspace compression with a failure flag](../../../quantum-information-theory.md#typical-subspace-compression-with-a-failure-flag) implements

$$
\Lambda_n(X)=PXP+\operatorname{Tr}(QX)|\varphi\rangle\langle\varphi|.
$$

For a source vector $|\Psi_k\rangle$, let $a_k=\langle\Psi_k|P|\Psi_k\rangle=\alpha_k^2$. Its overlap with the decoded state is

$$
f_k=a_k^2+(1-a_k)|\langle\Psi_k|\varphi\rangle|^2\geq a_k^2\geq2a_k-1,
$$

where the final step is $(1-a_k)^2\geq0$. Averaging proves [average pure-source fidelity after typical projection](../../../quantum-information-theory.md#average-pure-source-fidelity-after-typical-projection):

$$
\boxed{F_n\geq\sum_kp_k^{(n)}\alpha_k^4\geq2\sum_kp_k^{(n)}\alpha_k^2-1=2\operatorname{Tr}(\rho^{(n)}P)-1.}
$$

No orthogonality of the emitted vectors was used. The code dimension is $\dim\mathcal T_\varepsilon^{(n)}+1$; the extra flag has vanishing asymptotic rate cost. Exceptional small block lengths with empty typical space can use any channel, since they do not affect reliability.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Choose $0<\varepsilon<R-S(\pi)$. The preceding construction and the [typical subspace theorem](../../../quantum-information-theory.md#typical-subspace-theorem) give, for all sufficiently large $n$,

$$
\dim\mathcal K_n\leq2^{n(S(\pi)+\varepsilon)}+1\leq2^{\lceil nR\rceil}.
$$

Embed this code into $m_n=\lceil nR\rceil$ qubits. The unused subspace can be decoded to a fixed source state, making the extended decoder trace preserving; encoded states never enter it. Hence its rate is $m_n/n\to R$.

For every $\delta>0$, sufficiently large $n$ has $\operatorname{Tr}(\pi^{\otimes n}P_\varepsilon^{(n)})\geq1-\delta$. The proved fidelity bound yields

$$
1\geq F_n\geq1-2\delta.
$$

Since $\delta$ is arbitrary, $F_n\to1$. Therefore

$$
\boxed{R>S(\pi)\ \Longrightarrow\ \text{a reliable quantum source code of rate }R\text{ exists}.}
$$

This establishes the achievability part of [Schumacher compression](../../../quantum-information-theory.md#schumacher-compression), including the failure flag and without presuming the source ensemble is orthogonal. If $R$ exceeds one, the same rate-budget construction simply uses spare code qubits; no claim of reducing the physical register size is then needed.

## 3

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The PDF's first Pauli term contains an undefined $\rho_x$. For the stated [depolarizing channel](../../../quantum-information-theory.md#quantum-depolarizing-channel), use $\sigma_x\rho\sigma_x$, consistently with the other two terms. This is the minimal typographical correction needed to define the intended [Pauli channel](../../../quantum-information-theory.md#pauli-channel).

Write $\rho=\frac12(I+\mathbf s\cdot\boldsymbol\sigma)$ using its [Bloch vector](../../../quantum-theory.md#bloch-vector). The [Pauli matrices](../../../algebra.md#pauli-matrices) satisfy $\sigma_j\sigma_k\sigma_j=\sigma_k$ for $j=k$ and $-\sigma_k$ for $j\ne k$. Thus conjugating by each nonidentity Pauli matrix leaves one Bloch component unchanged and reverses the other two. Summing the three conjugates gives

$$
\sum_{j=x,y,z}\sigma_j\rho\sigma_j=\frac12(3I-\mathbf s\cdot\boldsymbol\sigma)=2I-\rho.
$$

Substitution yields

$$
\Phi(\rho)=\left(1-\frac{4p}{3}\right)\rho+\frac{2p}{3}I,
$$

so the [Pauli-mixture parametrization of qubit depolarization](../../../quantum-information-theory.md#pauli-mixture-parametrization-of-qubit-depolarization), with $p$ here the total error probability, gives

$$
\boxed{q=\frac{4p}{3},\qquad\Phi(\rho)=(1-q)\rho+qI/2.}
$$

There is also a genuine range error in the printed claim. For its full $0<p<1$ assumption, $0<q<4/3$, and **$0<q<1$ holds exactly when $0<p<3/4$**. For example $p=9/10$ gives $q=6/5$; on $|0\rangle\langle0|$ the output is $\operatorname{diag}(2/5,3/5)$, with negative $z$ Bloch component. No $q\in(0,1)$ could produce this output from that input, since its component would be $1-q>0$.

The corrected channel is still completely positive in the larger range: its original Pauli probabilities are $1-p,p/3,p/3,p/3$. This is [depolarizing noise weight above one](../../../quantum-information-theory.md#depolarizing-noise-weight-above-one); the formula with $q>1$ is not a convex mixture with weights $1-q,q$, but it has a valid [random unitary channel](../../../quantum-information-theory.md#random-unitary-channel) representation. The subsequent parts can therefore be solved both in the printed $q\in(0,1)$ regime and in the actual parameter range.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

From the derived formula,

$$
\Phi(\rho)=\frac12\left(I+(1-q)\mathbf s\cdot\boldsymbol\sigma\right),
$$

so the action on the [Bloch vector](../../../quantum-theory.md#bloch-vector) is

$$
\boxed{\mathbf s\longmapsto(1-q)\mathbf s=\left(1-\frac{4p}{3}\right)\mathbf s.}
$$

For $0<q<1$, every direction is contracted by the same positive factor. The pure-state [Bloch sphere](../../../quantum-theory.md#bloch-sphere) becomes a concentric sphere of radius $1-q$, and the [Bloch ball](../../../quantum-theory.md#bloch-ball) contracts towards the maximally mixed [density operator](../../../quantum-theory.md#density-matrix) $I/2$. The lack of a preferred direction explains the name [depolarizing channel](../../../quantum-information-theory.md#quantum-depolarizing-channel).

At $q=1$ all inputs become $I/2$. For the allowed Pauli-error range $1<q<4/3$, the factor is negative, so there is also an antipodal reversal; the radius is $q-1\leq1/3$. Thus it would be incorrect to describe the whole printed $p\in(0,1)$ range as positive radial contraction.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For the [quantum state ensemble](../../../quantum-theory.md#quantum-state-ensemble) $\mathcal E=\{p_i,\rho_i\}$ with average $\overline\rho=\sum_ip_i\rho_i$, the [Holevo quantity](../../../quantum-information-theory.md#holevo-quantity) is

$$
\boxed{\chi(\mathcal E)=S(\overline\rho)-\sum_ip_iS(\rho_i)=\sum_ip_iD(\rho_i\Vert\overline\rho).}
$$

The second equality follows by expanding the trace definition: $\sum_ip_i\operatorname{Tr}\rho_i\log\overline\rho=\operatorname{Tr}\overline\rho\log\overline\rho$. All positive-weight states are supported within $\overline\rho$, so the expression is finite.

For a [CPTP map](../../../quantum-information-theory.md#quantum-channel) $\Lambda$, the output average is $\Lambda(\overline\rho)$, with unchanged probabilities $p_i$. The [data-processing inequality for quantum relative entropy](../../../von-neumann-entropy.md#data-processing-inequality-for-quantum-relative-entropy) gives

$$
\begin{aligned}
\chi(\Lambda\mathcal E)
&=\sum_ip_iD(\Lambda(\rho_i)\Vert\Lambda(\overline\rho))\\
&\leq\sum_ip_iD(\rho_i\Vert\overline\rho)
=\chi(\mathcal E).
\end{aligned}
$$

Thus **the Holevo quantity cannot increase under a quantum channel**.

The underlying monotonicity can also be seen directly from [Strong subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#strong-subadditivity-of-quantum-entropy). Attach the classical label $X$, and realize $\Lambda$ by a [Stinespring representation of a completely positive map](../../../quantum-information-theory.md#stinespring-representation-of-a-completely-positive-map) with output $B$ and discarded environment $E$. The isometry preserves $I(X:BE)$, whose input value is $\chi(\mathcal E)$. The difference from the output value is

$$
I(X:BE)-I(X:B)=S(XB)+S(BE)-S(B)-S(XBE)\geq0,
$$

which is precisely strong subadditivity. This explains why discarding an environment loses accessible ensemble information.

Here “operation” means the unconditional channel, including the classical outcome when a measurement is retained. Conditioning on a selected outcome can increase the Holevo quantity. For instance, take equally likely vectors $\sqrt a|0\rangle\pm\sqrt{1-a}|1\rangle$, with $1/2<a<1$. Their input Holevo quantity is $h_2(a)<1$. The filter $K=\operatorname{diag}(\sqrt{(1-a)/a},1)$ succeeds on either state with probability $2(1-a)$ and produces the orthogonal states $|+\rangle,|-\rangle$ after normalization. The success-conditioned quantity is $1$. This does not violate the unconditional statement.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The [Holevo-Schumacher-Westmoreland theorem](../../../quantum-information-theory.md#holevo-schumacher-westmoreland-theorem) gives the classical coding formula

$$
C(\Phi)=\lim_{m\to\infty}\frac1m\chi^*(\Phi^{\otimes m}),\qquad\chi^*(\Lambda)=\sup_{\{p_i,\rho_i\}}\chi(\{p_i,\Lambda(\rho_i)\}).
$$

Its ensemble-coding statement makes every rate below a one-use output [Holevo quantity](../../../quantum-information-theory.md#holevo-quantity) achievable with product input encodings and collective output decoding. Under this product-input restriction, the capacity is

$$
C_{\mathrm{prod}}(\Phi)=\sup_{\{p_i,\rho_i\}}\chi(\{p_i,\Phi(\rho_i)\}).
$$

For any such input ensemble, rates below its output [Holevo quantity](../../../quantum-information-theory.md#holevo-quantity) are achievable with asymptotically vanishing decoding error. Maximization gives the [product-state classical capacity](../../../quantum-information-theory.md#holevo-capacity). The converse follows from the [Holevo bound](../../../quantum-information-theory.md#holevo-s-theorem), entropy bounds on product outputs, and [Fano's inequality](../../../information-theory.md#fano-s-inequality).

Define the [binary entropy](../../../information-theory.md#binary-entropy) $h_2(x)=-x\log_2x-(1-x)\log_2(1-x)$. For an input Bloch radius $r\leq1$, the output eigenvalues are $(1\pm(1-q)r)/2$. Its entropy is

$$
S(\Phi(\rho))=h_2\left(\frac{1+|1-q|r}{2}\right).
$$

On $[1/2,1]$, $h_2$ is decreasing, so this is minimized by pure inputs $r=1$. Throughout the completely positive interval $0\leq q\leq4/3$, the minimum equals $h_2(q/2)$, using symmetry $h_2(x)=h_2(1-x)$. The average output entropy is at most $1$, because it is a qubit. Hence every ensemble satisfies

$$
\chi(\{p_i,\Phi(\rho_i)\})\leq1-h_2(q/2).
$$

Two equally likely orthogonal pure inputs attain this bound: their average output is $I/2$, and each individual output has entropy $h_2(q/2)$. Therefore

$$
\boxed{C_{\mathrm{prod}}(\Phi)=1-h_2(q/2)=1-h_2(2p/3)\quad\text{bits per channel use}.}
$$

This gives the [Holevo capacity of a qubit depolarizing channel](../../../quantum-information-theory.md#holevo-capacity-of-a-qubit-depolarizing-channel) in the noise-weight convention used here.

For completeness, correlated classical code labels do not evade this upper bound. Each product input to $n$ uses has product output entropy at least $nh_2(q/2)$, whereas the average output entropy is at most $n$. Its [Holevo quantity](../../../quantum-information-theory.md#holevo-quantity) is consequently at most $n[1-h_2(q/2)]$. The [Holevo bound](../../../quantum-information-theory.md#holevo-s-theorem) and [Fano's inequality](../../../information-theory.md#fano-s-inequality) rule out a reliable rate larger than this value. Combined with HSW achievability, this proves the capacity under the stated product-input restriction. It also remains valid in the extended physical parameter range arising from the original $p$ assumption.

## 4

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Fix paired orthonormal bases in the two $d$-dimensional [Hilbert spaces](../../../hilbert-space.md). A [maximally entangled state](../../../quantum-theory.md#maximally-entangled-state) is

$$
\boxed{|\Psi_{AB}\rangle=\frac1{\sqrt d}\sum_{j=1}^d|j\rangle_A\otimes|j\rangle_B.}
$$

It is normalized, and the [partial traces](../../../quantum-theory.md#partial-trace) of its rank-one [density operator](../../../quantum-theory.md#density-matrix) are $\rho_A=\rho_B=I/d$. Thus all its [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient) are $1/\sqrt d$ and its [entanglement entropy](../../../von-neumann-entropy.md#entanglement-entropy) is $\log_2d$. No pure bipartite state of these dimensions can have larger entanglement entropy: [nonnegativity of quantum relative entropy](../../../von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy) applied to a reduced state and $I/d$ gives $0\leq D(\rho_A\Vert I/d)=\log_2d-S(\rho_A)$. Hence it is maximally entangled.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Write $|\phi_A\rangle=\sum_jc_j|j\rangle_A$ and choose the [conjugate index vector](../../../quantum-theory.md#conjugate-index-vector)

$$
|\phi_B^*\rangle=\sum_jc_j^*|j\rangle_B,\qquad\langle\phi_B^*|=\sum_jc_j\langle j|_B.
$$

With $|\widetilde\Psi_{AB}\rangle=\sqrt d|\Psi_{AB}\rangle=\sum_j|j\rangle_A|j\rangle_B$, the partial inner product gives

$$
\boxed{(I_A\otimes\langle\phi_B^*|)|\widetilde\Psi_{AB}\rangle=\sum_jc_j|j\rangle_A=|\phi_A\rangle.}
$$

This is the [relative state](../../../quantum-theory.md#relative-state-of-a-bipartite-vector) construction. The coefficient conjugation is defined relative to the fixed paired bases; it is essential, because the bra conjugates those coefficients again. Using the normalized entangled vector instead would give $|\phi_A\rangle/\sqrt d$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [linear operator](../../../vector-space.md#linear-operator) $M_A$ acts on the first factor, while the partial inner product acts on the second. They therefore commute in the contraction:

$$
\begin{aligned}
(I_A\otimes\langle\phi_B^*|)(M_A\otimes I_B)|\widetilde\Psi_{AB}\rangle
&=M_A(I_A\otimes\langle\phi_B^*|)|\widetilde\Psi_{AB}\rangle\\
&=\boxed{M_A|\phi_A\rangle}.
\end{aligned}
$$

Thus the operated vector is exactly the [relative state](../../../quantum-theory.md#relative-state-of-a-bipartite-vector) obtained from the operated bipartite vector using the same [conjugate index vector](../../../quantum-theory.md#conjugate-index-vector). For a physical normalized [pure state](../../../quantum-theory.md#pure-state), divide by $\|M_A\phi_A\|$ when that norm is nonzero. If $M_A\phi_A=0$, the vector identity still holds, but there is no normalized output state for that zero-probability branch. An arbitrary operator is not assumed unitary or norm preserving.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Use the unnormalized [Choi matrix](../../../quantum-information-theory.md#choi-matrix)

$$
J_\Phi=(\Phi_A\otimes\mathrm{id}_B)(|\widetilde\Psi_{AB}\rangle\langle\widetilde\Psi_{AB}|).
$$

It is positive because $\Phi_A$ is a [completely positive map](../../../quantum-information-theory.md#completely-positive-map). Take its spectral decomposition, absorbing square roots of nonzero eigenvalues into the vectors:

$$
J_\Phi=\sum_{k=1}^r|v_k\rangle\langle v_k|,\qquad r=\operatorname{rank}J_\Phi\leq d^2.
$$

Expand $|v_k\rangle=\sum_{i,j}v_{k,ij}|i\rangle_A|j\rangle_B$ and define the [Kraus operator](../../../quantum-information-theory.md#kraus-operator) $A_k$ by $(A_k)_{ij}=v_{k,ij}$. Equivalently,

$$
|v_k\rangle=(A_k\otimes I_B)|\widetilde\Psi_{AB}\rangle.
$$

The preceding [relative state](../../../quantum-theory.md#relative-state-of-a-bipartite-vector) identity then gives $(I\otimes\langle\phi_B^*|)v_k=A_k\phi_A$. Inserting the spectral decomposition into the stated reconstruction identity yields

$$
\Phi_A(|\phi\rangle\langle\phi|)=\sum_kA_k|\phi\rangle\langle\phi|A_k^\dagger.
$$

The conjugated index vector is required here; it is present in the PDF but missing in the converted TeX version of this identity.

Rank-one projectors span all operators by polarization. Explicitly, putting $P(w)=|w\rangle\langle w|$ gives

$$
4|u\rangle\langle v|=P(u+v)-P(u-v)+iP(u+iv)-iP(u-iv).
$$

Thus linearity extends the equality to every $X\in\mathcal B(\mathcal H_A)$:

$$
\boxed{\Phi_A(X)=\sum_kA_kXA_k^\dagger.}
$$

Finally trace preservation and cyclicity of the trace give

$$
\operatorname{Tr}X=\operatorname{Tr}\Phi_A(X)=\operatorname{Tr}\left[X\sum_kA_k^\dagger A_k\right].
$$

For pure-projector inputs this says the Hermitian operator $\sum_kA_k^\dagger A_k-I$ has zero expectation on every vector, so it vanishes. Therefore

$$
\boxed{\sum_kA_k^\dagger A_k=I_A.}
$$

This is the [spectral Kraus decomposition](../../../quantum-information-theory.md#spectral-kraus-decomposition). Using a normalized [Choi state](../../../quantum-information-theory.md#choi-state) $J_\Phi/d$ instead would require the extra factor $\sqrt d$ when reshaping its eigenvectors into Kraus operators.

## 5

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [generalized measurement postulate](../../../quantum-measurement.md#generalized-measurement-postulate) specifies [Kraus operators](../../../quantum-information-theory.md#kraus-operator) $M_{i\alpha}$, where $i$ is the recorded outcome and $\alpha$ permits unobserved alternatives for that outcome, satisfying

$$
\boxed{\sum_{i,\alpha}M_{i\alpha}^\dagger M_{i\alpha}=I.}
$$

For a [density operator](../../../quantum-theory.md#density-matrix) $\rho$, outcome $i$ has probability and conditional state

$$
\boxed{p_i=\operatorname{Tr}\left(\rho\sum_\alpha M_{i\alpha}^\dagger M_{i\alpha}\right),\qquad
\rho_i=\frac{\sum_\alpha M_{i\alpha}\rho M_{i\alpha}^\dagger}{p_i}\quad(p_i>0).}
$$

With one operator per outcome, this is the usual formula $p_i=\operatorname{Tr}(M_i\rho M_i^\dagger)$, $\rho_i=M_i\rho M_i^\dagger/p_i$. The positive operators $E_i=\sum_\alpha M_{i\alpha}^\dagger M_{i\alpha}$ form a [POVM](../../../quantum-measurement.md#positive-operator-valued-measure), while the state-update maps form a [quantum instrument](../../../quantum-measurement.md#quantum-instrument).

The full postulate reduces to the usual [projective measurement](../../../quantum-measurement.md#projective-measurement) with the Lüders update when there is one operator per outcome and $M_i=P_i$, with $P_i=P_i^\dagger=P_i^2$, $P_iP_j=0$ for $i\ne j$, and $\sum_iP_i=I$. Then $p_i=\operatorname{Tr}(P_i\rho)$ and $\rho_i=P_i\rho P_i/p_i$. Projective effects $E_i=P_i$ alone ensure these probabilities but do not fix the state update: an additional outcome-dependent unitary could still be applied. The choice $M_i=P_i$ makes the required projective state-update condition explicit.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The unread measurement is the [pinching map](../../../quantum-measurement.md#pinching-map) $\mathcal P(\rho)=\rho'=\sum_iP_i\rho P_i$, a [nonselective projective measurement](../../../quantum-measurement.md#nonselective-projective-measurement). Its output is block diagonal and commutes with each $P_i$, so $\log\rho'$ also commutes with the projectors on its support.

First the [quantum relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy) $D(\rho\Vert\rho')$ is finite. If $v$ lies in the kernel of $\rho'$, positivity gives

$$
0=\langle v|\rho'|v\rangle=\sum_i\|\rho^{1/2}P_iv\|^2.
$$

Every summand is zero; summing $\rho^{1/2}P_iv=0$ gives $\rho^{1/2}v=0$. Thus $\ker\rho'\subseteq\ker\rho$, equivalently $\operatorname{supp}\rho\subseteq\operatorname{supp}\rho'$.

The block-diagonal logarithm obeys $\sum_iP_i(\log\rho')P_i=\log\rho'$ on this support. Cyclicity of the trace therefore gives

$$
\operatorname{Tr}\rho\log\rho'=\operatorname{Tr}\left(\sum_iP_i\rho P_i\right)\log\rho'=\operatorname{Tr}\rho'\log\rho'.
$$

Consequently the [relative entropy of a pinched state](../../../von-neumann-entropy.md#relative-entropy-of-a-pinched-state) is exactly the entropy increase:

$$
D(\rho\Vert\rho')=-S(\rho)-\operatorname{Tr}\rho\log_2\rho'=S(\rho')-S(\rho).
$$

By the proved [nonnegativity of quantum relative entropy](../../../von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy) and its equality condition,

$$
\boxed{S(\rho')\geq S(\rho),\qquad S(\rho')=S(\rho)\ \Longleftrightarrow\ \rho'=\rho.}
$$

Equivalently, equality holds exactly when all off-diagonal blocks $P_i\rho P_j$ for $i\ne j$ already vanish, or when $\rho$ commutes with every measurement projector. This argument proves the equality condition even when the projectors are degenerate and the states singular.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto the $+1$ eigenspace of the [Pauli matrix](../../../algebra.md#pauli-matrices) $\sigma_z$ is $P_+=(I+\sigma_z)/2$. By the [Born rule](../../../quantum-mechanics.md#born-rule) and the [Bloch vector](../../../quantum-theory.md#bloch-vector) representation,

$$
\mathbb P(+1)=\operatorname{Tr}(\rho P_+)=\frac12\left(1+\operatorname{Tr}(\rho\sigma_z)\right)=\frac{1+s_z}{2}.
$$

Since $s_z=1/5$,

$$
\boxed{\mathbb P(+1)=\frac35.}
$$

The given vector has length $19/30<1$, so it lies inside the [Bloch ball](../../../quantum-theory.md#bloch-ball) and indeed defines a valid mixed qubit state. For the physical spin operator $S_z=(\hbar/2)\sigma_z$, the corresponding outcome is $+\hbar/2$ with the same probability.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
