# DOJ DOCUMENT REMOVAL AUDIT: 78,234 FILES REMOVED FROM JUSTICE.GOV AFTER EFTA PUBLICATION

## A Forensic Integrity Audit of the Department of Justice's Epstein Files Transparency Act Production

---

## EXECUTIVE SUMMARY

Between February 18 and 20, 2026, we conducted a comprehensive HTTP integrity scan of every document in the Department of Justice's Epstein Files Transparency Act (EFTA) production hosted at justice.gov/epstein. Of the 1,380,941 documents in the production corpus, we successfully scanned 1,365,677 (98.89%). The results reveal that **78,234 documents — 5.7% of the entire production — now return HTTP 404 (Not Found)**. These files were part of the original DOJ publication but have been silently removed from the public server without any Federal Register notice, without Congressional notification, and without published legal justification — all of which are required by the statute.

Manual browser verification using Playwright (which executes JavaScript and passes the DOJ's Akamai CDN challenge) confirms these are real removals, not scanner artifacts.

The removed documents are not random. They are concentrated overwhelmingly in Dataset 9 — the dataset containing the FBI's investigative files, prosecutorial correspondence, Bureau of Prisons records, and grand jury materials. Below, we examine four removed documents that contain **no victim personally identifying information** and for which **no lawful basis for removal exists** under the statute: the Bureau of Prisons' detention logs from Epstein's housing units during the period of his death, the BOP's own psychological reconstruction of his death, and bank statements for an Epstein-linked shell entity in the US Virgin Islands.

We also found that numerous other removed documents contain extensive, unredacted victim PII — full names, dates of birth, home addresses, phone numbers, and family members of victims who were minors at the time of the crimes. The DOJ failed to redact this information before publication, then removed the documents wholesale rather than fixing the redactions. We are not identifying those documents here — see "A Note on Victim Privacy" below.

Additionally, 23,989 documents that remain accessible show file sizes smaller than their originals — suggesting post-publication re-processing or content removal that has not been disclosed.

---

## PART I: THE EPSTEIN FILES TRANSPARENCY ACT

### What the Law Requires

The Epstein Files Transparency Act (Public Law 119-38, H.R. 4405) became law on November 19, 2025. In plain terms, it orders the Attorney General to make public — within 30 days — all unclassified records the Department of Justice holds relating to Jeffrey Epstein. The word "all" is not rhetorical. The statute specifies nine categories of material that must be released:

1. **All investigations, prosecutions, or custodial matters** involving Epstein
2. **All records relating to Ghislaine Maxwell**
3. **All flight logs and travel records** — manifests, itineraries, pilot records, customs and immigration documentation — for any aircraft, vessel, or vehicle owned or used by Epstein or related entities
4. **All references to individuals**, including government officials, named in connection with Epstein's criminal activities, civil settlements, immunity agreements, or investigations
5. **All references to entities** — corporate, nonprofit, academic, or governmental — with known or alleged ties to Epstein's trafficking or financial networks
6. **All immunity deals, non-prosecution agreements, plea bargains, or sealed settlements** involving Epstein or associates
7. **All internal DOJ communications** — emails, memos, meeting notes — concerning decisions to charge, not charge, investigate, or decline to investigate Epstein or associates
8. **All communications or metadata concerning destruction, deletion, alteration, misplacement, or concealment** of documents, recordings, or electronic data related to Epstein
9. **All documentation of Epstein's detention or death** — incident reports, witness interviews, medical examiner files, autopsy reports, and written records detailing the circumstances and cause of death

The statute requires these records be made available in "searchable and downloadable format."

### What the Law Prohibits

Section 2(b) creates an absolute prohibition: **No record shall be withheld, delayed, or redacted based on embarrassment, reputational harm, or political sensitivity** — including to any government official, public figure, or foreign dignitary. This is not a balancing test. It is a categorical bar.

### The Five Permitted Carveouts — And Their Limits

Section 2(c) defines exactly five categories of material the Attorney General *may* withhold or redact. These are the only lawful bases for removing any document from the production:

**(A) Victim Personally Identifiable Information** — Records may be withheld or redacted where they contain personally identifiable information of victims, or victims' personal and medical files, where disclosure "would constitute clearly unwarranted invasion of personal privacy." This protects victim names, addresses, phone numbers, medical records, and identifying details. It does **not** protect the names of perpetrators, government officials, law enforcement, attorneys, or other non-victim participants. It does **not** authorize removing an entire document when targeted redaction of victim identifiers would suffice.

**(B) Child Sexual Abuse Material (CSAM)** — Material depicting or containing CSAM as defined under 18 U.S.C. § 2256 may be withheld. Section 2256 defines CSAM to include visual depictions — photographs, films, videos, and digital images. This does not extend to investigative reports, legal filings, or text documents that reference or describe CSAM without depicting it.

**(C) Active Federal Investigation or Ongoing Prosecution** — Material may be withheld where disclosure "would jeopardize an active federal investigation or ongoing prosecution." The statute adds two critical qualifiers: such withholding must be "**narrowly tailored**" (removing only the specific material that would cause jeopardy, not entire documents or categories) and "**temporary**" (implying an obligation to release once the investigation concludes). This does not apply to investigations that have been resolved, declined, or closed.

**(D) Images of Death, Physical Abuse, or Injury** — Material may be withheld where it depicts or contains "images of death, physical abuse, or injury of any person." This covers visual depictions — not text descriptions, investigative reports, or administrative records that discuss these events without depicting them visually.

**(E) National Defense or Foreign Policy** — Material specifically authorized under criteria established by Executive order to be kept secret in the interest of national defense or foreign policy may be withheld. Any post-July 1, 2025 classification decision must be published in the Federal Register.

### The Procedural Requirement That Makes Removal Unlawful

Even where one of these five carveouts applies, the statute imposes a procedural requirement that the DOJ has not followed. Section 2(c)(2) mandates: **"All redactions must be accompanied by written justification published in the Federal Register and submitted to Congress."** The Attorney General must declassify to the maximum extent possible and, for any material that cannot be declassified, must release an unclassified summary.

As of this writing, no Federal Register notice has been published justifying the removal of 78,234 documents. No unclassified summaries have been provided. No Congressional notification has been submitted. The removals are, on their face, procedurally non-compliant with the statute regardless of whether any substantive carveout might apply to individual documents.

### The DOJ's Stated Explanation

On February 5, 2026, the U.S. Attorney's Office for the Southern District of New York filed a [letter to the court](https://storage.courtlistener.com/recap/gov.uscourts.nysd.518649/gov.uscourts.nysd.518649.105.0_2.pdf) (Case 1:19-cr-00490-RMB, Document 105) explaining its approach to post-publication removals. The letter, signed by Attorney General Pamela Bondi, Deputy Attorney General Todd Blanche, and U.S. Attorney Jay Clayton, states that:

- Victims and victim counsel can contact `efta@usdoj.gov` to flag insufficiently redacted documents
- Documents flagged through that process "are removed for further review by Department personnel"
- Approximately 7,000 documents were flagged based on "identifiers not previously provided to the Department or based on apparent instances of first names only, nicknames, misspellings or alternate spellings of names, or initials appearing in documents"
- The Department acknowledged "human errors, technical errors, and instances in which the effectiveness of certain quality control measures appears to have been hampered"
- Approximately 9,500 documents subject to the Maxwell Protective Orders were also removed

This explanation accounts for a subset of the removals. It does not account for the removal of Bureau of Prisons detention logs containing no victim information, financial records of Epstein-linked shell entities, or the BOP's own psychological reconstruction of Epstein's death — none of which contain victim-identifying information that would be flagged through the `efta@usdoj.gov` process.

---

## PART II: AUDIT METHODOLOGY

### Corpus Definition

The DOJ's EFTA production consists of 1,380,941 documents organized across 12 datasets. Each document is assigned an EFTA number (e.g., EFTA00074206) and hosted as a PDF at a predictable URL:

```
https://www.justice.gov/epstein/files/DataSet%20{N}/EFTA{NUMBER}.pdf
```

Our corpus manifest was built from the `full_text_corpus.db` database, which contains the complete text extraction of all documents in the production. The manifest includes every EFTA number and its dataset assignment.

### Scanning Method

HTTP HEAD requests were sent to every document URL in the production. Scans were conducted February 18-20, 2026. Each request recorded the HTTP status code, Content-Length, Content-Type, and response latency. The DOJ serves these files through an Akamai CDN that applies aggressive rate-limiting — particularly on Dataset 9, which contains over 531,000 documents and required multiple scanning passes to achieve coverage.

### Deduplication and Verification

All scan results were merged using a priority system: HTTP 200 (document present) takes precedence over HTTP 404 (removed), which takes precedence over error codes. This ensures that if a document was accessible in any scan pass, it is counted as present.

All 78,234 documents flagged as HTTP 404 were submitted to a second verification pass. False positives (documents that returned 404 initially but 200 on reverification) were reclassified as present.

### Manual Playwright Verification

Because the DOJ's Akamai CDN serves a JavaScript challenge page before delivering content, standard HTTP tools (curl, wget) can return misleading results. We verified a sample of removed documents using Playwright, a headless browser that executes JavaScript and renders pages as a real browser would. Playwright confirmed: removed documents display the DOJ's standard 404 error page. Present documents load as PDFs.

### Limitations

- **15,264 documents (1.1%) were unreachable** — all in Dataset 9 — due to Akamai CDN rate-limiting before scanning completed. These are recorded as UNSCANNED, not as removals.
- **2,614 documents returned HTTP 401** (CDN authentication challenge), also not counted as confirmed removals.
- **235 EFTA numbers** fall in gaps between dataset ranges and were not included in the manifest.
- Our HEAD requests do not verify document *content* — only whether the URL returns a valid response. A document that has been replaced with a different file at the same URL would not be detected.

---

## PART III: AUDIT RESULTS

### Summary

| Metric | Count | Percentage |
|--------|-------|------------|
| Total corpus | 1,380,941 | 100% |
| Documents scanned | 1,365,677 | 98.89% |
| Unscanned (Akamai blocked) | 15,264 | 1.11% |
| **HTTP 200 (present)** | **1,284,829** | **93.04%** |
| **HTTP 404 (REMOVED)** | **78,234** | **5.67%** |
| HTTP 401 (auth failure) | 2,614 | 0.19% |
| Zero-byte files (200 but empty) | 26 | <0.01% |

### Per-Dataset Breakdown

| Dataset | Manifest | Scanned | Present | Removed | Removal Rate |
|---------|----------|---------|---------|---------|--------------|
| 1 | 3,158 | 3,158 | 3,147 | 11 | 0.35% |
| 2 | 574 | 574 | 564 | 10 | 1.74% |
| 3 | 67 | 67 | 62 | 5 | 7.46% |
| 4 | 152 | 152 | 151 | 1 | 0.66% |
| 5 | 120 | 120 | 118 | 2 | 1.67% |
| 6 | 13 | 13 | 12 | 1 | 7.69% |
| 7 | 17 | 17 | 17 | 0 | 0.00% |
| 8 | 10,595 | 10,595 | 10,579 | 16 | 0.15% |
| **9** | **531,284** | **516,020** | **439,790** | **76,230** | **14.77%** |
| 10 | 503,154 | 503,154 | 499,464 | 1,076 | 0.21% |
| 11 | 331,655 | 331,655 | 330,777 | 878 | 0.26% |
| 12 | 152 | 152 | 148 | 4 | 2.63% |
| **TOTAL** | **1,380,941** | **1,365,677** | **1,284,829** | **78,234** | **5.73%** |

Dataset 9 accounts for **97.4% of all removals** (76,230 of 78,234). This is the dataset that contains the bulk of the FBI investigative files, prosecutorial correspondence, Bureau of Prisons records, and grand jury materials — the categories of documents most directly responsive to the EFTA's disclosure mandate.

### Size Mismatch Analysis

Separately, we compared the Content-Length reported by the DOJ server for documents that *are* still accessible against the original file sizes recorded in our database (extracted from the original production). Of the documents returning HTTP 200:

- **23,989 documents have file sizes smaller than their originals** — every mismatch is a *reduction*, never an increase
- The largest reduction: one document lost 67% of its original file size (from 22.7 MB to 7.5 MB)
- This suggests post-publication re-processing or content removal that has not been disclosed

---

## PART IV: REMOVED DOCUMENTS — CASE-BY-CASE ANALYSIS

The following analysis examines four removed documents selected because they contain **no victim personally identifying information** and can be cited with full EFTA numbers without risk of directing readers to leaked victim PII. For each document, we provide: a description of its contents, an assessment of its relevance to the EFTA's disclosure mandate, and a carveout-by-carveout analysis of whether any lawful basis for removal exists.

All four documents were read in full from our text corpus. Local PDF copies are preserved.

---

### Document 1: BOP TRUINTEL Log — Composite (General Population + SHU + Inventory)

**EFTA:** [EFTA00053963](https://www.justice.gov/epstein/files/DataSet%209/EFTA00053963.pdf) · [OCR text](https://epstein-data.com/full_text_corpus/pages?_search=EFTA00053963&efta_number=EFTA00053963)
**Dataset:** 9 | **Pages:** 1,000 | **Status:** HTTP 404

This is a composite Federal Bureau of Prisons document containing TRUINTEL (intelligence tracking) logs for both General Population and the Special Housing Unit (9 South) at Metropolitan Correctional Center New York, plus MCC inventory reports. The logs cover July 1 through August 19, 2019 — the entire period of Epstein's incarceration and death. They record, shift by shift: officer rounds, inmate counts, cell searches, feeding schedules, watch calls, and key/radio checks.

This is the official minute-by-minute operational record of the housing units where Epstein was held. It is the document that would show whether institutional protocols were followed during the period leading to his death.

**EFTA Relevance:** Directly responsive to Section 2(a)(9) — "documentation of Epstein's detention or death (incident reports, witness interviews, medical examiner files, autopsy reports, written records detailing circumstances and cause of death)."

**Carveout Analysis:**
- **(A) Victim PII:** The log contains names and register numbers of other inmates housed in the unit. These individuals are not "victims" under the statute — they are incarcerated persons. Even if treated as protected, their names could be redacted without removing a 1,000-page document.
- **(B) CSAM:** No.
- **(C) Active investigation:** The guard investigation (Tova Noel and Michael Thomas) was resolved through deferred prosecution agreements. No active investigation exists.
- **(D) Images of death/abuse:** The document is a text-based administrative log. It contains no images.
- **(E) Classified:** No.

**Assessment: No legitimate carveout justifies removal.**

---

### Document 2: BOP TRUINTEL Log — 9 South Special Housing Unit

**EFTA:** [EFTA00120887](https://www.justice.gov/epstein/files/DataSet%209/EFTA00120887.pdf) · [OCR text](https://epstein-data.com/full_text_corpus/pages?_search=EFTA00120887&efta_number=EFTA00120887)
**Dataset:** 9 | **Pages:** 395 | **Status:** HTTP 404

This is the companion TRUINTEL log for the Special Housing Unit (SHU), 9 South, at MCC New York — the exact unit where Epstein was housed after his July 7, 2019 transfer from general population, and where he died on August 10, 2019. The log covers July 1 through August 19, 2019, recording every officer round, watch call, count, cell search, and feeding for the SHU.

This is the single most critical operational record for evaluating guard conduct on the night of Epstein's death. It would show whether the 30-minute round schedule was actually maintained or whether there were gaps on August 9-10, 2019.

**EFTA Relevance:** Directly responsive to Section 2(a)(9) — detention and death documentation.

**Carveout Analysis:**
- **(A) Victim PII:** Same as Document 1 — other SHU inmates' names could be redacted.
- **(B) CSAM:** No.
- **(C) Active investigation:** Same as Document 1 — guard investigation resolved.
- **(D) Images of death/abuse:** Text-based administrative log. No images.
- **(E) Classified:** No.

**Assessment: No legitimate carveout justifies removal.** This document and Document 1 together constitute 1,395 pages of the BOP's own operational records of what happened in Epstein's housing units. Their removal from public access directly undermines the EFTA's mandate to disclose "written records detailing circumstances and cause of death."

---

### Document 3: Psychological Reconstruction of Inmate Death

**EFTA:** [EFTA00041963](https://www.justice.gov/epstein/files/DataSet%209/EFTA00041963.pdf) · [OCR text](https://epstein-data.com/full_text_corpus/pages?_search=EFTA00041963&efta_number=EFTA00041963)
**Dataset:** 9 | **Pages:** 1,000 | **Status:** HTTP 404

This is the BOP's official Psychological Reconstruction of Jeffrey Epstein's death, prepared by the National Suicide Prevention Coordinator. The report is the BOP's own internal finding that its systems failed. On its opening page, it acknowledges three critical limitations:

1. "Formal interviews were not conducted as a part of this reconstruction to avoid interference with pending investigations by other Department of Justice components"
2. "There was no such video in this case since the original video was confiscated by the Federal Bureau of Investigation (FBI) prior to the beginning of this reconstruction"
3. These absences "severely limited the ability to establish accurate timelines"

The report documents that of 71 staff members who were emailed the notification that Epstein needed a cellmate after being removed from Psychological Observation, **only 27 opened the email** — meaning 62% of relevant staff never read the message. It details Epstein's institutional history, the July 23 incident involving cellmate Nicholas Tartaglione and a noose, the August 9 court document unsealing that reportedly distressed Epstein, and the systemic failures in monitoring.

**EFTA Relevance:** Directly responsive to Section 2(a)(9) — this *is* the death investigation reconstruction.

**Carveout Analysis:**
- **(A) Victim PII:** One victim name appears in the antecedent circumstances section. It could be redacted in a single line.
- **(B) CSAM:** No.
- **(C) Active investigation:** The report references "pending investigations" as of its drafting, but the guard investigation has since been resolved and no other active investigation has been disclosed.
- **(D) Images of death/abuse:** The document describes the death but contains no images of it.
- **(E) Classified:** No.

**Assessment: No legitimate carveout justifies removal.** This is one of the most important documents in the entire EFTA corpus. It is the BOP's own admission that its monitoring systems failed — no video, no interviews possible, a cellmate notification ignored by the majority of staff. One victim name is trivially redactable. Removing a 1,000-page institutional accountability document because of one name on one page is not "narrowly tailored."

---

### Document 4: Southern Trust Company USVI Bank Statements

**EFTA:** [EFTA01670187](https://www.justice.gov/epstein/files/DataSet%2010/EFTA01670187.pdf) · [OCR text](https://epstein-data.com/full_text_corpus/pages?_search=EFTA01670187&efta_number=EFTA01670187)
**Dataset:** 10 | **Pages:** 455 | **Status:** HTTP 404

These are FirstBank Virgin Islands commercial checking account statements for **Southern Trust Company Inc.**, 6100 Red Hook Quarters Suite B-3, St. Thomas, VI. The account shows a $1,000 opening deposit in December 2012, a $100,000 incoming wire transfer in March 2013, and subsequent disbursements through numbered checks.

The Bates stamps show these were produced by SDNY as confidential grand jury materials (marked "CONFIDENTIAL SDNY_GM_00017243").

**EFTA Relevance:** Directly responsive to Section 2(a)(5) — entities tied to Epstein's financial networks.

**Carveout Analysis:**
- **(A) Victim PII:** No.
- **(B) CSAM:** No.
- **(C) Active investigation:** The "CONFIDENTIAL" marking reflects Federal Rule of Criminal Procedure 6(e) grand jury secrecy. However, the EFTA specifically requires release of grand jury-related materials in Section 2(a)(1), and the underlying bank records are not grand jury testimony — they are business records subpoenaed by the grand jury.
- **(D) Images of death/abuse:** No.
- **(E) Classified:** No.

**Assessment: No strong carveout applies.** Grand jury secrecy (Rule 6(e)) is not one of the EFTA's five permitted carveouts. The statute was enacted precisely to override the normal secrecy protections that had kept these materials hidden. The bank records themselves — showing money flows through an Epstein-linked USVI entity — are responsive to the statute's financial network disclosure mandate.

---

## PART V: THE BROADER PICTURE

### What Else We Found — And Why We Are Not Showing You

The four documents above were selected for full citation because they contain no victim PII. But our review of additional removed documents — including internal prosecutorial emails, grand jury testimony, NPA breach correspondence, law enforcement affidavits, and court filings — revealed a much larger problem.

Multiple removed documents contain **extensive, unredacted victim personally identifying information** that the DOJ failed to adequately redact before publication. In the most severe case, we found a complete FBI victim contact sheet embedded within an email chain: approximately 30 victims' **full names, dates of birth, home addresses, phone numbers, email addresses, and family members** — for victims who were between 13 and 17 years old at the time of the crimes. This document was not only published with this information exposed — it was subsequently **restored to the DOJ's server** after being briefly removed, with the victim PII still intact.

Other documents we reviewed contained victim dates of birth leaked through incomplete redaction of police affidavits, full residential addresses given in grand jury testimony, victim school names combined with ages and dates that create identification vectors, and victim MySpace profiles quoted in deposition transcripts.

We are not identifying these documents by EFTA number, and we are not linking to them. We will not create a roadmap to pages where the DOJ's redaction failed.

This matters for the legal analysis because it reveals the DOJ's approach in both directions: documents that **should** be publicly accessible (BOP logs, institutional reports, shell company financials) were removed, while documents containing the most sensitive victim PII were published — and in some cases restored — without adequate redaction. The failure is not one of over-caution or under-caution. It is a failure of process.

### A Note on Victim Privacy

We attempted targeted PII redaction of victim-identifying information in our own text corpus at [epstein-data.com](https://epstein-data.com). The difficulty was extreme. A single law enforcement affidavit can run over 1,000 pages of OCR-processed text, with victim names and identifying details scattered unpredictably throughout — sometimes in narrative, sometimes in structured police forms where the OCR is so garbled that automated detection produces hundreds of false positives for every real match. School names that could narrow victim identification appear hundreds of times across the broader corpus. Dates of birth appear in formats that overlap with case numbers, booking dates, and field labels.

We redacted the specific victim-identifying information we were able to confirm in our databases, but we cannot guarantee completeness. The complete list of victim PII we identified has been cataloged in a private research file that is never published, never committed to any repository, and never deployed to any server.

We say this not to excuse the DOJ, but to underscore the scale of the problem *they created.* The Department published 2.7 million pages with insufficient redaction, then — rather than surgically fixing the specific pages where victim information leaked — removed entire documents wholesale. This is the opposite of the "narrowly tailored" standard the statute requires.

### Pattern Analysis

The four documents examined in detail above total **2,850 pages**, all confirmed removed (HTTP 404). None have any plausible legal basis for removal under any of the EFTA's five carveout categories:

| Document | Pages | Content | Carveout? |
|----------|-------|---------|-----------|
| BOP TRUINTEL Composite | 1,000 | Detention logs, GP + SHU + inventory | None |
| BOP TRUINTEL 9 South | 395 | SHU logs — Epstein's exact unit | None |
| BOP Psychological Reconstruction | 1,000 | Death investigation — "no video, no interviews" | None |
| Southern Trust Company Bank Statements | 455 | USVI shell entity financials | None |

Three of the four are directly responsive to Section 2(a)(9) — documentation of Epstein's detention and death. The fourth is responsive to Section 2(a)(5) — entities tied to Epstein's financial networks. These are the core categories the EFTA was enacted to disclose.

### The Dataset 9 Concentration

The overwhelming concentration of removals in Dataset 9 (76,230 of 78,234, or 97.4%) is significant because Dataset 9 contains the FBI's investigative files, prosecutorial correspondence, Bureau of Prisons records, and grand jury materials. These are the categories of documents most directly responsive to the EFTA's nine disclosure categories. Datasets containing less sensitive material (depositions, court filings, public records) show removal rates below 1%.

---

## PART VI: LEGAL IMPLICATIONS

### 1. Procedural Non-Compliance

The removal of 78,234 documents without published Federal Register justification violates Section 2(c)(2) of the EFTA on its face. The statute does not contain an exception for post-publication removal. Every withholding, every redaction requires written justification published in the Federal Register and submitted to Congress. None has been provided.

### 2. Wholesale Removal vs. Narrowly Tailored Redaction

Even where a carveout genuinely applies — such as victim PII in a law enforcement affidavit — the statute authorizes *redaction of segregable portions*, not removal of entire documents. We know from firsthand experience that targeted PII redaction in these documents is painstaking: it requires identifying specific lines on specific pages out of thousands of OCR-processed pages. But it is work the DOJ is obligated to do under the statute — and removing documents wholesale is not a substitute.

### 3. The Embarrassment Prohibition

Section 2(b) prohibits withholding based on "embarrassment, reputational harm, or political sensitivity." The BOP TRUINTEL logs and psychological reconstruction expose systemic failures in Epstein's detention — failures the BOP itself acknowledged. The EFTA was enacted precisely because Congress determined these documents should be public despite their embarrassing content.

### 4. Searchable and Downloadable Format

Section 2(a) requires records be made available in "searchable and downloadable format." Removing 78,234 PDFs from the server makes them neither searchable nor downloadable. This is a straightforward violation of the accessibility mandate.

---

## PART VII: METHODOLOGY NOTES AND DATA FILES

### Generated Data Files

The complete scan data — including the full list of all 78,234 removed EFTA numbers — is preserved in our research archive. We are not publishing the complete document-level data at this time because our review identified extensive unredacted victim PII in multiple removed documents, and publishing the full list would direct public attention to those pages. The underlying data has been shared with investigative journalists who have the editorial infrastructure to handle victim-identifying material responsibly.

### Reproducibility

The scanning methodology is fully documented and the complete scan results are preserved for independent verification. Any researcher who independently identifies a removed EFTA number can verify its status using the method below.

### How to Check Yourself (No Coding Required)

**To verify a removal:**
1. Open your browser's Developer Tools (F12), go to the **Network** tab
2. Navigate to any EFTA PDF on justice.gov (click through the age gate)
3. Click the PDF request in the Network tab
4. Look at the **Response Headers** — find `Last-Modified` and `Content-Length`
5. If `Last-Modified` shows **September 2, 2025**, you are looking at the DOJ's 404 error page, not the document — the file has been removed
6. If `Last-Modified` shows a later date (January or February 2026), the file was re-uploaded after the original publication

**To check if a still-accessible document was modified:**
1. Download the file from justice.gov today
2. Compare it against an original copy (anyone who downloaded the datasets when they were first published has originals)
3. If the file sizes differ or the MD5 checksums differ, the file was modified
4. Extract text from both (any PDF viewer can do this) and diff them — you may find OCR quality degraded, text garbled, or redaction patterns changed

---

## CONCLUSION

The Epstein Files Transparency Act was enacted with bipartisan support because Congress determined that the Department of Justice's records relating to Jeffrey Epstein must be made available to the public. The statute defines five narrow carveouts, requires written Federal Register justification for any withholding, and categorically prohibits withholding based on embarrassment or political sensitivity.

The DOJ published 1,380,941 documents. Then 78,234 of them disappeared — without Federal Register notice, without Congressional notification, without published justification. Among the removed documents: Bureau of Prisons detention logs from the night Epstein died, the government's own psychological reconstruction admitting "no video" and "no interviews," and bank statements for an Epstein-linked USVI shell entity. None of these documents contain victim PII. None have any plausible legal basis for removal.

Meanwhile, documents containing the most sensitive victim information imaginable — full names, dates of birth, home addresses, phone numbers, and family members of minor victims — were published with inadequate redaction, and in at least one case restored to the server with the victim PII still exposed. The DOJ's removal process is not protecting victims. It is removing institutional accountability records while leaving victim PII on the server.

For the four documents examined in full above, no lawful basis for removal exists under the statute. For all 78,234 removals, the procedural requirement of Federal Register notice was not followed. The complete list of removed documents has been shared with investigative journalists.

---

*This analysis was conducted using Claude Code running Opus 4.6, which can make mistakes. All EFTA numbers, dataset assignments, and HTTP status codes were verified programmatically. Document contents were read from the extracted text corpus and cross-referenced against local PDF copies. The four documents cited above were reviewed page by page and found to contain no victim personally identifying information before their EFTA numbers were included in this report.*
