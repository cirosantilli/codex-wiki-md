<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $G=\operatorname{Gal}(L/K)$ and normalize $v_L$. The lower [ramification groups](../../../../../../ramification-group.md) are

$$
G_s(L/K)=\{\sigma\in G:v_L(\sigma(x)-x)\geq s+1\text{ for every }x\in\mathcal O_L\},
\qquad s\geq0,
$$

with $G_{-1}=G$. If $K\subseteq M\subseteq L$, the same inequality defines $G_s(L/M)$ inside $\operatorname{Gal}(L/M)$, so directly

$$
G_s(L/M)=G_s(L/K)\cap\operatorname{Gal}(L/M).
$$

Now suppose $M/K$ is [Finite Galois extension](../../../../../../finite-galois-extension.md). The [inertia group](../../../../../../inertia-group.md) is the kernel of the action on the residue field. Restriction sends $G_0(L/K)$ into $G_0(M/K)$. Conversely, the maximal unramified subextension of $M/K$ is the intersection of $M$ with the maximal unramified subextension of $L/K$. The Galois correspondence therefore shows that the restriction image is all of $G_0(M/K)$.

For the explicit extension, take $\alpha^3=3$ and a primitive cube root of unity $\zeta$. The polynomial $X^3-3$ is Eisenstein over $\mathbb Q_3$, while $\mathbb Q_3(\zeta)/\mathbb Q_3$ is a ramified quadratic extension. Its splitting field

$$
L=\mathbb Q_3(\alpha,\zeta)
$$

is therefore a totally ramified extension of degree six with Galois group $S_3$. With $v_L(3)=6$, one has $v_L(\alpha)=2$ and $v_L(\zeta-1)=3$, so

$$
\pi=\frac{\zeta-1}{\alpha}
$$

is a uniformizer. Let $\tau(\alpha)=\zeta\alpha$, $\tau(\zeta)=\zeta$, and let $\sigma(\alpha)=\alpha$, $\sigma(\zeta)=\zeta^{-1}$. Then

$$
v_L(\tau(\pi)-\pi)=v_L((\zeta^{-1}-1)\pi)=4,
\qquad
v_L(\sigma(\pi)-\pi)=1.
$$

The two nonidentity elements of $\langle\tau\rangle=A_3$ have ramification number four, whereas each transposition has ramification number one. Hence

$$
G_{-1}=G_0=S_3,
\qquad
G_1=G_2=G_3=A_3,
\qquad
G_s=1\quad(s\geq4).
$$

In particular, $A_3$ is the [wild inertia group](../../../../../../wild-inertia-group.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
