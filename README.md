# TruthChain Auditor – Level-1 DFD

```mermaid
flowchart LR
  User[User]
  P1((User Upload))
  P2((Pre-processing))
  P3((AI Analysis))
  P4((Result Hash Generation))
  P5((Blockchain Storage))
  P6((Dashboard Rendering))
  P7((Consensus Editing))
  DS1[(Blockchain Ledger)]

  User -->|Media File| P1
  P1 -->|Raw Media Data| P2
  P2 -->|Structured Data| P3
  P3 -->|Audit Scores| P4
  P4 -->|Hash + Metadata| P5
  P5 -->|Ledger Entry| DS1
  DS1 -->|Verified Data| P6
  P6 -->|Audit Report| User
  P6 -->|Community Suggestions| P7
  P7 -->|Edits + Hash| P5
