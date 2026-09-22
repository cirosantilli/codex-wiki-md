<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The exponent in the original PDF is $e^{-\alpha S}$ with real $\alpha>0$, not the $e^{-aS}$ produced by the local TeX. Use that authoritative expression. Put

$$
s=S+\bar S>0,\qquad t=T+\bar T,\qquad q=t-|C|^2>0,\qquad w(S)=ae^{-\alpha S}+b,\qquad W=C^3+w(S).
$$

The domain conditions ensure a real [Kähler potential](../../../../../kahler-potential.md) and positive [Kähler metric](../../../../../kahler-metric.md). There are no gauge multiplets specified, so the [scalar potential](../../../../../scalar-potential.md) is the [supergravity F-term potential](../../../../../supergravity-f-term-potential.md)

$$
V=e^K\left(K^{i\bar j}D_iW\overline{D_jW}-3|W|^2\right),\qquad D_iW=W_i+K_iW,\qquad e^K=\frac1{s q^3}.
$$

The [Kähler covariant derivative of a superpotential](../../../../../kahler-covariant-derivative-of-a-superpotential.md) and metric entries are

$$
D_SW=w_S-\frac Ws,\qquad D_TW=-\frac{3W}{q},\qquad D_CW=3C^2+\frac{3\bar C W}{q},\qquad K_{S\bar S}=s^{-2},
$$



$$
(K_{i\bar j})_{i,j=T,C}=\frac3{q^2}\begin{pmatrix}1&-C\\-\bar C&t\end{pmatrix}.
$$

State the inverse with its indices explicitly, since transposing the off-diagonal complex entries would change the answer:

$$
K^{S\bar S}=s^2,\qquad K^{T\bar T}=\frac{qt}{3},\qquad K^{T\bar C}=\frac{q\bar C}{3},\qquad K^{C\bar T}=\frac{qC}{3},\qquad K^{C\bar C}=\frac q3.
$$

Here $\sum_jK_{i\bar j}K^{k\bar j}=\delta_i^k$, so the displayed upper-index array is the transpose of the ordinary [matrix](../../../../../matrix.md) inverse of the displayed lower-index array.

Substitution shows that the cross terms involving $W$ cancel and that the $T,C$ sector gives

$$
K^{i\bar j}D_iW\overline{D_jW}=3|W|^2+\frac q3|W_C|^2\quad(i,j=T,C).
$$

The first term cancels the universal negative term. Thus the [no-scale supergravity](../../../../../no-scale-supergravity.md) potential is

$$
\boxed{V=\frac{|s w_S-W|^2+3q|C|^4}{s q^3}=\frac{|C^3+b+(1+\alpha s)ae^{-\alpha S}|^2+3q|C|^4}{s q^3}\ge0.}
$$

This positivity is an algebraic cancellation, not an assumption that the individual Kähler derivatives vanish.

Choose the [supergravity auxiliary field](../../../../../supergravity-auxiliary-field.md) convention $F^i=-e^{K/2}K^{i\bar j}\overline{D_jW}$. Direct multiplication gives

$$
\boxed{F^S=e^{K/2}s(\bar W-s\bar w_S),\qquad F^T=e^{K/2}q\bar w,\qquad F^C=-e^{K/2}q\bar C^2.}
$$

A conventional common phase or overall sign on the [auxiliary fields](../../../../../auxiliary-field.md) changes none of the vanishing conditions. A supersymmetric configuration requires every $F^i$ to vanish. First $F^C=0$ implies $C=0$, then $F^T=0$ implies $w=0$, and $F^S=0$ implies $w_S=0$. Since $w_S=-\alpha a e^{-\alpha S}$, at a finite point of the physical domain this is possible only when $a=0$, followed by $b=0$. Consequently **If $(a,b)\ne(0,0)$, every finite configuration has a nonzero [auxiliary field](../../../../../auxiliary-field.md), so any finite vacuum breaks [supersymmetry](../../../../../supersymmetry-split.md)**. The printed request cannot hold for arbitrary parameters without this exception: $a=b=0$, $C=0$ is a zero-energy supersymmetric family with both $S$ and $T$ unfixed.

With the stipulated vanishing [vacuum expectation value](../../../../../vacuum-expectation-value.md) of $C$, define $A(S)=b+(1+\alpha s)ae^{-\alpha S}$. The potential reduces to $|A|^2/(s t^3)$. Its derivative along $t$ is $-3V/t$, so a finite stationary point must have $A=0$. Such a point is a global minimum of the full nonnegative potential, since both squares vanish at $C=0$. The [finite zero-energy vacuum for a single exponential superpotential](../../../../../finite-zero-energy-vacuum-for-a-single-exponential-superpotential.md) therefore satisfies

$$
\boxed{C=0,\qquad b=-(1+\alpha s)ae^{-\alpha S},\qquad V=0.}
$$

For nonzero $a,b$, write $S=\sigma+i\chi$ and $x=\alpha\sigma>0$. The modulus and phase conditions are

