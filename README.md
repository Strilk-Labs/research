# STRILK security research

STRILK works on application security, DevSecOps, security assessments and remediation. This repository brings together the laboratory's research projects and planned studies.

We study Windows internals, memory safety, virtualization and binary analysis, and develop tools for process analysis, executable-format validation and memory-integrity monitoring. The aim is to turn technical findings into useful detection, corrective changes and regression checks.

## Projects

| Area | Repository |
| --- | --- |
| Process metadata and integrity | [PEBWatch](https://github.com/Strilk-Labs/PEBWatch) |
| PE analysis and detection signals | [CRTScan](https://github.com/Strilk-Labs/CRTScan) |
| Virtualization and memory isolation | [HvShield](https://github.com/Strilk-Labs/HvShield) |
| C++ object integrity | [VTCheck](https://github.com/Strilk-Labs/VTCheck) |
| Binary-analysis assistance | [IDAVtableRecovery](https://github.com/Strilk-Labs/IDAVtableRecovery) |

These are research prototypes with documented limitations. The proposed Windows research sequence is in [ROADMAP.md](ROADMAP.md).

## How we work

**Scope → validate → fix → verify.** Studies identify the source revision, environment and authorized scope. Findings are reviewed against observed evidence, corrective changes and validation results. Source analysis, compilation and runtime testing are recorded separately.

Research follows [STRILK's laboratory scope](https://strilk.com/laboratoire). Publications document the result, its limitations and the applicable [disclosure status](https://strilk.com/divulgation-responsable).

[Website](https://strilk.com/) · [Services](https://strilk.com/services) · [Contact](mailto:contact@strilk.com)
