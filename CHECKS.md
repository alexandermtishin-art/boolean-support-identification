# Reproducibility checkpoints

1. Download and unzip `IS_GITHUB_REPRODUCIBILITY_STAGING_2026-10-22.zip`.
2. Run from its `boolean-support-reproducibility/` directory:
   ```bash
   python adaptive_n5/verify_saved_tree.py
   python proofs/verify_nonadaptive_witnesses.py
   ```
3. Consult `proofs/THEOREM_C.md` for the asymptotic argument.
4. Consult `k6/verify_k6_independent.py` and `reports/K6_REPORT.md` for the exact input and status of the 147 capped-certificate tasks. Some historical pipelines require third-party datasets not redistributed here.

The exact five-variable adaptive minimum remains under computation. A depth-14 tree is an **upper bound**, not a proof that 14 is optimal. Historical solver logs are distinct from independently repeated checks.

The packaged archive is a staging snapshot; make no stronger reproducibility claims than the checked commands support.
