# STRILK Windows research roadmap

Proposed sequence, prepared 26 September 2026. No completion dates or research results are implied.

## 1 Establish the evidence baseline

For PEBWatch and CRTScan, document a source revision, prerequisites, compiler/SDK versions, an isolated Windows lab environment and the result of a clean build. Record limitations directly in each README. Keep the original authorship and MIT license notices.

**Deliverable:** an accurate build/status record that another researcher can evaluate. A build result alone does not establish detection quality or runtime stability.

## 2 Publish a PEBWatch study

Investigate how normal process activity and Windows-version differences affect the prototype's observations. Use researcher-owned processes and lab observations. Explain expected changes, ambiguous cases and false positives. Record actual results before writing the conclusions.

**Deliverable:** a dated technical note linked to the tested revision, an environment matrix and a set of regression checks based on observed benign cases.

## 3 Publish a parser correctness study

Review the PE-reading code used by the defensive tools. Focus on input validation, size arithmetic, error handling and predictable rejection of invalid input. Keep evaluation within owned code and controlled local fixtures.

**Deliverable:** a reviewed corrective change, relevant regression evidence, and a write-up explaining the cause and limitations. Do not describe a third-party library as vulnerable without a verified finding and the appropriate disclosure process.

## 4 Extend into Windows driver correctness

Use owned or expressly authorized driver source to study memory lifetime, interface contracts and error handling. Document the analysis toolchain and separate static findings from runtime observations. Current Microsoft guidance names CodeQL for static driver analysis and Driver Verifier for dynamic testing; SDV is no longer supported in recent WDKs.

**Deliverable:** a source-review and validation report with exact version information. Runtime work requires a suitable test machine or VM and a separately defined lab procedure. This roadmap does not supply an exploit-development workflow or direct testing against third-party deployments.

## 5 Document HvShield honestly

Publish a design review and a status matrix for the early HvShield source snapshot. The README already calls out unfinished implementation. Establish the prerequisites for safe laboratory evaluation before representing the project as a functioning or production-ready monitor.

**Deliverable:** a design/status note tied to a revision, with the next bounded engineering task identified. Later results should be added only after actual evaluation.

## Supporting tools

VTCheck and IDAVtableRecovery support the same Windows/binary-analysis direction. Their documented compiler, ABI and heuristic limitations should remain visible. They can be incorporated into studies when relevant; there is no need to create additional repository names solely to enlarge the portfolio.

## Sources

- [Microsoft driver verification tools](https://learn.microsoft.com/en-us/windows-hardware/drivers/devtest/static-and-dynamic-verification-tools)
- [STRILK laboratory scope](https://strilk.com/laboratoire)
- [Research projects](https://github.com/Strilk-Labs)
