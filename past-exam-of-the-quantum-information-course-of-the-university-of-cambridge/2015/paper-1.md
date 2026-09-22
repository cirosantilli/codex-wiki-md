# Paper 1

↑ **Parent:** [2015](../2015.md)

Original public paper: [Physical PDF pages 761–764](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=761). All questions and all optional notes are answered. A pure premeasurement state, a nonselective projection, and a state conditional on one observed outcome are distinguished throughout.

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
  - [f](#1/f)
    - [Solution](#1/f/solution)
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
  - [f](#2/f)
    - [Solution](#2/f/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Linearity of the detector's [unitary time evolution](../../quantum-system.md#unitary-time-evolution) maps the two input branches separately, giving the [quantum premeasurement](../../quantum-measurement.md#quantum-premeasurement) state

$$
|\Phi^C\rangle=\frac{|\uparrow d_\uparrow\rangle+|\downarrow d_\downarrow\rangle}{\sqrt2}.
$$

In the ordered [tensor product](../../multilinear-algebra.md#tensor-product) basis $(|\uparrow d_\uparrow\rangle,|\uparrow d_\downarrow\rangle,|\downarrow d_\uparrow\rangle,|\downarrow d_\downarrow\rangle)$, its pure [density matrix](../../density-matrix.md) is

$$
\rho_C=\frac12\begin{pmatrix}1&0&0&1\\0&0&0&0\\0&0&0&0\\1&0&0&1\end{pmatrix}.
$$

A nonselective [projective measurement](../../quantum-measurement.md#projective-measurement) in the indicated detector basis applies $\rho\mapsto\sum_j(I_S\otimes\Lambda_j)\rho(I_S\otimes\Lambda_j)$, removing the two off-diagonal terms:

$$
\boxed{\rho_{\rm up/down}=\frac12\left(|\uparrow d_\uparrow\rangle\langle\uparrow d_\uparrow|
+|\downarrow d_\downarrow\rangle\langle\downarrow d_\downarrow|\right)
=\operatorname{diag}\left(\frac12,0,0,\frac12\right).}
$$

This is the usual nonselective meaning of [von Neumann process 1](../../quantum-measurement.md#von-neumann-process-1). It is not equal to the pure projector $|\Phi^C\rangle\langle\Phi^C|$. If “the detector has clicked” means conditioning on an actual up outcome, the normalized postselected state is instead $|\uparrow d_\uparrow\rangle$, with probability $1/2$. The correlated superposition describes the coherent premeasurement before that selection.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $c=\cos(\theta/2)$ and $s=\sin(\theta/2)$. The detector rotation is real and orthogonal, so its inverse is the same transformation. Substituting it gives

$$
|\Phi^C\rangle=\frac1{\sqrt2}\left[
(c|\uparrow\rangle+s|\downarrow\rangle)|d_\nearrow\rangle
+(s|\uparrow\rangle-c|\downarrow\rangle)|d_\swarrow\rangle\right].
$$

Thus the requested orthonormal system states are

$$
\boxed{|\nearrow\rangle=c|\uparrow\rangle+s|\downarrow\rangle,\qquad
|\swarrow\rangle=s|\uparrow\rangle-c|\downarrow\rangle.}
$$

The pure [density operator](../../density-matrix.md) has not changed: this is only a different [Schmidt decomposition](../../von-neumann-entropy.md#schmidt-decomposition) of a maximally entangled state. But choosing a nonselective [projective measurement](../../quantum-measurement.md#projective-measurement) in this new detector basis gives a different operation and generally a different state:

$$
\boxed{\rho_\theta=\frac12\left(|\nearrow d_\nearrow\rangle\langle\nearrow d_\nearrow|
+|\swarrow d_\swarrow\rangle\langle\swarrow d_\swarrow|\right).}
$$

For an explicit matrix in the original ordered basis, write $q=c^2s^2$ and $h=cs(c^2-s^2)/2$. Then

$$
\rho_\theta=\begin{pmatrix}
\frac12-q&h&h&q\\h&q&q&-h\\h&q&q&-h\\q&-h&-h&\frac12-q
\end{pmatrix}.
$$

At $\theta=\pi/2$ the entries $(1,4)$ and $(2,3)$ are $1/4$, whereas they vanish in $\rho_{\rm up/down}$. Nevertheless, the system and detector individually each have [reduced density matrix](../../bell-state.md#reduced-density-matrix) $I/2$ for either mixture.

This is the [preferred-basis problem](../../quantum-theory.md#preferred-basis-problem): the correlated state alone does not specify which detector observable becomes a stable classical record. Arbitrarily declaring collapse in a Schmidt basis changes the physical prediction. The actual detector interaction and environment must supply the basis selection, rather than a mere choice of notation.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write $H=gI_S\otimes Z_D\otimes X_E$, with $Z_D=\Lambda_\uparrow-\Lambda_\downarrow$. The orthogonal [projection operators](../../vector-space.md#projection-linear-algebra) obey $\Lambda_\uparrow\Lambda_\downarrow=0$ and $\Lambda_j^2=\Lambda_j$. Hence $[Z_D,\Lambda_j]=0$, and the remaining tensor factors commute with detector operators. Therefore

$$
\boxed{[H,I_S\otimes\Lambda_j\otimes I_E]=0,\qquad j=\uparrow,\downarrow.}
$$

The environment interaction preserves these detector populations, making their basis a candidate [pointer basis](../../quantum-theory.md#pointer-basis). It can change their relative coherence without flipping the stored labels.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Since $(Z_D\otimes X_E)^2=I$, the solution of the [Time-dependent Schrödinger equation](../../mathematical-physics.md#time-dependent-schrodinger-equation) is

$$
U(t)=I_S\otimes\left[\cos A\,I_{DE}-i\sin A\,Z_D\otimes X_E\right],
\qquad \boxed{A(t)=gt/\hbar.}
$$

The two detector eigenvalues generate opposite rotations of the environment. Acting on the initial state gives

$$
\boxed{|\Psi(t)\rangle=\frac1{\sqrt2}\left[
|\uparrow d_\uparrow\rangle(\cos A|E_\uparrow\rangle-i\sin A|E_\downarrow\rangle)
+|\downarrow d_\downarrow\rangle(\cos A|E_\uparrow\rangle+i\sin A|E_\downarrow\rangle)\right].}
$$

These are the indicated $|E_-\rangle$ and $|E_+\rangle$. Their [conditional environment overlap](../../quantum-theory.md#conditional-environment-overlap) is $\langle E_+|E_-\rangle=\cos2A$. The [partial trace](../../quantum-theory.md#partial-trace) therefore multiplies the coherence between $|\uparrow d_\uparrow\rangle$ and $|\downarrow d_\downarrow\rangle$ by $\cos2A$. This is an exactly solvable [single-qubit environment dephasing model](../../quantum-theory.md#single-qubit-environment-dephasing-model), with fully reversible global evolution.

<a id="1/d/image-single-qubit-environmental-records-suppress-and-later-restore-reduced-coherence"></a>
![](../../past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2015/paper-1-finite-environment-revival.png)

**[Figure 1](#1/d/image-single-qubit-environmental-records-suppress-and-later-restore-reduced-coherence). Single-qubit environmental records suppress and later restore reduced coherence**. Original ideal unitary model. Zero off-diagonal coherence at one time does not imply irreversible collapse of the full state.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

At $A=\pi/4$, define

$$
\boxed{|E_\leftarrow\rangle=\frac{|E_\uparrow\rangle-i|E_\downarrow\rangle}{\sqrt2},\qquad
|E_\rightarrow\rangle=\frac{|E_\uparrow\rangle+i|E_\downarrow\rangle}{\sqrt2}.}
$$

They are normalized and orthogonal. The full state is the pure superposition $(|\uparrow d_\uparrow E_\leftarrow\rangle+|\downarrow d_\downarrow E_\rightarrow\rangle)/\sqrt2$. A nonselective [von Neumann process 1](../../quantum-measurement.md#von-neumann-process-1) selecting the original detector records gives

$$
\boxed{\rho^{(1)}_{SDE}=\frac12\left(
|\uparrow d_\uparrow E_\leftarrow\rangle\langle\uparrow d_\uparrow E_\leftarrow|
+|\downarrow d_\downarrow E_\rightarrow\rangle\langle\downarrow d_\downarrow E_\rightarrow|\right).}
$$

Without imposing any projection on the full state, tracing out the orthogonal environment states already gives $\rho_{SD}=\rho_{\rm up/down}$ from part (a). These two global descriptions share that reduced state but differ in their global coherence. [Quantum decoherence](../../quantum-theory.md#quantum-decoherence) does not make a pure global state literally equal to the corresponding statistical mixture.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Inverting the detector rotation at this time gives

$$
|\Psi\rangle=\frac1{\sqrt2}\left[
|d_\nearrow\rangle\big(c|\uparrow E_\leftarrow\rangle+s|\downarrow E_\rightarrow\rangle\big)
+|d_\swarrow\rangle\big(s|\uparrow E_\leftarrow\rangle-c|\downarrow E_\rightarrow\rangle\big)
\right].
$$

For a representation with one system factor and one environment factor per displayed detector state, each parenthesized system–environment vector would have to be a [product state](../../bell-state.md#product-state). But the first has coefficient matrix $\operatorname{diag}(c,s)$ in the indicated orthonormal bases; the second has matrix $\operatorname{diag}(s,-c)$. Their [matrix ranks](../../vector-space.md#matrix-rank) are two whenever $cs\ne0$. Equivalently, their two nonzero [Schmidt coefficients](../../von-neumann-entropy.md#schmidt-coefficient) are $|c|,|s|$, which no independent basis changes can remove. Thus **the proposed factorization is impossible when $\sin\theta\ne0$**.

The exception matters: at $\theta=m\pi$, the detector basis is the original basis up to phases or interchange, and a factorization does exist. In particular, the literal condition $\theta\ne0$ is insufficient if it includes $\theta=\pi$. The intended obstruction concerns genuinely mixed detector bases.

The environment has selected robust detector records: its interaction commutes with the original projectors, and orthogonal environmental records suppress their interference in the [reduced density matrix](../../bell-state.md#reduced-density-matrix). A rotated detector branch instead leaves the system and environment entangled. This is [environment-induced pointer-basis selection](../../quantum-theory.md#environment-induced-pointer-basis-selection), the issue analyzed by [W. H. Zurek](../../physicist.md#w-h-zurek) in his apparatus-environment model.[1981 abstract: the apparatus-environment interaction selects recorded observables through a commutation condition](../../physics-bibliography.md#pointer-basis-of-quantum-apparatus-into-what-mixture-does-the-wave-packet-collapse-by-w-h-zurek)

This addresses the basis ambiguity but does not by itself select one realized outcome from the global superposition. Moreover, a two-state environment has recurrences: $\cos2A$ returns to unit modulus, so the toy model does not establish irreversible macroscopic collapse. A large environment can make records effectively persistent over experimental times, but that requires further dynamical assumptions. The distinction is part of the [measurement problem](../../quantum-theory.md#measurement-problem), not an algebraic error cured by a partial trace.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [spin singlet state](../../bell-state.md#spin-singlet-state) has zero local means and outcomes $X,Y\in\{+1,-1\}$, so both [variances](../../variance.md) are one. Its [Pearson correlation coefficient](../../variance.md#pearson-correlation-coefficient) is therefore $C=\mathbb E[XY]$. Summing over the four joint outcomes gives

$$
\boxed{C=P_{++}+P_{--}-P_{+-}-P_{-+}.}
$$

The equal-sign products contribute $+1$ and the opposite-sign products contribute $-1$. In a finite sample the corresponding relative frequencies estimate these probabilities; the formula is not an assertion that a finite random sample has exactly zero empirical means.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

A [spin measurement](../../angular-momentum-operator.md#spin-measurement) along unit vector $\mathbf a$ has outcome projector $\Pi_s(\mathbf a)=(I+s\mathbf a\cdot\boldsymbol\sigma)/2$, with $s=\pm1$. The [spin singlet state](../../bell-state.md#spin-singlet-state) obeys $\langle\sigma_i\otimes I\rangle=\langle I\otimes\sigma_i\rangle=0$ and $\langle\sigma_i\otimes\sigma_j\rangle=-\delta_{ij}$. Applying the [Born rule](../../wave-function.md#born-rule),

$$
\boxed{P_{st}(\mathbf a,\mathbf b)
=\operatorname{Tr}\!\left[\rho_-\Pi_s(\mathbf a)\otimes\Pi_t(\mathbf b)\right]
=\frac{1-st\mathbf a\cdot\mathbf b}{4}.}
$$

Thus $P_{++}=P_{--}=(1-\mathbf a\cdot\mathbf b)/4$ and $P_{+-}=P_{-+}=(1+\mathbf a\cdot\mathbf b)/4$. Substitution into part (a) gives

$$
\boxed{C(\mathbf a,\mathbf b)=-\mathbf a\cdot\mathbf b.}
$$

Equal axes give perfect anticorrelation, while orthogonal axes give zero correlation. Each local marginal remains uniform.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The four required [dot products](../../inner-product.md#dot-product) are

$$
\mathbf a_1\cdot\mathbf b_1=\frac1{\sqrt2},\quad
\mathbf a_1\cdot\mathbf b_3=-\frac1{\sqrt2},\quad
\mathbf a_3\cdot\mathbf b_1=\frac1{\sqrt2},\quad
\mathbf a_3\cdot\mathbf b_3=\frac1{\sqrt2}.
$$

Consequently the specified [CHSH inequality](../../foundations-of-quantum-mechanics.md#chsh-inequality) combination is

$$
\boxed{S=-\frac1{\sqrt2}-\frac1{\sqrt2}-\frac1{\sqrt2}-\frac1{\sqrt2}=-2\sqrt2.}
$$

The magnitude reaches the quantum [Tsirelson bound](../../foundations-of-quantum-mechanics.md#tsirelson-s-bound) and exceeds the local bound two. The negative sign follows this singlet and the stated order of terms; other conventions can reverse it.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let Eve obtain $u,v\in\{\pm1\}$. Applying part (b) to her axes gives $p(u,v)=[1-uv\mathbf n_a\cdot\mathbf n_b]/4$. Conditional on these rank-one local measurements, the forwarded particles are a [product state](../../bell-state.md#product-state) with individual spin directions $u\mathbf n_a$ and $v\mathbf n_b$. Hence

$$
\mathbb E[X\mid u]=u\mathbf a\cdot\mathbf n_a,\qquad
\mathbb E[Y\mid v]=v\mathbf b\cdot\mathbf n_b.
$$

Conditional independence gives the product of these means. Averaging over Eve's outcomes,

$$
C=(\mathbf a\cdot\mathbf n_a)(\mathbf b\cdot\mathbf n_b)
\sum_{u,v}uv\frac{1-uv\mathbf n_a\cdot\mathbf n_b}{4}.
$$

The sum is $-\mathbf n_a\cdot\mathbf n_b$, so

$$
\boxed{C(\mathbf a,\mathbf b)=-(\mathbf a\cdot\mathbf n_a)
(\mathbf n_a\cdot\mathbf n_b)(\mathbf b\cdot\mathbf n_b).}
$$

Eve has turned the entangled source into an ensemble of product states by an [intercept-resend attack](../../computer-science.md#intercept-resend-attack). Ignoring her records does not restore the original singlet coherence.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Write $\mathbf n_a=(\cos\alpha,\sin\alpha)$ and $\mathbf n_b=(\cos\beta,\sin\beta)$. Since $\mathbf b_1-\mathbf b_3=\sqrt2\hat{\mathbf x}$ and $\mathbf b_1+\mathbf b_3=\sqrt2\hat{\mathbf y}$, the [CHSH inequality](../../foundations-of-quantum-mechanics.md#chsh-inequality) combination becomes

$$
S=-\sqrt2\cos(\alpha-\beta)
\left(\cos\alpha\cos\beta+\sin\alpha\sin\beta\right).
$$

Therefore

$$
\boxed{S=-\sqrt2\cos^2(\alpha-\beta),\qquad -\sqrt2\leq S\leq0.}
$$

Parallel or antiparallel Eve axes attain the lower endpoint; orthogonal axes attain zero. This bound is specific to the two-sided projective attack and these planar settings. It is stronger than the generic local bound $|S|\le2$ and should not be attributed to every possible eavesdropping strategy.

If Eve varies her axes independently of the users' still-secret random settings, the measured correlations average over her choices. The same linear combination obeys $S=-\sqrt2\,\mathbb E[\cos^2(\alpha-\beta)]$ and remains in the interval by [convexity](../../real-analysis.md#convex-function). Strategies correlated with disclosed measurement settings would violate that independence premise; the protocol must protect it.

<a id="2/e/image-the-planar-two-sided-intercept-resend-attack-cannot-reproduce-the-singlet-chsh-value"></a>
![](../../past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2015/paper-1-intercept-resend-bound.png)

**[Figure 2](#2/e/image-the-planar-two-sided-intercept-resend-attack-cannot-reproduce-the-singlet-chsh-value). The planar two-sided intercept-resend attack cannot reproduce the singlet CHSH value**. Original analytic curve as Eve changes the relative angle of her measurement axes. The dashed line is the undisturbed singlet result, outside the attack's attainable interval.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

This is an entanglement-based [quantum key distribution](../../computer-science.md#quantum-key-distribution) scheme of the type proposed by [Artur K. Ekert](../../physicist.md#artur-k-ekert).[1991 primary proposal: Bell correlations used to test a key-distribution channel](../../physics-bibliography.md#quantum-cryptography-based-on-bell-s-theorem-by-artur-k-ekert) The measurements generate correlated random data; Alice does not choose a message by choosing their random outcomes.

After the measurements, Alice and Bob announce their basis choices over an authenticated public channel. They retain the pairs with equal axes, here $(\mathbf a_2,\mathbf b_1)$ and $(\mathbf a_3,\mathbf b_2)$, and Bob flips his outcome signs to match Alice's bits. They sacrifice a random subset for error estimation and use the appropriate other setting combinations to estimate $S$. In the ideal source the same-axis bits match after the flip and $S=-2\sqrt2$; the specified intercept-resend attack cannot reproduce that value.

A practical protocol includes information reconciliation, an accounting of information leaked publicly, and [privacy amplification](../../computer-science.md#privacy-amplification). It must abort when its statistical security conditions fail. Authentication is essential: a completely unauthenticated public channel permits a [man-in-the-middle attack](../../computer-science.md#man-in-the-middle-attack). A Bell-violation observation alone, without sampling, device and adversary assumptions and a finite-key analysis, is not a proof that Eve knows no key bits.

With a sufficiently uniform secret shared key $k$ of the required length, Alice can send $c=m\oplus k$ publicly using a [one-time pad](../../coding-theory.md#one-time-pad); Bob recovers $m=c\oplus k$. **The pad must be secret, as long as the protected message, and never reused.** A complete security proof makes the probability or distinguishing advantage of failure small under stated assumptions. The ideal exam correlations diagnose the stated attack; they do not provide an unconditional guarantee against every attack or implementation fault.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A bipartite pure state is entangled when it is not a [product state](../../bell-state.md#product-state). Its [Schmidt decomposition](../../von-neumann-entropy.md#schmidt-decomposition) is $|\psi\rangle=\sum_i\sqrt{\lambda_i}|i_Ai_B\rangle$, where $\lambda_i\ge0$ and $\sum_i\lambda_i=1$. More than one nonzero coefficient means entanglement. The two [reduced density matrices](../../bell-state.md#reduced-density-matrix) have the same nonzero spectrum, and their [Von Neumann entropy](../../von-neumann-entropy.md) $-\sum_i\lambda_i\log_2\lambda_i$ is the pure-state [entanglement entropy](../../von-neumann-entropy.md#entanglement-entropy). A maximally entangled pair of qubits has one bit of this entropy.

For mixed states, classical correlations are not sufficient: a [separable quantum state](../../quantum-information-theory.md#separable-quantum-state) is a convex mixture $\sum_jp_j\rho_A^{(j)}\otimes\rho_B^{(j)}$, and entanglement means that no such decomposition exists. A reduced entropy alone no longer measures mixed-state entanglement. An [entanglement witness](../../quantum-information-theory.md#entanglement-witness) or a suitable separability criterion can detect it.

[Local unitary transformations](../../bell-state.md#local-unitary-operation) preserve the Schmidt spectrum. More general [local operations and classical communication](../../bell-state.md#local-operations-and-classical-communication) can discard entanglement but cannot freely create it from a separable input. [Nielsen's pure-state conversion theorem](../../bell-state.md#nielsen-s-pure-state-conversion-theorem) gives the exact deterministic criterion: $|\psi\rangle\to|\phi\rangle$ is possible precisely when $\lambda^\psi\prec\lambda^\phi$. In decreasing order, every partial sum for the input is no larger than the corresponding output sum, with equal totals. The direction matters: a uniform spectrum can be converted to a concentrated one; a product state cannot deterministically become a Bell pair.

A probabilistic local filter can concentrate a partially entangled pair. For $|\psi\rangle=\sqrt\lambda|00\rangle+\sqrt{1-\lambda}|11\rangle$ with $1/2\le\lambda<1$, Alice's successful operator $F=\operatorname{diag}(\sqrt{(1-\lambda)/\lambda},1)$ produces equal amplitudes. The outcome is a Bell pair with probability $2(1-\lambda)$; a complementary operator supplies a complete measurement. Failure is heralded, so there is no deterministic creation of a more entangled pair. This illustrates [entanglement concentration](../../bell-state.md#entanglement-concentration).

Many-copy [entanglement distillation](../../bell-state.md#entanglement-distillation) and [entanglement dilution](../../bell-state.md#entanglement-dilution) connect noisy or nonuniform resources with standard Bell pairs. Entanglement enables [quantum teleportation](../../bell-state.md#quantum-teleportation) and other protocols, but classical communication is still required; the [no-communication theorem](../../bell-state.md#no-communication-theorem) excludes message transmission merely by choosing a distant local measurement.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A [qubit](../../quantum-system.md#qubit) has state $\alpha|0\rangle+\beta|1\rangle$ with $|\alpha|^2+|\beta|^2=1$. An $n$-qubit register occupies a $2^n$-dimensional [Hilbert space](../../hilbert-space.md) and may contain entanglement. This large state space does not mean that a measurement reads out all its complex amplitudes: computational-basis outcomes occur with the [Born rule](../../wave-function.md#born-rule) probabilities.

A [quantum circuit](../../quantum-circuit.md) prepares a register, applies [quantum gates](../../quantum-circuit.md#quantum-logic-gate), and measures selected outputs, possibly using classical feed-forward. Closed gates are [unitary operators](../../vector-space.md#unitary-operator) and therefore reversible; initialization, measurement and discarding can be treated using a larger system and environment. Single-qubit rotations together with an entangling two-qubit gate give a [universal quantum gate set](../../quantum-circuit.md#universal-quantum-gate-set). The [CNOT gate](../../quantum-theory.md#controlled-not-gate) acts as $|x,y\rangle\mapsto|x,y\oplus x\rangle$.

For example, a [Hadamard gate](../../quantum-theory.md#hadamard-gate) on the first qubit of $|00\rangle$ followed by a CNOT creates $(|00\rangle+|11\rangle)/\sqrt2$. A Hadamard produces amplitudes with relative signs, so later gates can make unwanted alternatives interfere destructively and useful alternatives reinforce. [Quantum algorithms](../../algorithm.md#quantum-algorithm) organize this interference to improve a specified computational task; superposition alone does not supply an arbitrary speedup or permit reading every branch.

A finite discrete universal set such as Clifford gates together with a non-Clifford phase gate approximates general unitaries to chosen precision. Runtime includes the number of gates, repetitions and classical processing. Measurement outcomes may require multiple runs to estimate a probability or amplify success.

[Quantum decoherence](../../quantum-theory.md#quantum-decoherence) and imperfect gates limit an implementation. [Quantum error correction](../../quantum-error-correction.md) encodes logical information into several physical qubits and measures error syndromes without directly learning the encoded amplitudes. Under appropriate noise and control assumptions, fault tolerance permits reliable longer computations; simply maintaining an isolated ideal state is not a realistic account of a large processor.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

In [de Broglie-Bohm theory](../../foundations-of-quantum-mechanics.md#de-broglie-bohm-theory), the system has both a [wavefunction](../../wave-function.md) and an actual configuration of particle positions. The wavefunction obeys the [Time-dependent Schrödinger equation](../../mathematical-physics.md#time-dependent-schrodinger-equation); the configuration follows the [guidance equation](../../foundations-of-quantum-mechanics.md#guidance-equation). For spinless particles without electromagnetic vector potentials, write $\Psi=R e^{iS/\hbar}$ using a dimensionful action $S$. Then

$$
\boxed{\dot{\mathbf Q}_i=\frac{\nabla_iS}{m_i}
=\frac\hbar{m_i}\operatorname{Im}\frac{\nabla_i\Psi}{\Psi}\bigg|_{\mathbf q=\mathbf Q}.}
$$

The actual configuration selects a trajectory, while the guiding wave generally retains all branches. A measurement correlates system and apparatus configurations; the actual apparatus position lies in one recorded branch. Effective collapse follows when wave packets have separated sufficiently in configuration space, although the full wave continues its Schrödinger evolution.

Substituting the polar form into that equation yields the [probability continuity equation](../../wave-function.md#probability-continuity-equation) and a modified Hamilton-Jacobi equation,

$$
\partial_tS+\sum_i\frac{|\nabla_iS|^2}{2m_i}+V+Q=0,
\qquad Q=-\sum_i\frac{\hbar^2}{2m_i}\frac{\nabla_i^2R}{R}.
$$

The amplitude-dependent term is the [quantum potential](../../foundations-of-quantum-mechanics.md#quantum-potential). Taking gradients gives a second-order force description, but initial velocities remain constrained by the guidance law. Nodes require care because the displayed quotient is singular there.

If the initial configuration distribution is $|\Psi|^2$, the same continuity equation preserves that distribution: [quantum equilibrium equivariance](../../foundations-of-quantum-mechanics.md#quantum-equilibrium-equivariance). It then reproduces ordinary nonrelativistic quantum measurement statistics within the model's applicability. Equivariance preserves a distribution; it is not by itself a proof that every initial distribution equals $|\Psi|^2$.

For entangled particles the guiding wave lives on their joint configuration space, so one particle's velocity can depend on the distant actual configuration. This explicit nonlocality avoids the locality premise of a [Bell inequality](../../foundations-of-quantum-mechanics.md#bell-inequality). In quantum equilibrium it does not permit controllable faster-than-light signalling. Spin extensions use a spinor wavefunction and its probability current; they need not assign a classical little spinning vector with simultaneous definite values for every spin component.

[David Bohm](../../physicist.md#david-joseph-bohm) developed this account in his two 1952 papers. The first sets out the dynamics and the second treats measurement and the relation to ordinary predictions.[1952, first paper in the two-part interpretation](../../physics-bibliography.md#a-suggested-interpretation-of-the-quantum-theory-in-terms-of-hidden-variables-i-by-david-bohm)[1952, second paper on the measurement account](../../physics-bibliography.md#a-suggested-interpretation-of-the-quantum-theory-in-terms-of-hidden-variables-ii-by-david-bohm) The theory supplies additional dynamical variables and a particular nonlocal account of outcomes, rather than deriving a unique interpretation from the standard wavefunction alone.

## ↑ Ancestors (11)

1. [2015](../2015.md)
2. [Past exam of the quantum information course of the University of Cambridge](../../past-exam-of-the-quantum-information-course-of-the-university-of-cambridge.md)
3. [Quantum Information course of the University of Cambridge](../../university-of-cambridge.md#quantum-information-course-of-the-university-of-cambridge)
4. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
