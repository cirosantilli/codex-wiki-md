<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $i:F\hookrightarrow E$. A pair

$$
(x,y)\in H^r(F;\mathbb F_2)\times H^{r+1}(B;\mathbb F_2)
$$

is [transgressive pair](../../../../../transgressive-pair.md) when, in the long exact sequence of the pair $(E,F)$,

$$
\delta x=\pi^*y\in H^{r+1}(E,F;\mathbb F_2),
$$

where $H^{r+1}(B,b_0)$ is identified with reduced cohomology. In the [Serre spectral sequence](../../../../../serre-spectral-sequence.md), this says that $x$ survives to the transgression and

$$
d_{r+1}(x)=y
$$

under the edge identifications, modulo the usual earlier-differential indeterminacy.

The [Kudo transgression theorem](../../../../../kudo-transgression-theorem.md) says that if $(x,y)$ is transgressive and $0\leq j\leq r$, then

$$
(\operatorname{Sq}^j x,\operatorname{Sq}^j y)
$$

is transgressive. To prove it, use relative [Steenrod squares](../../../../../steenrod-square.md). Naturality gives

$$
\operatorname{Sq}^j(\pi^*y)=\pi^*(\operatorname{Sq}^j y),
$$

and stability, equivalently compatibility with the suspension isomorphism, makes squares commute with the connecting map:

$$
\operatorname{Sq}^j(\delta x)=\delta(\operatorname{Sq}^j x).
$$

Applying $\operatorname{Sq}^j$ to $\delta x=\pi^*y$ proves the theorem. The properties used are naturality, stability, additivity, and the instability conditions $\operatorname{Sq}^jz=0$ for $j>|z|$ and $\operatorname{Sq}^{|z|}z=z^2$.

Let $x\in H^1(\mathbb{RP}^\infty;\mathbb F_2)$ be the generator. Instability gives

$$
\operatorname{Sq}(x)=\operatorname{Sq}^0x+\operatorname{Sq}^1x=x+x^2.
$$

The [Cartan formula](../../../../../cartan-formula-algebraic-topology.md) says the total square is multiplicative, so

$$
\operatorname{Sq}(x^k)=(x+x^2)^k
=\sum_{j=0}^k\binom{k}{j}x^{k+j}.
$$

Comparing components yields the complete formula

$$
\boxed{\operatorname{Sq}^j(x^k)=\binom{k}{j}x^{k+j}},
$$

with the binomial coefficient reduced modulo two.

Finally, $\operatorname{Sq}^1$ is the [Bockstein homomorphism](../../../../../bockstein-homomorphism.md) associated with

$$
0\longrightarrow\mathbb Z/2\longrightarrow\mathbb Z/4
\longrightarrow\mathbb Z/2\longrightarrow0.
$$

If a mod-two cocycle representing $y$ is lifted to an integral cochain $A$, write $dA=2B$. Then $B$ modulo two represents $\operatorname{Sq}^1y$. But $dB=0$, because integral cochains are torsion-free and $2dB=d^2A=0$. Thus $B$ itself is a cocycle lift, so its Bockstein vanishes. Therefore

$$
\operatorname{Sq}^1\operatorname{Sq}^1(y)=0
$$

for every space $Y$ and every $y\in H^*(Y;\mathbb F_2)$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 127](../../paper-127-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
