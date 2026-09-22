# Differential sky map monopole degeneracy

↑ **Parent:** [COBE DMR sky anisotropy experiment](cobe-dmr-sky-anisotropy-experiment.md)

An ideal differential measurement constrains two sky [temperatures](temperature-split.md) through $d_{ij}=T_i-T_j$. Represent every observed pair by a row of a [matrix](matrix.md) $A$, with $+1$ in column $i$, $-1$ in column $j$ and zeros elsewhere. Then $d=AT$ and $A\mathbf1=0$: adding any constant to the entire map changes no measurement. This [null space](kernel-of-a-linear-map-split.md) is the angular [angular monopole](angular-monopole.md) ambiguity, explaining why a directional comparison alone cannot measure the absolute [blackbody](blackbody.md) [temperature](temperature-split.md) established by [FIRAS](far-infrared-absolute-spectrophotometer.md).

For an original three-pixel example choose $T=(30,-10,-20)\,\mathrm{\mu K}$ relative to an unspecified mean. Measurements $d_{12}=40\,\mathrm{\mu K}$ and $d_{23}=10\,\mathrm{\mu K}$ determine the third difference $d_{31}=-50\,\mathrm{\mu K}$. The zero-mean condition recovers the chosen map, but adding $100\,\mathrm{\mu K}$ to every pixel gives identical differences. The closure sum $d_{12}+d_{23}+d_{31}=0$ checks consistency without establishing the mean.

More generally, the [graph](graph-split.md) joining measured pixel pairs must be a [connected graph](connected-graph.md). If $AT=0$, each edge forces equal endpoint [temperatures](temperature-split.md); a path propagates that equality throughout each connected component. Thus a connected observation [graph](graph-split.md) leaves exactly one undetermined constant, whereas disconnected coverage leaves one per component. Fixing the mean makes an ideal connected reconstruction unique; real [noise](noise-signal-processing.md) calls for [least-squares solution](least-squares-solution-of-a-linear-inverse-problem.md) fitting and uncertainty analysis.

The figure chooses a [cosmic microwave background quadrupole](cosmic-microwave-background-quadrupole.md) sky $T(\theta)=Q P_2(\cos\theta)$, with $Q=30\,\mathrm{\mu K}$ and [Legendre polynomial](legendre-polynomial.md) $P_2(u)=(3u^2-1)/2$. On a great-circle scan, with $\phi$ measured from the chosen symmetry axis and ideal beams separated by $\alpha=60^\circ$,

$$
d(\phi)=T(\phi)-T(\phi+\alpha)
=\frac{3Q}{2}\sin\alpha\,\sin(2\phi+\alpha).
$$

Expanding $\cos^2\phi=(1+\cos2\phi)/2$ proves the formula; its peak magnitude is $45\sqrt3/2\simeq38.9711\,\mathrm{\mu K}$. A constant sky gives zero. This deliberately restricted scan also misses some angular patterns, so rejecting the [angular monopole](angular-monopole.md) is not a proof of complete sky reconstruction. Broad, overlapping coverage supplies the missing constraints; finite [antenna beam patterns](antenna-beam-pattern.md) additionally smooth small angular features.

## ↑ Ancestors (8)

1. [COBE DMR sky anisotropy experiment](cobe-dmr-sky-anisotropy-experiment.md)
2. [Differential Microwave Radiometer](differential-microwave-radiometer.md)
3. [Cosmic microwave background anisotropy](cosmic-microwave-background-anisotropy-split.md)
4. [Cosmic microwave background](cosmic-microwave-background-split.md)
5. [Cosmology](cosmology-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
