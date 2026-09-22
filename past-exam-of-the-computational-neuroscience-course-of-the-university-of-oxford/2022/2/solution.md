<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**I would combine visually calibrated [continuous attractor networks](../../../continuous-attractor-network.md) with [competitive learning](../../../competitive-learning.md), while keeping heading, self-location and the viewed location as distinct variables.** A [head direction cell](../../../head-direction-cell.md) reports orientation, a [place cell](../../../place-cell.md) reports self-location, and a [spatial view cell](../../../spatial-view-cell.md) reports a viewed part of the external world. A model that predicts all three from the same retinal image without controlling eye position and body position risks explaining a sampling correlation rather than the neural code.

For heading, let $r_i$ be rates in a ring indexed by preferred directions $\theta_i$. A concrete rate model is

$$
\tau\dot r_i=-r_i+\phi\!\left(\sum_jJ_{ij}r_j+I_i^{\rm visual}+I_i^{\rm motion}-b\right).
$$

Choose local excitation and broad inhibition strengths so that one localized activity bump is stable; a bump is not guaranteed for arbitrary connection strengths. An asymmetric component driven by angular velocity shifts the bump, implementing [path integration](../../../path-integration.md). An approximate decoded angle is $\widehat\theta=\arg\sum_i r_i e^{\mathrm i\theta_i}$. Its periodic representation avoids an artificial discontinuity between $359^\circ$ and $0^\circ$. During active turns, correlated landmark features and the currently active direction population modify visual afferents by bounded [Hebbian learning](../../../hebbian-learning.md). Repeated encounters calibrate visual inputs to the internal angular state. In the absence of external cues, recurrent activity can persist while velocity noise produces drift; the landmarks correct that drift rather than having to generate every moment of activity.

This separates a model assumption from a developmental explanation. Prespecifying a ring with a moving bump assumes part of the organization; it does not show that vision constructs the ring. A stronger developmental model should start from the claimed immature connectivity and demonstrate emergence of stable tuning under realistic self-motion. The observed [head direction cell](../../../head-direction-cell.md) system is constrained by cue-card experiments: rats explored a cylindrical enclosure, and rotating a prominent wall card rotated preferred firing directions with much less change in tuning shape. Card removal could change the angular anchor without eliminating directional firing. These results motivate learned landmark anchoring plus internally maintained heading, rather than a purely retinal feature detector.[Abstract; pp. 436–447, cue-card rotation and removal](../../../head-direction-cells-recorded-from-the-postsubiculum-in-freely-moving-rats-ii-effects-of-environmental-manipulations-by-jeffrey-s-taube-and-others.md)

For [place cells](../../../place-cell.md), use converging visual-landmark features, boundary geometry and a self-motion estimate of position. A [winner-take-all network](../../../winner-take-all-network.md) can learn prototypes of this conjunctive input. For normalized input $z$ and winning unit $k$, a simple [competitive learning](../../../competitive-learning.md) rule is $\Delta w_k=\eta(z-w_k)$ followed by any required [synaptic normalization](../../../synaptic-normalization.md). Similar conjunctions recur around a location, whereas their component retinal appearances vary with heading. Multiple headings and eye positions must therefore be sampled at each location. Coupling these learned visual responses to a two-dimensional [continuous attractor network](../../../continuous-attractor-network.md) or another self-motion state estimator lets vision calibrate a position representation that remains usable during brief cue loss. One must not silently supply correct world-position labels to an allegedly unsupervised developmental system: simulated position is a validation variable, and any internal position estimate needs a specified sensory origin.

For [spatial view cells](../../../spatial-view-cell.md), the target variable is different. In a planar illustration, if the animal is at $p$, head angle is $\theta_h$ and eye angle relative to the head is $\theta_e$, a viewed point lies on

$$
q=p+\lambda\begin{pmatrix}\cos(\theta_h+\theta_e)\\\sin(\theta_h+\theta_e)\end{pmatrix},\qquad\lambda>0.
$$

A depth estimate or intersection with an inferred scene surface is needed to determine $\lambda$. Combining visual features, eye-position signals, heading and location can let [competitive learning](../../../competitive-learning.md) associate multiple views of the same world location. The formula specifies the geometric computation to be learned; it is not evidence that a [neuron](../../../neuron-split.md) literally performs trigonometry. For example, facing east with a $30^\circ$ leftward gaze and facing $30^\circ$ north of east with straight-ahead gaze can look toward the same point from the same position, despite different head directions. This distinction is experimentally important: recordings in freely walking macaques, with eye-position measurements, found [hippocampal](../../../hippocampus.md) responses related to looked-at locations rather than simply to the monkey's place or head direction.[Abstract; pp. 1789–1794, active locomotion, eye position and allocentric spatial-view responses](../../../spatial-view-cells-in-the-primate-hippocampus-by-edmund-t-rolls-and-others.md)

**The main outstanding challenges are developmental causation, ambiguous sensory input and generalization across conditions.** First, spatial circuitry need not wait for patterned vision: recordings before and after eye opening show an early directional signal, with immature stability. Therefore vision can calibrate or stabilize a partially organized circuit, and a theory claiming wholly visual construction must account for that developmental timing.[Abstract; pp. 479–483, recordings before and after eye opening](../../../the-development-of-the-head-direction-system-before-eye-opening-in-the-rat-by-hui-min-tan-and-others.md) Second, visually similar corridors can correspond to different positions, while one position can produce very different images. Cue conflict, darkness, passive transport and novel environments separate landmark anchoring, self-motion updating and [hippocampal remapping](../../../hippocampal-remapping.md). Third, retinal direction is not world direction: eye movements, head pitch, depth, occlusion and independently moving objects challenge an [allocentric spatial representation](../../../allocentric-spatial-representation.md). Finally, the model must explain species and task differences without assuming that rodent [place cells](../../../place-cell.md) and primate [spatial view cells](../../../spatial-view-cell.md) exhaust all spatial responses.

I would assess held-out positions, headings and gaze combinations, compare predicted tuning and drift against recordings, and ablate the visual-learning and self-motion components separately. A successful model should predict how tuning changes after specific experience and cue manipulations, not merely fit a familiar trajectory. **Visually guided development is therefore a multisensory learning problem with an experimentally constrained internal spatial dynamics.**

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2022](../../2022-split.md)
3. [Past exam of the computational neuroscience course of the University of Oxford](../../split.md)
4. [Computational neuroscience course of the University of Oxford](../../../computational-neuroscience-course-of-the-university-of-oxford.md)
5. [Year 3 of the psychology (experimental) course of the University of Oxford](../../../year-3-of-the-psychology-experimental-course-of-the-university-of-oxford.md)
6. [Psychology (experimental) course of the University of Oxford](../../../psychology-experimental-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
