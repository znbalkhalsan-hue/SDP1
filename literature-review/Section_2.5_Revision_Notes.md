# Section 2.5 – revision notes (progress report)

`Section_2.5_Revised.docx` replaces the whole of Section 2.5 in the shared report (pages 8–22 of *Report Shared Doc*). The older per-subsection drafts in this folder are now out of date.

## Length

| | Before | After |
|---|---|---|
| Pages (Garamond 11, A4) | about 15 | about 5.3 |
| Words (text, tables, captions, references) | about 7,840 | about 3,520 |
| Figures / tables | 6 / 6 | 2 / 2 |
| Reference lists | 4 (same papers repeated) | 1 (15 papers) |

## New structure

- **2.5.1 PD Classification Problem**
  - Detection, classification and prediction are kept as separate tasks.
  - The classifier supports the engineer; it does not replace the measurement system.
  - Covers the provisional classes, the input representations and the reasons classification is hard.
- **2.5.2 Traditional ML.** Features, classifiers, strengths and limits. The SVM and RF baselines are named here once.
- **2.5.3 Deep learning.** Grouped by the supervisors' three families: temporal/1D, PRPD/2D and image (new Figure 2).
- **2.5.4 Comparison.**
  - Table 1 is the literature matrix, using exactly the fields the supervisors listed: paper/year, PD type/dataset, input, algorithm, accuracy, precision/recall/F1, key limitation.
  - Table 2 compares the three families against the supervisors' decision criteria.
  - Ends with the provisional shortlist.
- **2.5.5 Performance, robustness, generalisation.**
  - Topics: metrics, noise, new specimens and data splitting, amount of data.
  - Ends with a short "link to early warning" paragraph.

## Errors found in the old version (all fixed)

Reference numbers in this list are the **old** ones. The rest of these notes use the new numbering in the revised section.

1. **Table 3 cited the wrong papers.**
   - "2017 [1]" should be Raymond [8].
   - "2024 [8]" (composite defects) should be Qin [7].
   - "2024 [7]" (cable-terminal pulses) should be Sun [6].
   - "1993 [5]" should be Gulski & Krivda [3].
2. **Stale cross-references from the old Section 3.2 numbering.**
   - "Section 3.2.2" and "Section 3.2.4" in 2.5.3.2.
   - "compared in Section 3.2.4" in 2.5.3.
   - "Sections 3.2.2 and 3.2.3" and "Section 3.2.5.4" in 2.5.4.
   - 2.5.2.4 also said the DL models were in 2.5.4 (they are in 2.5.3).
3. **Figure numbers in the text did not match the captions.**
   - The text said Figures 1, 2, 3, 5 and 6 where the captions were 3, 4, 5, 6 and 7.
   - One caption sat in the middle of 2.5.1.2.
   - Table 6 had no caption.
   - All figure and table numbers are now Word fields (see "Pasting into the report" below).
4. **Raymond et al., ANFIS figure.** The best noise-free ANFIS accuracy is **96.6%**, not 97.0%. All three best clean results (SVM 98.8%, ANFIS 96.6%, ANN 93.2%) use statistical features.
5. **Raymond et al., noise drop.** "SVM with statistical features fell from 91.6% to 48.2%" started from the 5 s noise point. The clean value is 98.8%, so the text now says 98.8% → 48.2% at 60 s.
6. **DL vs ML gap stated two ways.**
   - 2.5.3 said "1 to 6.47 points" (6.47 was measured against the weaker BPNN baseline).
   - 2.5.4 said "1.0 to 4.76 points" (measured against the best traditional model).
   - Only the second, consistent version is kept.
7. **Sahoo et al. [1] overstated.** The survey says classification *usually* has two steps (the old text said "almost all"). It also says only *limited* success had been achieved with simple sources (the old text said "some success").
8. **"Failure prediction is a key objective of this project"** conflicts with both meeting records. Both say to keep the focus on classifying the PD type and not claim predictive capability until the data support it. The supervisors' notes add that classification, monitoring and prediction should be kept distinct. Early warning is now described as a possible future extension. **This reverses an edit made in an earlier session, so please confirm with the team.**
9. **Unconfirmable details removed.** The Gulski & Krivda details (12 defect types, 40–400 kHz detector, training times) could not be confirmed and were not needed.

## Repetition removed (examples)

- "Untrained/unknown patterns get misclassified" appeared about 7 times. It is now once, with the "unknown" output decision.
- Peng et al.'s 3,500 PD + 3,500 interference pulses appeared 5 times; now once (as a feature-selection example).
- The SVM tuning result (84.52% → 97.29%) appeared twice in the text plus a table; now once plus Table 1.
- Sun et al.'s 94.8% vs 95.8% appeared about 6 times.
- The per-class accuracies (80.87%, 85.42%, 79.54%) were in both 2.5.3 and 2.5.5; now only 2.5.5.
- The training times and GFLOPs were in both the text and the tables.
- "Results can't be compared across studies" appeared 4 times, twice in back-to-back sentences.
- The project plan (baselines and shortlist) appeared 3 times.
- The "5–20 fingerprints per feature" rule appeared twice and has been removed.
- Old Tables 1, 3, 4 and 5 covered the same studies and are merged into the new Table 1.

