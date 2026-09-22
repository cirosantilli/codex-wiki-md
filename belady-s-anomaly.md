<h1 id="belady-s-anomaly">Bélády's anomaly</h1>

↑ **Parent:** [Page replacement](page-replacement.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bélády's_anomaly)

Increasing the number of [page frames](page-frame.md) can increase misses under a given [page replacement](page-replacement.md) policy on the same [page-reference trace](page-reference-trace.md). For [FIFO page replacement](fifo-page-replacement.md) on the displayed twelve-reference [sequence](sequence.md), an empty start with three [page frames](page-frame.md) gives nine misses, while an empty start with four gives ten. The larger run hits only at indices 5 and 6; it misses at 1–4 and 7–12. These are miss counts, not observed running times.[Belady's Anomaly aside, p. 5: the reference sequence and increasing capacity from three to four](operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/beyond-physical-memory-policies.md)

<a id="image-fifo-page-replacement-queue-states-and-cumulative-misses-four-page-frames-give-ten-misses-versus-nine-with-three"></a>
![](fifo-belady-anomaly-frame-comparison.png)

**[Figure 11](#image-fifo-page-replacement-queue-states-and-cumulative-misses-four-page-frames-give-ten-misses-versus-nine-with-three). FIFO page replacement queue states and cumulative misses: four page frames give ten misses versus nine with three**.

The explanation is visible before the final count. After access 6, the three-[page frame](page-frame.md) queue is $(4,1,2)$ and the four-[page frame](page-frame.md) queue is $(1,2,3,4)$, both oldest first. Loading [memory page](memory-page.md) 5 at access 7 removes [memory page](memory-page.md) 4 in the smaller run but [memory page](memory-page.md) 1 in the larger. Their resulting [resident sets](resident-set.md) are $\{1,2,5\}$ and $\{2,3,4,5\}$. The smaller [resident set](resident-set.md) is not a [subset](subset.md) of the larger: its next access to [memory page](memory-page.md) 1 hits while the larger run misses. Different earlier evictions create different histories; an extra [page frame](page-frame.md) is not simply an extra unchanged slot. [FIFO page replacement](fifo-page-replacement.md) can improve on other [sequences](sequence.md); the anomaly is an existence claim, not a claim that more [page frames](page-frame.md) usually hurt.

## ↑ Ancestors (6)

1. [Page replacement](page-replacement.md)
2. [Paging](paging.md)
3. [Virtual memory](virtual-memory-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)
