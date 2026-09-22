# Signaling feedback

↑ **Parent:** [Signal transduction](signal-transduction-split.md)

[Signaling feedback](signaling-feedback.md) returns the effect of a downstream event to an earlier stage of [signal transduction](signal-transduction-split.md), closing a loop analogous to [feedback control](closed-loop-control.md). Trace the causal arrows: if an earlier relay activates a later relay and the later relay changes the earlier relay's activity, the return path closes the loop. [Negative feedback](negative-feedback.md) opposes the initiating change; [positive feedback](positive-feedback.md) reinforces it. [Signaling feedback](signaling-feedback.md) is a possible property of [signal transduction](signal-transduction-split.md), not a requirement of every pathway.

For a schematic example, let relay $A$ activate relay $B$. If $B$ inhibits $A$, increased $A$ eventually produces an opposing influence: [negative feedback](negative-feedback.md). If $B$ activates $A$, increased $A$ produces a reinforcing influence: [positive feedback](positive-feedback.md). These signs describe effects on activity, rather than the direction in which [molecules](molecule-split.md) travel. A closed loop containing two inhibitions can have [positive feedback](positive-feedback.md), because inhibiting an inhibitor reinforces the original change. The sign belongs to the whole loop.

<a id="image-negative-feedback-positive-feedback-and-an-incoherent-feedforward-loop"></a>
![](signaling-feedback-loops.png)

**[Figure 8](#image-negative-feedback-positive-feedback-and-an-incoherent-feedforward-loop). Negative feedback, positive feedback and an incoherent feedforward loop**. Original causal schematics. Arrows activate; flat-ended lines inhibit. The upper loops return from downstream relay $B$ to earlier relay $A$. In the lower [incoherent feedforward loop](incoherent-feedforward-loop.md), input $s$ drives both a fast activating branch $x$ and a slower inhibitory branch $a$; their contributions meet at readout $r$. There is no return arrow from $r$ to either branch or to $s$. Shapes and connections illustrate the distinction, rather than a measured pathway.

[Negative feedback](negative-feedback.md) can restrain excessive activation and help preserve a usable range of responses. [Positive feedback](positive-feedback.md) can support a decisive transition: Alberts and colleagues describe an [enzyme](enzyme-split.md) whose product increases its own activity. Such reinforcement can contribute to switchlike behavior, but a [positive feedback](positive-feedback.md) arrow alone does not prove [bistability](bistability.md). A different structure, an [incoherent feedforward loop](incoherent-feedforward-loop.md), sends opposing influences forward from the same input; inhibition there is not a downstream return. [General Principles of Cell Communication](molecular-biology-of-the-cell-4th-edition-by-bruce-alberts-and-others/general-principles-of-cell-communication.md) [Ma et al., Defining Network Topologies that Can Achieve Biochemical Adaptation, Cell 138 (2009), pp. 760–773: definitions on p. 764](https://cqb.pku.edu.cn/tanglab/pdf/78.pdf)

A worked [mathematical model](mathematical-model.md) shows why [negative feedback](negative-feedback.md) does not automatically produce complete [signaling adaptation](signaling-adaptation.md). Let $s$ be a fixed normalized input, $r$ a normalized response, $g\geq0$ a dimensionless [feedback gain](feedback-gain.md), and $\tau>0$ a [time constant](time-constant.md). Suppose response removal contributes $-r$ and a return proportional to the response contributes $-gr$. The [ordinary differential equation](ordinary-differential-equation.md) is

$$
\tau\frac{dr}{dt}=s-r-gr=s-(1+g)r.
$$

Setting the [derivative](derivative.md) to zero gives the [equilibrium point](equilibrium-point-of-a-dynamical-system.md) $r_*=s/(1+g)$. A displacement $\delta r=r-r_*$ obeys $\tau\,d(\delta r)/dt=-(1+g)\delta r$, so its decaying [exponential function](exponential-function.md) establishes [asymptotic stability](asymptotic-stability.md). For a unit input switched on at $t=0$, [initial condition](initial-condition.md) $r(0)=0$, $g=2$ and $\tau=1$ second,

$$
r(t)=\frac{1-e^{-3t/\tau}}{3},\qquad r(1\,\mathrm{s})\simeq0.316737,\qquad \lim_{t\to\infty}r(t)=\frac13.
$$

The [negative feedback](negative-feedback.md) reduces the eventual response from $1$ to $1/3$, but this response rises monotonically and never returns to its zero baseline. Attenuation and complete [signaling adaptation](signaling-adaptation.md) are different properties. This deliberately simple [mathematical model](mathematical-model.md) specifies no molecular pathway; [integral action](integral-action.md) provides a contrasting way to remove a lasting offset in a stable [feedback control](closed-loop-control.md) system. [Åström and Murray, Feedback Systems, Chapter 2: proportional and integral feedback](https://www.fbswiki.org/wiki/index.php/Feedback_Principles)

**Table of contents**

- [Negative feedback](negative-feedback.md)
  - [Delayed negative feedback model](delayed-negative-feedback-model.md)
    - [Delayed feedback characteristic root](delayed-feedback-characteristic-root.md)
  - [Chemotaxis feedback regulation](chemotaxis-feedback-regulation.md)
    - [Robust perfect adaptation](robust-perfect-adaptation.md)
    - [Receptor methylation](receptor-methylation.md)
    - [Tar receptor](tar-receptor.md)
    - [Chemotaxis feedback proteins](chemotaxis-feedback-proteins.md)
      - [CheW](chew.md)
      - [CheA](chea.md)
      - [CheB](cheb.md)
      - [CheR](cher.md)
      - [CheY](chey.md)
      - [CheZ](chez.md)
    - [Chemotaxis FRET assay](chemotaxis-fret-assay.md)
- [Positive feedback](positive-feedback.md)
  - [Double-negative feedback](double-negative-feedback.md)
  - [Saturating positive feedback](saturating-positive-feedback.md)
  - [Cell-cycle activation feedback](cell-cycle-activation-feedback.md)
    - [Cell-cycle hysteresis experiment](cell-cycle-hysteresis-experiment.md)
      - [Xenopus laevis egg extract](xenopus-laevis-egg-extract.md)
      - [Histone H1](histone-h1.md)
      - [Phosphorimager](phosphorimager.md)
    - [Cyclin-dependent kinase 1](cyclin-dependent-kinase-1.md)
      - [CDK1 phosphorylation state](cdk1-phosphorylation-state.md)
        - [CDK-activating kinase](cdk-activating-kinase.md)
        - [Myt1](myt1.md)
      - [Histone H1 kinase assay](histone-h1-kinase-assay.md)
      - [CDK1 activity and protein abundance](cdk1-activity-and-protein-abundance.md)
    - [Cyclin B](cyclin-b.md)
    - [Cdc25](cdc25.md)
    - [Wee1](wee1.md)

## ↑ Ancestors (3)

1. [Signal transduction](signal-transduction-split.md)
2. [Biology](biology-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Delayed negative feedback model](delayed-negative-feedback-model.md)
- [Metabotropic receptor](metabotropic-receptor.md)
- [Morphogen response threshold](morphogen-response-threshold.md)
- [Negative feedback](negative-feedback.md)
- [Positive feedback](positive-feedback.md)
- [Signal transduction](signal-transduction-split.md)
- [Signaling adaptation](signaling-adaptation.md)
- [Signaling feedback](signaling-feedback.md)
