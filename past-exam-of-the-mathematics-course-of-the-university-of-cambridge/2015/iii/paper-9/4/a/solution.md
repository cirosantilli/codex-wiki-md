<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We use a [blow-up compactness proof of an interior Schauder estimate](../../../../../../blow-up-compactness-proof-of-an-interior-schauder-estimate.md), with [Taylor normalization in elliptic blow-up arguments](../../../../../../taylor-normalization-in-elliptic-blow-up-arguments.md). Fix $n,\mu,\delta$ and suppose no suitable constant exists. There would be solutions $u_j$ with forcing $f_j$ for which

$$
S_j^{\mathrm{in}}>\delta S_j+jN_j,\qquad S_j^{\mathrm{in}}=[D^2u_j]_{\mu;B_{1/2}},\quad S_j=[D^2u_j]_{\mu;B_1},\quad N_j=\|u_j\|_{C^2}+\|f_j\|_{C^{0,\mu}}.
$$

Choose distinct $x_j,y_j\in B_{1/2}$ such that, for $r_j=|y_j-x_j|$,

$$
A_j=\frac{|D^2u_j(y_j)-D^2u_j(x_j)|}{r_j^\mu}>\frac12S_j^{\mathrm{in}}.
$$

Then $S_j/A_j<2/\delta$, $N_j/A_j<2/j$, and

$$
r_j^\mu\leq\frac{2\|D^2u_j\|_\infty}{A_j}\leq\frac4j.
$$

In particular $r_j\to0$. Subtract the quadratic [Taylor polynomial](../../../../../../taylor-polynomial.md) of $u_j$ at $x_j$ and rescale:

$$
v_j(z)=\frac{u_j(x_j+r_jz)-u_j(x_j)-r_j\nabla u_j(x_j)\cdot z-\tfrac12r_j^2z^TD^2u_j(x_j)z}{A_jr_j^{2+\mu}}.
$$

Its domain $\{z:x_j+r_jz\in B_1\}$ exhausts $\mathbb R^n$. The normalization gives

$$
v_j(0)=0,\quad\nabla v_j(0)=0,\quad D^2v_j(0)=0,\quad[D^2v_j]_{\mu}\leq2/\delta.
$$

[Taylor theorem](../../../../../../taylor-theorem.md), or integration along line segments from zero, consequently bounds $D^2v_j,\nabla v_j,v_j$ on every fixed ball by constants times $|z|^\mu,|z|^{1+\mu},|z|^{2+\mu}$, respectively. The [Hessian matrices](../../../../../../hessian-matrix.md) are [equicontinuous](../../../../../../equicontinuity.md). The [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) and a diagonal subsequence therefore give $v_j\to v$ in $C^2$ on compact subsets of $\mathbb R^n$.

The rescaled equation is

$$
\Delta v_j(z)=\frac{f_j(x_j+r_jz)-f_j(x_j)}{A_jr_j^\mu},\qquad|\Delta v_j(z)|\leq\frac{[f_j]_\mu}{A_j}|z|^\mu\longrightarrow0
$$

on each compact set. Thus $v$ is harmonic and is smooth. Every entry of its [Hessian matrix](../../../../../../hessian-matrix.md) is harmonic and has a global [Hölder seminorm](../../../../../../holder-seminorm.md) at most $2/\delta$. The allowed [Liouville lemma for globally Hölder harmonic functions](../../../../../../liouville-lemma-for-globally-holder-harmonic-functions.md) makes each entry constant. Since $D^2v(0)=0$, all these constants are zero.

On the other hand, $e_j=(y_j-x_j)/r_j$ is a unit vector and $|D^2v_j(e_j)|=1$ by construction. A further subsequence has $e_j\to e$; the local $C^2$ convergence implies $|D^2v(e)|=1$, a contradiction. Hence the desired constant exists, and

$$
\boxed{[D^2u]_{\mu;B_{1/2}}\leq\delta[D^2u]_{\mu;B_1}+C(n,\mu,\delta)\bigl(\|u\|_{C^2(B_1)}+\|f\|_{C^{0,\mu}(B_1)}\bigr).}
$$

The global [Hölder seminorm](../../../../../../holder-seminorm.md) on the limiting [Hessian matrix](../../../../../../hessian-matrix.md), rather than a bound on its magnitude throughout space, is what makes this Liouville argument work.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
