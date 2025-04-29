#MedInfo-2025

#**Clinical decision support systems redeployment – levels of matching between variables in different ecosystems**

Gourav GUPTA,  Jan STANEK, Wolfgang MAYER, and Georg GROSSMANN

Industrial AI Research Centre, Digital Health Innovation and Clinical Informatics Lab (DHICI), University of South Australia, Adelaide, Australia

ORCiD ID: Gourav Gupta https://orcid.org/0000-0003-3122-1976, 
Jan Stanek https://orcid.org/0000-0003-0499-8317, 
Wolfgang Mayer https://orcid.org/0000-0002-2154-2269, 
Georg Grossmann https://orcid.org/0000-0003-4415-2228

**Abstract**. Creation of complex AI solutions is laborious and costly. Health organizations are highly diverse, so simple transfer of a solution from one organization to another is typically not viable, and redeployment is necessary. The first step in redeployment process is to determine differences between variables on the source and target system. In our paper we describe 5 dimensions to determine the match: shallow match, deep match, representation match, metadata match and data match.

**Keywords**. Clinical Decision Support System, portability, ecosystem interoperability

**Introduction**
New approaches in Artificial Intelligence (AI) encourage development of increasingly complex solutions – however development of these is becoming increasingly expensive and laborious [1] – e.g. compiling adequate training datasets for machine learning may take extended time and substantial effort in labelling the data (such as COD10K dataset [2]). Redeployment of a complex AI solution across different health care organizations needs to consider differences in the data ecosystems [3]  between these organizations. Associated cost of re-building of the CDSS from scratch in the new (target) ecosystem can be substantial [4]. In our project [5], we are proposing a framework to support portability of complex Clinical Decision Support Systems (CDSS). Below we discuss the first phase of the redeployment process which is the semi-automatic identification of the relevant set of differences between the organizations. where the CDSS was initially developed (source) and another organization (target). This process revolves around reconciliation of the set of input variables for the specific CDSS on the source system with the variables available in the target system.

**Dimensions of differences**
We propose five dimensions to establish the differences between two CDSS:

**1. Shallow match:** This match is based on terminologies used in both systems (such as SNOMED-CT [6] or UMLS [7]). The result can be: (1) Exact match (e.g. “Oliguria” on input = “Oliguria” term or after transformation: “Oliguria” on input ≈ “Low urine output” term), (2) Approximate match – exact match could not be found, but a similar term (terms) can be found in the terminology, or (3) No match found between the variable on input and terms in the terminology.

**2. Deep match:** Deep match is established on the level of an ontology – looking at definitions of the source and target concepts (identified in the previous step), e.g., Oliguria was historically defined anywhere between 300 and 700 ml/day; now the definition narrowed to 300 – 400 ml/day [8].

**3. Representation match:** An input may match on previous techniques, but its representation may differ, e.g., units of measure: blood glucose – while deemed an exact match on shallow and deep level – may be represented in mg% on source system and in mmol/l in the target system. In some cases, the units of measure cannot be easily reconciled, e.g., vitamin A contents given in mg is difficult to match with Retinol Activity Equivalent (RAE), as one unit of measure is based on weight of the substance, other one reflects biological activity.

**4. Metadata match:** Health data is collected and interpreted in context, e.g., assessing glomerular filtration rate in stable patients can be calculated using Cockroft-Galt formula, this does not work well in instable Intensive Care Unit (ICU) cases.

**5. Data match:** Heath care organizations frequently differ in their patient case mix, even if the type of care is identical. Performance of a CDSS can be affected by changes of case mix (e.g. dependence of the predictive value of the CDSS advice on prevalence of a diagnosis or symptom).

**Acknowledgements:** This work is part of the Digital Health Cooperative Research Centre project ‘PreHaRM: A Predictive Harm Response Management algorithmic tool to reduce adverse events in healthcare settings’ (DHCRC-0156).


**References**

[1]  Sutton, R.T., et al., An overview of clinical decision support systems: benefits, risks, and strategies for success. NPJ digital medicine,2020. 3(1): p. 17.

[2]  Fan, D.-P., et al., Concealed object detection. IEEE transactions on pattern analysis and machine intelligence, 2021. 44(10): p. 6024-6042.

[3]  Weber, G.M., K.D. Mandl, and I.S. Kohane, Finding the missing link for big biomedical data. Jama, 2014. 311(24): p. 2479-2480.

[4]  Donovan, T., et al., Implementation costs of hospital-based computerised decision support systems: a systematic review. Implementation Science, 2023. 18(1): p. 7.

[5]  Gupta, G., et al., Adaptive Semantic Framework for CDSS to a new environment, in Proceedings of the 2024 Australasian Computer Science Week. 2024. p. 75-77.

[6]  Chang, E. and J. Mostafa, The use of SNOMED CT, 2013-2020: a literature review. Journal of the American Medical Informatics Association, 2021. 28(9): p. 2017-2026.

[7]  Bodenreider, O., The unified medical language system (UMLS): integrating biomedical terminology. Nucleic acids research, 2004. 32(suppl_1): p. D267-D270.

[8]  Glassford, N.J. and Bellomo, R.: The role of oliguria and the absence of fluid administration and balance information in illness severity scores. Korean J. of Critical Care Medicine, 2017, 32(2), pp 106-123.