$$
\rho\equiv\left|\frac ba\right|=(1+2x)e^{-x},\qquad e^{-i\alpha\chi}=-\frac{b/a}{\rho}.
$$

The function $(1+2x)e^{-x}$ increases up to $x=1/2$ and then decreases to zero; its maximum is $2e^{-1/2}$. Hence a finite minimum exists exactly when

$$
\boxed{a b\ne0,\qquad0<|b/a|\le2e^{-1/2}.}
$$

There is one positive solution for $0<\rho\le1$, two for $1<\rho<2e^{-1/2}$, and one coalesced solution at the upper bound. The formal $x=0$ solution at $\rho=1$ is outside $s>0$. At each allowed $x$, the phase fixes $\chi$ modulo $2\pi/\alpha$. Equivalently $x=-\tfrac12-W_k(-\rho/(2\sqrt e))$, using the real branches of the [Lambert W function](../../../../../lambert-w-function.md) and retaining only $x>0$.

At any of these nontrivial minima, $w=-\alpha s ae^{-\alpha S}\ne0$. The [auxiliary fields](../../../../../auxiliary-field.md) become

$$
\boxed{F^S=F^C=0,\qquad F^T=e^{K/2}t\bar w\ne0.}
$$

This is a [supersymmetry breaking](../../../../../supersymmetry-breaking.md) Minkowski minimum in which the nonzero [auxiliary field](../../../../../auxiliary-field.md) belongs to $T$. Both real components of $T$ are exact [flat directions of a scalar potential](../../../../../flat-direction-of-a-scalar-potential.md) at the minimum. They change the metric and auxiliary-field magnitudes but not the zero potential. Generically the two real components of $S$ are fixed. At the coalesced solution $x=1/2$, the radial quadratic restoring term vanishes, but the leading restoring term is quartic; this is not an additional exact [flat direction of a scalar potential](../../../../../flat-direction-of-a-scalar-potential.md). The matter field $C$ likewise has a positive leading quartic potential, not an exact [flat direction of a scalar potential](../../../../../flat-direction-of-a-scalar-potential.md), despite its zero quadratic mass here.

The exceptional parameter cases must also be stated. If $a=0,b\ne0$ or $a\ne0,b=0$, no finite zero-energy minimum with $C=0$ exists. The same holds when $|b/a|>2e^{-1/2}$. Because the $t$ derivative is nonzero at any positive-energy point on $C=0$, none is a finite minimum there; the energy approaches zero along the runaway $t\to\infty$. If $a=b=0$, all physical $S,T$ at $C=0$ give supersymmetric zero-energy minima. Thus an unconditional finite minimum or unconditional breaking would be a false claim for the printed arbitrary parameters.

For the homogeneous model, assume $\Gamma>0$ is twice differentiable, of degree one in the real moduli $\tau_i$, and that its [Hessian matrix](../../../../../hessian-matrix.md) for $K$ is invertible on the sector considered. Differentiate $K=-3\log\Gamma$:

$$
K_i=-\frac{3\Gamma_i}{\Gamma},\qquad K_{ij}=\frac{3\Gamma_i\Gamma_j}{\Gamma^2}-\frac{3\Gamma_{ij}}{\Gamma}.
$$

The two [Euler theorem for homogeneous functions](../../../../../euler-theorem-for-homogeneous-functions.md) identities in the question imply

$$
\boxed{\tau_iK_{ij}=\frac{3\Gamma_j}{\Gamma}.}
$$

Multiplying by the inverse gives $K^{-1}_{ij}\Gamma_j/\Gamma=\tau_i/3$, so contracting once more yields

$$
\boxed{\frac{\Gamma_iK^{-1}_{ij}\Gamma_j}{\Gamma^2}=\frac13,\qquad K_iK^{-1}_{ij}K_j=3.}
$$

This is the [no-scale identity from degree-one homogeneity](../../../../../no-scale-identity-from-degree-one-homogeneity.md). It does not assert that every degree-one function gives a positive or invertible metric: for example $\Gamma=\tau_1+\tau_2$ has a rank-one Kähler Hessian, and its inverse is undefined. The inverse hypothesis is necessary.

For complex moduli with $\tau_i=T_i+\bar T_i$, the same derivatives are the mixed [Kähler metric](../../../../../kahler-metric.md); choosing real parts with a factor of two only introduces factors that cancel in the contraction. If $W$ is independent of these moduli, $D_iW=K_iW$, and their contribution is $3e^K|W|^2$. It cancels the universal $-3e^K|W|^2$, leaving no [scalar potential](../../../../../scalar-potential.md) from this isolated no-scale sector. **Other chiral sectors can still contribute positive terms**. For this conclusion in a larger theory, the displayed metric must be the appropriate decoupled no-scale block, or the full inverse metric must itself satisfy the corresponding identity; arbitrary mixed additions to $K$ do not inherit the cancellation automatically.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 307](../../paper-307-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