## Removed as not needed for a progress report

- Krivda four-outcome figure (now one sentence)
- HFCT 20 ms waveform figure (belongs in 2.2/2.4 if anywhere)
- SVM-principle figure
- Raymond noise-curve figure (key numbers kept in the text)
- Statistical-operators table (main operators named in one sentence)
- CNN/LSTM layer-by-layer details
- Auto-encoders
- DL history (2006/2015)
- The "Transformer" naming note

## Added

- **Xie et al. 2024** (Sensors 24(23) 7602). S-transform time–frequency images plus a 2D CNN, separating PD from corona interference with up to 98.75% accuracy. It covers the "image from a single pulse" route that the supervisors' image family includes, and shows that image methods do not always need a phase reference.
  - It is a PD-vs-interference study, not defect classification, so it is kept out of Table 1.
- **Figure 2** (approach families) and **Table 2** (comparison against the decision criteria).
- An abbreviation note under Table 1.
- One sentence on a simple Jupyter baseline on public data this semester (from Minutes 2 and the supervisors' "ready for Meeting 2" list). Delete it if the team has decided otherwise.

## What was checked, and what you still need to check

The paper websites are blocked in this environment, so checks used web-search abstracts and indexed text. Your earlier draft was written from the full papers, so the unchecked items are probably right, but please tick them off against the PDFs.

**Confirmed this time**
- [1] Sahoo: two-step procedure; limited success with simple sources.
- [2] Krivda: recognition used to be done "by eye" on an oscilloscope.
- [3] Kumar: the three PD types are not equally harmful.
- [5] Gulski & Krivda: BP/SOM/LVQ networks; untrained patterns can be misclassified.
- [6] Raymond: all setup details; SVM 98.8% (statistical); ANN 93.2%; ANFIS 96.6%; SVM-PCA 93.6% → 75.6%; SVM fastest to train; reports accuracy only. 48.2% at 60 s was read from the paper's own Figure 5.
- [7] Qin: defects; 5 features; 2,400 samples; 97.29%; standard SVM average 84.52% (computed from the per-defect results).
- [8] Sun:
  - specimens: electrode models on EPDM film; HFCT + oscilloscope; 251 points; 400 per class;
  - model: 2-conv-layer 1D CNN on raw pulses;
  - results: 95.8 / 94.8 / 91.2%; 73.6% → 98.7% with more training data; reports precision, recall and F1.
- [9] Peng (CNN): EPR cable; 5 defects; 3,500 pulses; 33 features; CNN beat SVM and BPNN.
- [11] Üçkol: 36 kV XLPE terminations; 5 defects; 1,200 PRPD images (two sets of 600); 30 s recordings; RGB images.
- [13] Xie: as above.

**Not re-checked (please look at the PDFs)**
- [4] Peng (RF): 3,500 + 3,500 pulses; 34 + 119 + 1,082 features.
- [9] Peng (CNN): 92.57%, 87.81%, 86.10%; 80.87% and 85.42%; 384 s vs 6.3 s.
- [10] Nguyen:
  - setup: GIS/UHF; 60-cycle sequences;
  - results: 96.74%; floating 79.54%; ANN 93.01%; SVM 90.71%;
  - slower than the baselines; overlapping windows split at random.
- [11] Üçkol:
  - 64 × 64 images;
  - results: 96.77%; 98.8 / 97.2 / 94.3%; void misclassification;
  - pretrained-network comparison; 485 s vs 9,349 s;
  - noise listed as future work.
- [12] Li: every number in the row (HFCT + UHF, 1,426 maps, classes, 97.52%, less computation than VGG16, per-class accuracy, noise as future work).
- [2] Krivda: patterns change with test voltage and ageing.
- [3] Kumar: PRPD works best with one source and low noise; the general ANN, SVM and DL statements.
- Table 1, "Per-class results" column for [9]–[12].
- [13] Xie: first author's initial.
- [14] Sahoo & Karmakar and [15] Wang are now described without any numbers.

## Check with teammates

- Cross-references to other sections: 2.4.2 (PRPD / time-resolved representations), 2.4.3 (signal processing), 2.4.4 (public datasets), and "Sections 2.2 to 2.4".
- 2.5.4 says the same criteria will be used for the **decision matrix in Section 3**. Make sure Section 3 has one, or delete that sentence.
- The handover note in this folder still lists the statistical-operators table and Krivda's four-outcome figure as "already in 2.5". They have been removed, so 2.4.3 can use the operators table if it wants.

## Pasting into the report

1. Copy everything from `Section_2.5_Revised.docx` and paste it over the old Section 2.5.
2. If your headings are numbered automatically, delete the typed numbers ("2.5", "2.5.1" …) from the headings after pasting.
3. Press **Ctrl+A, then F9** to update the fields. Figure and table numbers and the in-text "Figure 1 / Table 1" references are Word fields, so they renumber to fit the report (for example, Figure 1 becomes Figure 3 if two figures come before it).
4. Citations are plain-text [1]–[15], numbered in order of first use in this section.
