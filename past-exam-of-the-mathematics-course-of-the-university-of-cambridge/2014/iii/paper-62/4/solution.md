<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [GRW model](../../../../../ghirardi-rimini-weber-theory.md) takes a normalized [wave function](../../../../../wave-function.md) in $L^2(\mathbb R^{3N})$. Between jumps it obeys the [Schrödinger equation](../../../../../schrodinger-equation.md), $i\hbar\partial_t\Psi=H\Psi$, with the usual many-particle [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md), for example $H=\sum_i[-\hbar^2\nabla_i^2/(2m_i)]+V(\mathbf x_1,\ldots,\mathbf x_N)$. Each particle has an independent [Poisson process](../../../../../poisson-process.md) of collapse times with rate $1/\tau$. Thus the total jump rate is $N/\tau$, the mean wait is $\tau/N$, and the jumping label is uniform on $\{1,\ldots,N\}$.

At a jump of particle $i$, use the [GRW localization operator](../../../../../grw-localization-operator.md)

$$
L_i(\mathbf c)=(\pi a^2)^{-3/4}\exp[-|\mathbf x_i-\mathbf c|^2/(2a^2)].
$$

Its centre has [probability density function](../../../../../probability-density-function.md) $p_i(\mathbf c)=\|L_i(\mathbf c)\Psi\|^2$. The post-jump [quantum state](../../../../../quantum-state.md) is $L_i(\mathbf c)\Psi/\|L_i(\mathbf c)\Psi\|$. The normalization is consistent because $\int d^3\mathbf c\,L_i(\mathbf c)^2=I$. The collapse times and labels have these state-independent rates; the centres depend on the [wave function](../../../../../wave-function.md) through the [Born rule](../../../../../born-rule.md)-like squared norm.

For precision about the stated spatial event, let $B=Y_{10a}=\{\mathbf c:\operatorname{dist}(\mathbf c,Y)\leq10a\}$. With $H=0$, the [GRW collapse-centre event probabilities](../../../../../grw-collapse-centre-event-probabilities.md) are exactly

$$
p_1(B)=\frac1N\sum_i\int_B\|L_i(\mathbf c)\Psi\|^2\,d^3\mathbf c,
$$



$$
p_{12}(B,B)=\frac1{N^2}\sum_{i,j}\int_Bd^3\mathbf c\int_Bd^3\mathbf d\,
\|L_j(\mathbf d)L_i(\mathbf c)\Psi\|^2,
\qquad
\boxed{p_{2\mid1}(B)=p_{12}(B,B)/p_1(B).}
$$

The last expression is defined only for $p_1(B)>0$. It includes the possibility that the next jump hits the same particle.

Write $f_i^Y(\mathbf x)=|\phi(\mathbf x-\mathbf y_i)|^2$, and similarly $f_i^Z$. Put

$$
g_a(\mathbf u)=(\pi a^2)^{-3/2}e^{-|\mathbf u|^2/a^2},\quad
q_i^Y(\mathbf c)=\int g_a(\mathbf x-\mathbf c)f_i^Y(\mathbf x)\,d^3\mathbf x,
$$



$$
G_B(\mathbf x)=\int_Bg_a(\mathbf x-\mathbf c)\,d^3\mathbf c,\qquad
\eta_i^Y=\int f_i^Y G_B\,d^3\mathbf x,\qquad
R_i^Y=\int f_i^Y G_B^2\,d^3\mathbf x,
$$

with the same definitions for $Z$. The macroscopic separation and negligible packet tails make the two branches essentially orthogonal, so their interference contribution can be neglected. The first-event probability is therefore

$$
\boxed{p_1(B)\simeq\frac{|\alpha|^2}{N}\sum_i\eta_i^Y+\frac{|\beta|^2}{N}\sum_i\eta_i^Z.}
$$

The $Z$ contribution is extremely small: its actual positions are within $r$ of $Z$, whereas centres in $B$ are within $10a$ of $Y$, leaving a distance much larger than $a$ in the Gaussian. Packet-tail errors add to this Gaussian-tail error.

