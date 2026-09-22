<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write the [monad](../../../../../monad.md) identities as

$$
\mu_A\eta_{TA}=1_{TA}=\mu_AT\eta_A,\qquad
\mu_AT\mu_A=\mu_A\mu_{TA}.
$$

If $\mu_A$ is invertible, its two right inverses agree, so $\eta_{TA}=T\eta_A$. Conversely, suppose $\eta_T=T\eta$. [Naturality](../../../../../naturality.md) of $\eta$ at $\mu_A$, followed by that equality at $TA$, gives

$$
\eta_{TA}\mu_A=T\mu_A\eta_{TTA}=T\mu_AT\eta_{TA}=T(\mu_A\eta_{TA})=1_{TTA}.
$$

Together with $\mu_A\eta_{TA}=1_{TA}$ this proves

$$
\boxed{\mu\text{ is invertible}\ \Longleftrightarrow\ \eta_T=T\eta,\qquad\mu^{-1}=\eta_T=T\eta.}
$$

This is the equivalence defining an [idempotent monad](../../../../../idempotent-monad.md).

For the [equalizer submonad of a monad](../../../../../equalizer-submonad-of-a-monad.md), let $\beta_A:RA\to TA$ equalize $\eta_{TA}$ and $T\eta_A$. If $f:A\to B$, [naturality](../../../../../naturality.md) of these two transformations shows that $Tf\beta_A$ equalizes the corresponding pair at $B$. There is therefore a unique $Rf$ satisfying

$$
\beta_BRf=Tf\beta_A.
$$

Uniqueness gives $R1=1$ and $R(gf)=Rg\,Rf$, so $R$ is a [functor](../../../../../functor.md) and $\beta:R\Rightarrow T$ is a [natural transformation](../../../../../natural-transformation.md).

Take the stipulated factorizations $\alpha_A$ and $\theta_A$. [Naturality](../../../../../naturality.md) of $\beta$ at $\beta_A$ rewrites their defining equations as

$$
\beta_A\alpha_A=\eta_A,\qquad
\beta_A\theta_A=\mu_A\beta_{TA}R\beta_A=\mu_AT\beta_A\beta_{RA}.
$$

The composites on the right are natural in $A$; cancellation of the [monic arrow](../../../../../monomorphism.md) $\beta_A$ therefore makes $\alpha$ and $\theta$ natural. We now verify every [monad](../../../../../monad.md) law, rather than assuming that restricting the structure automatically preserves them.

For the two unit laws, [naturality](../../../../../naturality.md) and the unit laws of $T$ give

$$
\begin{aligned}
\beta_A\theta_A\alpha_{RA}
&=\mu_AT\beta_A\eta_{RA}
=\mu_A\eta_{TA}\beta_A=\beta_A,\\
\beta_A\theta_AR\alpha_A
&=\mu_AT\beta_AT\alpha_A\beta_A
=\mu_AT\eta_A\beta_A=\beta_A.
\end{aligned}
$$

Cancelling $\beta_A$ proves $\theta_A\alpha_{RA}=1_{RA}=\theta_AR\alpha_A$. For associativity, the same [naturality](../../../../../naturality.md) equations give

$$
\begin{aligned}
\beta_A\theta_AR\theta_A
&=\mu_AT\mu_A\,TT\beta_A\,T\beta_{RA}\,\beta_{RRA},\\
\beta_A\theta_A\theta_{RA}
&=\mu_A\mu_{TA}\,TT\beta_A\,T\beta_{RA}\,\beta_{RRA}.
\end{aligned}
$$

These are equal by associativity of $\mu$; cancelling $\beta_A$ proves associativity of $\theta$. Thus

$$
\boxed{(R,\alpha,\theta)\text{ is a monad, and }\beta:R\Rightarrow T\text{ is a monad morphism}.}
$$

The remaining claims use two [split equalizers associated with a monad](../../../../../split-equalizers-associated-with-a-monad.md). First, $\eta_{TA}:TA\to TTA$ is a [split equalizer](../../../../../split-equalizer.md) of $\eta_{TTA},T\eta_{TA}$. Its retraction is $\mu_A$, and the splitting of the parallel pair is $T\mu_A$, since

$$
\mu_A\eta_{TA}=1,\qquad
T\mu_A\eta_{TTA}=\eta_{TA}\mu_A,\qquad
T\mu_AT\eta_{TA}=1.
$$

The equalizing equation follows from [naturality](../../../../../naturality.md) of $\eta$. In general, identities $re=1$, $sf=er$, $sg=1$ and $fe=ge$ prove that $e$ is an [equalizer](../../../../../equaliser.md): if $fh=gh$, then $h=erh$, with unique factorization $rh$. Hence $\eta_{TA}$ and $\beta_{TA}$ are two [equalizers](../../../../../equaliser.md) of the same pair. Their comparison is $\alpha_{TA}$, and its inverse is $\mu_A\beta_{TA}$. In particular

