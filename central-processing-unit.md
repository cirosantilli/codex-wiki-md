# Central processing unit

↑ **Parent:** [Computer science](computer-science-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Central_processing_unit)

The processor executing a program's instructions. In [polled input-output](polled-input-output.md) the [CPU](central-processing-unit.md) explicitly checks status; in [interrupt-driven input-output](interrupt-driven-input-output.md) it enters an [interrupt handler](interrupt-handler.md); in [DMA](direct-memory-access.md) it delegates payload movement while retaining setup and completion work.

**Table of contents**

- [Out-of-order execution](out-of-order-execution.md)
  - [Reorder buffer](reorder-buffer.md)
    - [Instruction retirement](instruction-retirement.md)
  - [Common data bus](common-data-bus.md)
  - [Register renaming](register-renaming.md)
    - [Physical register](physical-register.md)
  - [Reservation station](reservation-station.md)
- [Multicore processor](multicore-processor.md)
  - [CPU core](cpu-core.md)
- [Speculative execution](speculative-execution.md)
  - [Branch prediction](branch-prediction.md)
- [Instruction pipelining](instruction-pipelining.md)
  - [Data hazard](data-hazard.md)
    - [Read-after-write hazard](read-after-write-hazard.md)
      - [Register forwarding](register-forwarding.md)
  - [Pipeline stall](pipeline-stall.md)
  - [Pipeline register](pipeline-register.md)
  - [In-order pipeline](in-order-pipeline.md)
- [Datapath](datapath.md)
  - [Functional unit](functional-unit.md)
- [Arithmetic logic unit](arithmetic-logic-unit.md)
- [Busy waiting](busy-waiting.md)
- [Processor register](processor-register.md)
  - [Processor condition flag](processor-condition-flag.md)
    - [Zero flag](zero-flag.md)
  - [Carry flag](carry-flag.md)
    - [Subtract with carry](subtract-with-carry.md)
    - [Add with carry](add-with-carry.md)
  - [Register file](register-file.md)
    - [Write-suppression destination](write-suppression-destination.md)
    - [MIPS zero register](mips-zero-register.md)
    - [Spilling a register](spilling-a-register.md)
  - [Stack pointer](stack-pointer.md)

## ↑ Ancestors (2)

1. [Computer science](computer-science-split.md)
2. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Machine code](machine-code.md)