For the next-event calculation, two distinct labels have independent position densities within either product branch, giving factors $\eta_i\eta_j$. A repeated label instead gives $R_i$, since both localization Gaussians multiply the same position variable. Consequently

$$
p_{12}(B,B)\simeq\frac1{N^2}\left[
|\alpha|^2\left(\sum_{i\ne j}\eta_i^Y\eta_j^Y+\sum_iR_i^Y\right)
+|\beta|^2\left(\sum_{i\ne j}\eta_i^Z\eta_j^Z+\sum_iR_i^Z\right)\right].
$$

These formulas, with $p_{2\mid1}=p_{12}/p_1$, answer the spatial questions without an extra containment assumption. If the first event is dominated by the $Y$ branch, they simplify to

$$
\boxed{p_{2\mid1}(B)\simeq
\frac{(\sum_i\eta_i^Y)^2-\sum_i(\eta_i^Y)^2+\sum_iR_i^Y}
{N\sum_i\eta_i^Y}.}
$$

Neglecting the $Z$ term in this conditional expression requires it to be small relative to the retained first-event probability, not merely small in absolute value. The exact operator formulas above cover rare-event exceptions as well.

The intended [GRW branch persistence versus geometric containment](../../../../../grw-branch-persistence-versus-geometric-containment.md) approximation is obtained if $Y$ and $Z$ contain essentially all the position mass of their corresponding branches. Then positions in $Y$ have a Gaussian-centre margin of $10a$ inside $B$, so $\eta_i^Y\simeq R_i^Y\simeq1$, while $\eta_i^Z,R_i^Z\simeq0$. This gives

$$
\boxed{p_1(Y_{10a})\simeq|\alpha|^2,\qquad
p_{2\mid1}(Y_{10a})\simeq1.}
$$

For the Gaussian convention used here, the three-dimensional probability of a displacement exceeding $10a$ is $\operatorname{erfc}(10)+20e^{-100}/\sqrt\pi$, an extremely small number. A first centre near $Y$ also suppresses the $Z$ branch relative to the $Y$ branch by the very small ratio $|\beta|^2q_i^Z(\mathbf c)/(|\alpha|^2q_i^Y(\mathbf c))$ when the latter branch has appreciable weight. All particles are correlated with the same pointer alternative, so one localization selects the macroscopic branch even when the next particle label differs.

The literal PDF, however, only places the packet centres $\mathbf y_i$ in $Y$; it does not say that the packets themselves fit inside $Y$. Since it permits $r>a$, the two numerical approximations just displayed do not follow for every allowed packet and region. For example, take all $\mathbf y_i=0$, let $Y$ be a very small ball, and let $|\phi|^2$ be uniform on a ball of radius $r\gg10a$. Translate the other branch to a similarly small region $Z$ at distance much larger than $100r$. Then

$$
\eta_i^Y\simeq(10a/r)^3\ll1,\qquad
p_1(B)\simeq|\alpha|^2(10a/r)^3.
$$

If these equal packet probabilities are denoted by $\eta$ and their repeated-label integral by $R$, the next probability is

$$
p_{2\mid1}(B)\simeq\frac{N-1}{N}\eta+\frac1N\frac R\eta,
$$

which approaches $\eta$, not one, for large $N$. Thus **packet containment is needed for the stated near-region event to have the usual branch probabilities**. The literal general answer is given by the integrals above.

The physical [GRW amplification mechanism](../../../../../grw-amplification-mechanism.md) remains intact: with properly chosen macroscopic branch regions, spontaneous localization selects the alternatives with approximately the squared branch amplitudes and stabilizes the selected record, on a time scale $\tau/N$. Gaussian tails are not exactly eliminated, so the persistence is approximate. The containment qualification concerns how the region is defined, rather than whether the dynamics selects a macroscopically separated branch.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