$$
\boxed{\alpha_{TA}\text{ is invertible},\qquad \alpha_{TA}^{-1}=\mu_A\beta_{TA}.}
$$

Second, $e_A=T\eta_A:TA\to TTA$ is a [split equalizer](../../../../../split-equalizer.md) of $TT\eta_A,T\eta_{TA}$, with retraction $\mu_A$ and splitting $\mu_{TA}$. Indeed,

$$
\mu_AT\eta_A=1,\qquad
\mu_{TA}TT\eta_A=T\eta_A\mu_A,\qquad
\mu_{TA}T\eta_{TA}=1.
$$

This is precisely the parallel pair in the PDF's diagram after $T\beta_A$. The map $T\beta_A$ equalizes that pair, because applying $T$ to the defining [equalizer](../../../../../equaliser.md) equation gives their equality on $T\beta_A$. Put

$$
h_A=\mu_AT\beta_A:TRA\to TA.
$$

The split-equalizer factorization and $\beta_A\alpha_A=\eta_A$ give

$$
e_Ah_A=T\beta_A,\qquad h_AT\alpha_A=1_{TA}.
$$

If $T\alpha_A$ is invertible, then $T\beta_A=e_A(T\alpha_A)^{-1}$ is a [monic arrow](../../../../../monomorphism.md). Conversely, if $T\beta_A$ is a [monic arrow](../../../../../monomorphism.md), the equation

$$
T\beta_A(T\alpha_Ah_A)=e_Ah_A=T\beta_A
$$

forces $T\alpha_Ah_A=1_{TRA}$, so $h_A$ is the inverse of $T\alpha_A$. Therefore

$$
\boxed{T\alpha_A\text{ invertible}\ \Longleftrightarrow\ T\beta_A\text{ monic}.}
$$

Notice that, under either condition, $T\beta_A$ is actually a [split monomorphism](../../../../../split-monomorphism.md), with retraction $T\alpha_A\mu_A$. Thus $TT\beta_A$ is a [monic arrow](../../../../../monomorphism.md) too, since a [functor](../../../../../functor.md) preserves [split monomorphisms](../../../../../split-monomorphism.md). We have not assumed that $T$ preserves arbitrary [monomorphisms](../../../../../monomorphism.md).

Now prove the specified [naturality](../../../../../naturality.md) square is a [pullback in a category](../../../../../pullback-category-theory.md). Let $x:X\to TRA$ and $y:X\to RTA$ satisfy $T\beta_Ax=\beta_{TA}y$. [Naturality](../../../../../naturality.md) of $\eta$, followed by the [equalizer](../../../../../equaliser.md) equation for $\beta_{TA}$, gives

$$
\begin{aligned}
TT\beta_A\eta_{TRA}x
&=\eta_{TTA}T\beta_Ax
=\eta_{TTA}\beta_{TA}y\\
&=T\eta_{TA}\beta_{TA}y
=T\eta_{TA}T\beta_Ax
=TT\beta_AT\eta_{RA}x.
\end{aligned}
$$

Cancel the [monic arrow](../../../../../monomorphism.md) $TT\beta_A$. Thus $x$ equalizes $\eta_{TRA},T\eta_{RA}$ and factors uniquely as $x=\beta_{RA}z$ with $z:X\to RRA$. [Naturality](../../../../../naturality.md) of $\beta$ then gives

$$
\beta_{TA}R\beta_Az=T\beta_A\beta_{RA}z=T\beta_Ax=\beta_{TA}y.
$$

Cancel $\beta_{TA}$ to obtain $R\beta_Az=y$. This is exactly existence and uniqueness in the pullback [universal property](../../../../../universal-property.md).

Because the square is a pullback and $T\beta_A$ is a [monic arrow](../../../../../monomorphism.md), $R\beta_A$ is a [monic arrow](../../../../../monomorphism.md). [Naturality](../../../../../naturality.md) of $\alpha$ and the formula for $\theta$ now give

$$
R\beta_A\alpha_{RA}\theta_A
=\alpha_{TA}\beta_A\theta_A
=\alpha_{TA}\mu_A\beta_{TA}R\beta_A
=R\beta_A.
$$

Cancelling $R\beta_A$ proves $\alpha_{RA}\theta_A=1_{RRA}$. The other composite is already one of the unit laws. Hence $\theta_A$ is invertible. If the equivalent monicity conditions hold for every $A$, we conclude

$$
\boxed{(R,\alpha,\theta)\text{ is idempotent},\qquad \theta^{-1}=\alpha_R=R\alpha.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
