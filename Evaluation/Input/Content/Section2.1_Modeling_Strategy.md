The general workflow for building an adult PBPK model has been described by Kuepfer et al. ([Kuepfer 2016](#5-References)). Relevant information on the anthropometry (height, weight) was gathered from the respective clinical study, if reported. Information on physiological parameters (e.g. blood flows, organ volumes, hematocrit) in adults was gathered from the literature and has been incorporated in PK-Sim<sup>®</sup>) as described previously ([Willmann 2007](#5-References)). The  applied activity and variability of plasma proteins and active processes that are integrated into PK-Sim® are described in the publicly available 'PK-Sim<sup>®</sup> Ontogeny Database Version 7.3' ([PK-Sim Ontogeny Database Version 7.3](#5-References)).

The PBPK model was developed based on clinical data of healthy, non-obese, adult subjects obtained from the literature, covering different single doses of alprazolam administered via the intravenous (IV) or oral (PO) route in the fasted state. Several oral dosage forms were included in the model building process, such as Xanax<sup>®</sup> and Solanax<sup>®</sup> tablets. Comparison of the reported alprazolam plasma concentration-time profiles following administration of Xanax<sup>®</sup> and Solanax<sup>®</sup> tablets indicated that the latter oral dosage form yields a larger t<sub>max</sub> than the Xanax<sup>®</sup> immediate release formulation. Therefore, different dissolution kinetics were developed for these two oral dosage forms. The reported PK profiles following administration of Solanax<sup>®</sup> tablets were measured in Japanese subjects ([Yasui 1996](#5-References), [Yasui 1998](#5-References), [Yasui 2000](#5-References)). To account for ethnicity-related differences in anatomical and physiological model parameters, the European Standard Individual used per default in the simulations was scaled to a Japanese individual and the reference concentration of CYP3A4 in this individual was optimized to better match the clinical data. Finally, mass balance information on urinary excretion of unchanged <sup>14</sup>C-alprazolam after PO administration reported by  Eberts et al. ([Eberts 1980](#5-References)) was also accounted for during the model building process. 

Unknown parameters were simultaneously optimized using all available PK data, in particular:

-  2 plasma concentration-time profiles following single IV administration of 0.25 mg
-  2 plasma concentration-time profiles following single IV administration of 0.5 mg
-  3 plasma concentration-time profiles following single IV administration of 1 mg
-  1 plasma concentration-time profile following single IV administration of 1 mg followed by 1.576 mg over 8 h
-  2 plasma concentration-time profiles following single IV administration of 2 mg
-  3 plasma concentration-time profiles following single IV administration of 4 mg
- 2 plasma concentration-time profiles following single PO administration of 0.5 mg
- 3 plasma concentration-time profiles following single PO administration of Solanax<sup>®</sup> tablets containing 0.8 mg alprazolam to Japanese subjects
- 12 plasma concentration-time profiles following single PO administration of 1 mg
- 1 plasma concentration-time profile following single PO administration of 2 mg
- 1 dose fraction excreted unchanged in urine following single PO administration of 2 mg

Structural model selection was mainly guided by visual inspection of the resulting description of data and biological plausibility. The following parameters were identified using the Parameter Identification module provided in PK-Sim<sup>®</sup> and MoBi<sup>®</sup> ([Open Systems Pharmacology Documentation](#5-References)):

- `Dissolution time (50% dissolved)`
- `Dissolution shape`
- `Specific intestinal permeability`
- `Mucosa permeability (interstitial<->intracellular)`
- `Lipophilicity`
- `Metabolizing Enzyme - CYP3A4 - kcat`
- `Reference concentration CYP3A4` (only for Japanese subjects)
- `GFR fraction`

Details about input data (physicochemical, *in vitro* and clinical) can be found in [Section 2.2](#22-Data).

Details about the structural model and its parameters can be found in [Section 2.3](#23-Model-Parameters-and-Assumptions).





