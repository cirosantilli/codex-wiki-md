<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The expectations use normalized counting measure on a [finite abelian group](../../../../../../finite-abelian-group.md) $G$. This is the finite-group convention implicit in the averaging notation; an arbitrary infinite group has no normalized counting [probability](../../../../../../probability.md) measure on all its points. For $h\in G$, define $\Delta_hf(x)=f(x)\overline{f(x+h)}$, and let $\mathcal C$ denote [complex conjugation](../../../../../../complex-conjugation.md). The [Gowers U3 norm](../../../../../../gowers-u3-norm.md) is

$$
\boxed{\|f\|_{U^3}^8=\mathbb E_{x,h_1,h_2,h_3}\prod_{\omega\in\{0,1\}^3}\mathcal C^{|\omega|}f(x+\omega_1h_1+\omega_2h_2+\omega_3h_3).}
$$

Averaging first over $h_3$ gives the [Derivative identity for the Gowers U3 norm](../../../../../../derivative-identity-for-the-gowers-u3-norm.md)

$$
\|f\|_{U^3}^8=\mathbb E_{h_1,h_2}\left|\mathbb E_x\Delta_{h_1}\Delta_{h_2}f(x)\right|^2\geq0.
$$

Indeed, if $u(x)=\Delta_{h_1}\Delta_{h_2}f(x)$, the average over $(x,h_3)$ is $\mathbb E_{x,h_3}u(x)\overline{u(x+h_3)}=|\mathbb E_xu(x)|^2$. The eighth root is consequently well-defined. Homogeneity follows because the cube has four unconjugated and four conjugated factors, so $\|af\|_{U^3}=|a|\|f\|_{U^3}$. If the [norm](../../../../../../norm.md) is zero, every squared term in the finite average vanishes. Taking $h_1=h_2=0$ gives $\mathbb E_x|f(x)|^4=0$, so $f=0$ pointwise. This proves positive definiteness.

For the [triangle inequality](../../../../../../triangle-inequality.md), we prove the needed [Gowers-Cauchy-Schwarz inequality](../../../../../../gowers-cauchy-schwarz-inequality.md). For eight [functions](../../../../../../function-split.md) $F_\omega$ on a product of [finite sets](../../../../../../finite-set.md) $X_1\times X_2\times X_3$, form the [box norm](../../../../../../box-norm.md) multilinear average

$$
\mathcal L(F)=\mathbb E_{x_j^0,x_j^1}\prod_{\omega\in\{0,1\}^3}\mathcal C^{|\omega|}F_\omega(x_1^{\omega_1},x_2^{\omega_2},x_3^{\omega_3}).
$$

Fix a coordinate $j$. After averaging its two variables separately, this is $\mathbb E A\overline B$, where $A$ uses all vertices with $\omega_j=0$ and $B$ those with $\omega_j=1$, with the remaining parity conjugations. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
|\mathcal L(F)|^2\leq\mathcal L(S_j^0F)\,\mathcal L(S_j^1F),
$$

where $S_j^b$ replaces the [function](../../../../../../function-split.md) at each vertex by the original [function](../../../../../../function-split.md) with its $j$th index [set](../../../../../../set-split.md) to $b$. Each right-hand average is a squared [absolute value](../../../../../../absolute-value.md) averaged over the other coordinates, hence nonnegative. Apply this operation successively for $j=1,2,3$, to every resulting factor. The eight final families each use one original $F_\omega$ at all vertices. Taking roots gives the [box Cauchy-Schwarz inequality](../../../../../../box-cauchy-schwarz-inequality.md)

$$
|\mathcal L(F)|\leq\prod_\omega\|F_\omega\|_{\Box^3}.
$$

Now take $X_j=G$ and $F_\omega(a,b,c)=f_\omega(a+b+c)$. With $x=a_0+b_0+c_0$ and $h_j=x_j^1-x_j^0$, these independent variables induce uniform $(x,h_1,h_2,h_3)$: each such tuple has exactly $|G|^2$ preimages. Therefore each box [norm](../../../../../../norm.md) is the corresponding $U^3$ [norm](../../../../../../norm.md), and the mixed cube obeys

$$
\left|\mathbb E_{x,h_1,h_2,h_3}\prod_\omega\mathcal C^{|\omega|}f_\omega(x+\omega\cdot h)\right|\leq\prod_\omega\|f_\omega\|_{U^3}.
$$

Expand the eight factors in the cube expression for $f+g$. Its $2^8$ mixed terms are bounded by this inequality, and their bounds sum to $(\|f\|_{U^3}+\|g\|_{U^3})^8$. Thus $\boxed{\|f+g\|_{U^3}\leq\|f\|_{U^3}+\|g\|_{U^3}}$, completing the [norm](../../../../../../norm.md) proof.

Two consequences will be useful below. Multiplication by a [character of a finite abelian group](../../../../../../character-of-a-finite-abelian-group.md) leaves the [norm](../../../../../../norm.md) unchanged, because the alternating character product around a three-dimensional cube equals one. Also

$$
\|f\|_{U^3}^8=\mathbb E_h\|\Delta_hf\|_{U^2}^4\geq\frac1{|G|}(\mathbb E_x|f(x)|^2)^4,
$$

where the last inequality uses the $h=0$ term and $\|u\|_{U^2}^4=\sum_\chi|\widehat u(\chi)|^4\geq|\mathbb Eu|^4$. Hence $\|f\|_{U^3}\geq|G|^{-1/8}\|f\|_2$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
