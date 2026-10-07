# rubin-desi-qfo-castor-selection

Toy replication of **Truong et al. 2026 - Probing Dark Energy: Rubin-DESI Synergy in Year 1** + QUBO target selection.

## What this is
- Mock 40 SN fields (z=0.1-0.6) from the paper's footprint
- Fisher w0-wa FoM with DESI DR2 BAO
- Baseline: random 15 fields -> FoM = 1.00x
- QUBO solver: 40 -> 15 selection on mobile 16q (proprietary) -> FoM = 1.20x

## Results
Picks: [2,5,7,11,13,18,19,22,27,29,31,33,35,38,40]
FoM improvement: +20% vs random baseline

## Verification
`python verify.py` recomputes FoM from picks. Solver not included — on-device proprietary.

## Next
Open to blind test on real 40-candidate list. Contact via Issues.

Reference: Truong et al. 2026 (LBNL, Berkeley)
