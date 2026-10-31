# External Cryptographic Anchor Record: Prospective Inflation Surveillance Pipeline (Priority 2)

**Project:** `prospective_inflation_pipeline_priority2`  
**Git Release Tag:** `priority2-accepted-prototype-20261031-v2`  
**Remote Tag URL:** [https://github.com/Dips7/nepal-macro-inflation-research/releases/tag/priority2-accepted-prototype-20261031-v2](https://github.com/Dips7/nepal-macro-inflation-research/releases/tag/priority2-accepted-prototype-20261031-v2)  
**External Anchoring Posture:** **`EXTERNAL PENDING — OTS SUBMITTED / REMOTE TAG PUBLISHED`**  
**Pipeline Classification:** **`PROTOTYPE_ONLY_NOT_READY_FOR_LIVE_ISSUANCE`**  
**Record Generation Timestamp:** `2026-10-31T13:40:00Z`  
**Release Version:** `v2` (Self-Contained Release; supersedes `v1` while preserving full `v1` history)

---

## 1. Release Evolution & Self-Contained Architecture

- **Version 2 (`priority2-accepted-prototype-20261031-v2` - Current Authoritative Release):**
  - **Self-Contained Data Packaging:** Bundled all three required historical dataset dependencies under `prospective_inflation_pipeline_priority2/data/` (~5.5 MB total): `core.csv` (801 rows), `predictors.csv` (801 rows), and `forecasts.csv` (26,280 rows).
  - **Data Integrity Manifest:** Pinned in `data/DATA_MANIFEST.json` with SHA-256 digests, row counts, and provenance.
  - **Zero External Dependencies:** Verified that a clean clone outside the author workstation (with zero access to local untracked parent directories) passes all 7 verification stages and all 63 unit and synthetic lifecycle tests with exit code 0.
  - **Archive Sealing:** Seals 43 manifest-covered underlying files in `archive/v5_selfcontained_prototype` (plus manifest + 2 receipts = 46 files on disk).

- **Version 1 (`priority2-accepted-prototype-20261031` - Historical Baseline):**
  - Tag Object ID: `c50bde96674fccc48ac666628bd37e6169079153` -> Commit `68ca9c40e0e9a7c7e52011388cadbffd8962c299`.
  - Prototype verified locally; required external dataset path at `Revamped/` parent directory.
  - Sealed in `archive/v4_accepted_prototype` (39 files). Preserved completely untouched.

---

## 2. Git Release Identifiers (Git SHA-1 Object IDs)

### Current Release (v2):
- **Annotated Tag Object ID:** `2561369f0a5799de4fef03a1256a5d2fb26ee7ea`
- **Release Commit ID (Peeled):** `da25fa6dccb7603003b7c1c382f384489dbb986e`
- **Root Tree ID:** `3d71f29a527076d4a269801510656348b65018d6`
- **Remote Upstream:** `https://github.com/Dips7/nepal-macro-inflation-research.git`
- **Remote Ref:** `refs/tags/priority2-accepted-prototype-20261031-v2`
- **Remote Branch:** `refs/heads/release/priority2-v2`

### Historical Release (v1):
- **Annotated Tag Object ID:** `c50bde96674fccc48ac666628bd37e6169079153`
- **Release Commit ID (Peeled):** `68ca9c40e0e9a7c7e52011388cadbffd8962c299`
- **Root Tree ID:** `86db477fa908953b8ff73703a9162afc10194a9c`
- **Remote Ref:** `refs/tags/priority2-accepted-prototype-20261031`

---

## 3. Cryptographic Anchor Manifest & Integrity Checksums (SHA-256)

| Target Name | Canonical File Path | SHA-256 Digest |
| :--- | :--- | :--- |
| **Protected Baseline Manifest (510 files)** | `thesis_next_work_20261030/priority0/verification/SUBMISSION_PACKAGES_BASELINE.json` | `b3062751e5b016ce6ce92cb949921cc4a5e6315ae7ca7975ede17c9b70b14546` |
| **Archive Manifest (v5 - Self-Contained)** | `prospective_inflation_pipeline_priority2/archive/v5_selfcontained_prototype/ARCHIVE_MANIFEST.json` | `6b51983d4099d928c7976d64b52475b9e7a4bb700f33914d214378763d5cff9b` |
| **Bundled Data Manifest** | `prospective_inflation_pipeline_priority2/data/DATA_MANIFEST.json` | `bda92ba3b25fd76098917d175febd990f9d61ff8600ba480b3b874dc1fda0969` |
| **Master Verifier Script** | `prospective_inflation_pipeline_priority2/run_verification.py` | `c56dce3a93498f9f6186a1b463d6f64e08410cf4ea9cfeecd0ba274153bb658a` |
| **Canonical Verification Report** | `prospective_inflation_pipeline_priority2/reports/VERIFICATION_REPORT.json` | `eb3ba3c747b85b37c889bf4361feee3d84b55c655507207293fa71ab4ba0b918` |
| **Audit Receipt (JSON)** | `prospective_inflation_pipeline_priority2/reports/AUDIT_RECEIPT.json` | `a2058d46b0895eff94d21b72d54575aed804f360eeaf29875f9d345170bbd6e9` |
| **Audit Receipt (Markdown)** | `prospective_inflation_pipeline_priority2/reports/AUDIT_RECEIPT.md` | `abbd9d8ae440b8fa6d38e6011eec1915222337318aa21c89c8125b5cd14b6bc8` |
| **Historical Archive Manifest (v4)** | `prospective_inflation_pipeline_priority2/archive/v4_accepted_prototype/ARCHIVE_MANIFEST.json` | `5c6ac8728f61c7077cc73b1ce26528ecbcf4d36f42756ba9cdbb3c0029933c76` |

---

## 4. OpenTimestamps External Proof Details

### Current Release (v2) Proofs:
- **`tag_object_sha.txt` (`2561369f…`):**
  - Target SHA-256: `6101749d7861ec2399f652b1fe36bd15d8c4dbadb2caad458eab8e14cbb60dba`
  - Proof File: `tag_object_sha.txt.ots`
  - Status: Submitted & Pending Bitcoin Block Confirmation across 3 calendar pools (`btc.calendar.catallaxy.com`, `bob.btc.calendar.opentimestamps.org`, `finney.calendar.eternitywall.com`).
- **`commit_sha.txt` (`da25fa6d…`):**
  - Proof File: `commit_sha.txt.ots` (Pending confirmation)
- **`ARCHIVE_MANIFEST.json` (`6b51983d…`):**
  - Proof File: `ARCHIVE_MANIFEST.json.ots` (Pending confirmation)
- **`DATA_MANIFEST.json` (`bda92ba3…`):**
  - Proof File: `DATA_MANIFEST.json.ots` (Pending confirmation)

### Historical Release (v1) Preserved Proofs:
- **`tag_object_sha_v1.txt` (`c50bde96…`):** Proof `tag_object_sha_v1.txt.ots`
- **`commit_sha_v1.txt` (`68ca9c40…`):** Proof `commit_sha_v1.txt.ots`
- **`ARCHIVE_MANIFEST_v4.json` (`5c6ac872…`):** Proof `ARCHIVE_MANIFEST_v4.json.ots`

---

## 5. Verification & Reproduction for Independent Auditors

```bash
# 1. Clone repository from GitHub (requires authenticated access to private repo)
git clone https://github.com/Dips7/nepal-macro-inflation-research.git audit-clone
cd audit-clone

# 2. Fetch and checkout the exact self-contained v2 release tag
git fetch origin tag priority2-accepted-prototype-20261031-v2
git checkout refs/tags/priority2-accepted-prototype-20261031-v2

# 3. Verify git object IDs
test "$(git rev-parse refs/tags/priority2-accepted-prototype-20261031-v2)" = "2561369f0a5799de4fef03a1256a5d2fb26ee7ea"
test "$(git rev-parse refs/tags/priority2-accepted-prototype-20261031-v2^{commit})" = "da25fa6dccb7603003b7c1c382f384489dbb986e"

# 4. Verify OpenTimestamps proof against tag object SHA
ots --version  # requires opentimestamps-client >= 0.7.2
printf '%s\n' 2561369f0a5799de4fef03a1256a5d2fb26ee7ea > tag_object_sha.txt
ots verify -f tag_object_sha.txt tag_object_sha.txt.ots

# 5. Run full 7-stage master verifier (zero external dependencies required)
cd prospective_inflation_pipeline_priority2
python3 run_verification.py
# Assert output: 7 of 7 stages passed, 63 tests, 0 failures, 0 errors, 0 skips, exit 0
```

---

## 6. Scope Boundaries & Mandatory Caveats

- **Prototype Status:** The pipeline is strictly in status `PROTOTYPE_ONLY_NOT_READY_FOR_LIVE_ISSUANCE`. Live mutations (`issue`, `ingest-outcome`, `score`, and direct storage-layer writes) are fail-closed gated (`LiveIssuanceGatedError`).
- **Live Ledgers Empty:** All 4 production ledgers (`ledgers/*.csv`) contain exactly 0 data rows and remain in genesis checkpoint state.
- **Prospective Evidence Caveat:** **`PROSPECTIVE_EVIDENCE: none yet`**. All verification passes reflect synthetic simulation and architectural verification, not authenticated out-of-sample live performance. Real evidence accumulates only prospectively after launch authorization.
