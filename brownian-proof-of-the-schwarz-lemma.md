# Brownian proof of the Schwarz lemma

↑ **Parent:** [Schwarz lemma](schwarz-lemma.md)

For a [holomorphic function](holomorphic-function-split.md) on the unit disk fixing zero, $g(z)=f(z)/z$ has a removable singularity at zero and a bounded holomorphic extension. A bounded holomorphic function evaluated along [planar Brownian motion](planar-brownian-motion.md) is a bounded stopped [martingale](martingale-split.md) before domain exit. Stop at the first exit from a concentric radius-$r$ disk with $|z|<r<1$. [Optional stopping](optional-sampling-theorem-for-a-supermartingale.md) gives $g(z)=\mathbb E_z g(Z_{T_r})$, hence $|g(z)|\leq1/r$. Letting $r$ increase to one proves the displayed bound.

If $|g(z_0)|=1$ at a nonzero point, put $c=g(z_0)$. The same expectation identity forces $\operatorname{Re}(\overline c\,g(Z_{T_r}))=1$ almost surely. The exit density is strictly positive on every boundary arc by the [Poisson kernel for the unit disk](poisson-kernel-for-the-unit-disk.md), and $g$ is continuous there, so $g=c$ on that circle. The expectation identity for every starting point inside it then gives $g=c$ throughout that smaller disk. Letting $r$ increase to one shows $f(z)=cz$ on the full disk, with $|c|=1$. This derives both the inequality and its rigidity using Brownian harmonic measure.

## ↑ Ancestors (5)

1. [Schwarz lemma](schwarz-lemma.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford/2011/3/b/ii/solution.md)
