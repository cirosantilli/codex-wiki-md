<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $d\geq2$, write $\widehat x_j$ for the $(d-1)$ coordinates other than $x_j$, and set

$$
S_j(\widehat x_j)=\int_{\mathbb R}s_j(x_1,\ldots,x_{j-1},t,x_{j+1},\ldots,x_d)\,dt.
$$

By [Tonelli theorem](../../../../../tonelli-theorem.md), $\|S_j\|_1=\|s_j\|_1$. The key estimate is the [functional Loomis-Whitney inequality](../../../../../functional-loomis-whitney-inequality.md):

$$
\int_{\mathbb R^d}\prod_{j=1}^d S_j(\widehat x_j)^{1/(d-1)}\,dx\leq\prod_{j=1}^d\left(\int_{\mathbb R^{d-1}}S_j\right)^{1/(d-1)}.
$$

Here is a proof in every dimension. In dimension two, the left-hand side separates into a product of two one-dimensional integrals, so [Tonelli theorem](../../../../../tonelli-theorem.md) gives equality. For $d\geq3$, first integrate $x_d$. Apply [Hölder's inequality](../../../../../holder-s-inequality.md) with $d-1$ factors to $S_1,\ldots,S_{d-1}$, which may depend on $x_d$, and leave the factor $S_d$ outside that integral. Write

$$
H_j(\widehat{x\prime}_j)=\int_{\mathbb R}S_j(\widehat x_j)\,dx_d\quad(j<d).
$$

Each $H_j$ depends on the $d-2$ coordinates other than $j,d$. With $x'=(x_1,\ldots,x_{d-1})$, the full integral is at most

$$
\int_{\mathbb R^{d-1}} S_d(x')^{1/(d-1)}\prod_{j<d}H_j(\widehat{x\prime}_j)^{1/(d-1)}\,dx'.
$$

Put $G(x')=\prod_{j<d}H_j^{1/(d-2)}$. A second application of [Hölder's inequality](../../../../../holder-s-inequality.md), with exponents $d-1$ and $(d-1)/(d-2)$, bounds this expression by

$$
\left(\int S_d\right)^{1/(d-1)}\left(\int G\right)^{(d-2)/(d-1)}.
$$

By induction in dimension $d-1$, $\int G\leq\prod_{j<d}(\int H_j)^{1/(d-2)}$. Since $\int H_j=\int S_j$, substitution proves the claimed functional inequality. Nonnegative integrands justify all integrations; truncation gives the extended-valued version if necessary.

The pointwise hypotheses imply $f^d\leq\prod_j S_j$, so

$$
f^{d/(d-1)}\leq\prod_j S_j^{1/(d-1)}.
$$

Apply the proved functional inequality and take the $(d-1)/d$ power to obtain

$$
\boxed{\|f\|_{d/(d-1)}\leq\prod_{j=1}^d\|s_j\|_1^{1/d}}.
$$

For the useful case all the right-hand norms are finite. If one of them is zero, its line integral vanishes for almost every transverse coordinate and forces $f=0$ almost everywhere; there is no division by that factor. In dimension one the corresponding direct assertion is $\|f\|_\infty\leq\|s_1\|_1$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
