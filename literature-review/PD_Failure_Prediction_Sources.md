# PD-based failure prediction – prior work (for Section 2.5.5 / project scope)

Checked through publisher, PMC, DOAJ and institutional-repository search records only; direct DOI pages could not be opened. **Open every DOI before citing.** [check] = one field not confirmed.

## A. Degradation / tree-stage classification (precursor to failure, not a forecast)
- **A1** R. Sahoo, S. Karmakar, "Investigation of electrical tree growth characteristics and partial discharge pattern analysis using deep neural network," *Electr. Power Syst. Res.*, vol. 220, 109287, 2023. https://doi.org/10.1016/j.epsr.2023.109287
  - XLPE tree specimens; PRPD classified into inception / propagation / breakdown stages.
  - Accuracy of 98.78% (EfficientNet) comes from a thesis summary [check].
- **A2** M. Florkowski, "Classification of partial discharge images using deep convolutional neural networks," *Energies*, 13(20), 5496, 2020. https://doi.org/10.3390/en13205496
  - Ageing classes: start / middle / end, plus noise.
- **A3** Z. Yang, Y. Gao, J. Deng, L. Lv, "Partial discharge characteristics and growth stage recognition of electrical tree in XLPE insulation," *IEEE Access*, vol. 11, pp. 145527–145535, 2023. https://doi.org/10.1109/ACCESS.2023.3344596
  - Accuracy not confirmed [check].
- **A4** R. Schurch et al., "Identification of electrical tree aging state in epoxy resin using partial discharge waveforms compared to traditional analysis," *Polymers*, 15(11), 2461, 2023. https://doi.org/10.3390/polym15112461
  - Detects the pre-breakdown state (tree crossing the insulation) in epoxy.
- **A5** R. Sahoo, S. Panigrahy, S. Karmakar, "Aging state recognition of a crosslinked polyethylene power cable insulation using machine learning and FTIR spectroscopy," IEEE ICHVE 2024 [check DOI].
  - XGBoost reached 93.33% separating moderately from highly aged insulation.

## B. Time-to-breakdown / remaining-life prediction (true prediction)
- **B1** S. Aziz (as indexed) [check first author], B. Catterson, S. M. Rowland, S. Bahadoorsingh, "Analysis of partial discharge features as prognostic indicators of electrical treeing," *IEEE TDEI*, 24(1), pp. 129–136, 2017. https://doi.org/10.1109/TDEI.2016.005957
  - PD features ranked for how well they track degradation; an exponential model predicts time to breakdown.
  - Silicone needle-plane samples.
- **B2** Y. Wang, J. Wu, T. Han, K. Haran, Y. Yin, "Insulation condition forewarning of form-wound winding for electric aircraft propulsion based on partial discharge and deep learning neural network," *High Voltage*, 6(2), pp. 302–313, 2021. https://doi.org/10.1049/hve2.12034
  - An autoencoder builds a failure precursor from PD features; an LSTM forecasts it several steps ahead.
- **B3** G. C. Stone, I. Culbert, "Prediction of stator winding remaining life from diagnostic measurements," IEEE ISEI 2010 [check DOI].
  - Industry caution: PD trends give relative risk, not a reliable remaining life.
- **B4** "Study on characteristics of health monitoring and critical warning based on partial discharge signals during the growth of electrical trees," *Electrical Engineering*, 2024. https://doi.org/10.1007/s00202-024-02687-z [check authors]
  - Defines a critical-warning threshold and a dynamic health index.

## C. Health index of XLPE cables (classification of current condition)
- **C1** R. Sahoo, S. Karmakar, S. Panigrahy, "Health index analysis of XLPE cable insulation using machine learning technique," IEEE UPCON 2020 (conference) [check DOI].
  - SVM 98%.
- **C2** A. Ansari et al., "Estimating the insulation health index of XLPE cables using machine learning," *Sci. Rep.*, vol. 15, 2025. https://doi.org/10.1038/s41598-025-25080-7
  - ANN 94.5%.
- **C3** M. Abdolahi, W. Song, M. Yazdani-Asrami, "Intelligent condition monitoring of power cables using advanced machine learning models," *Results in Engineering*, vol. 29, 108371, 2026. https://doi.org/10.1016/j.rineng.2025.108371
- **C4** J. I. Aizpurua et al., "Towards a hybrid power cable health index for MV power cable condition monitoring," IEEE EIC 2019, pp. 481–484 [check DOI].

## D. Online monitoring / early warning (field)
- **D1** G. C. Montanari, P. Seri, R. Hebner, "A scheme for the health index and residual life of cables based on measurement and monitoring of diagnostic quantities," IEEE PES GM 2018. https://doi.org/10.1109/PESGM.2018.8585858
- **D2** G. C. Montanari, R. Hebner, P. Seri, R. Ghosh, "Self-assessment of health conditions of electrical assets and grid components: a contribution to smart grids," *IEEE Trans. Smart Grid*, 12(2), pp. 1206–1214, 2021. https://doi.org/10.1109/TSG.2020.3028501
- **D3** F. Steennis et al., "Smart Cable Guard for PD-online monitoring of MV underground power cables in Stedin's network," CMD 2014, pp. 525–528 [check DOI].
  - Utility deployment (Netherlands).

## E. Reviews
- **E1** M. Fikri, Z. Abdul-Malek, "Partial discharge diagnosis and remaining useful lifetime in XLPE extruded power cables under DC voltage: a review," *Electrical Engineering*, 105(6), 2023. https://doi.org/10.1007/s00202-023-01935-y
- **E2** M. Al Shaikh Saleh et al., "A review on the lifetime estimation methods of XLPE power cables," *IEEE Open J. Ind. Appl.*, vol. 6, pp. 445–489, 2025 [check DOI].
- **E3** K. Emdadi et al., "Overview of monitoring, diagnostics, aging analysis, and maintenance strategies in high-voltage AC/DC XLPE cable systems," *Sensors*, 25(22), 7096, 2025. https://doi.org/10.3390/s25227096
