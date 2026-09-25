# Arabic MoCA AI Multimodal Dataset

This repository contains the anonymized multimodal dataset used for evaluating a hybrid AI-assisted Montreal Cognitive Assessment (MoCA) scoring framework for cognitive screening in Arabic-speaking older adults.

The dataset was collected during supervised cognitive assessment sessions conducted in an elderly care facility and is intended to support research in AI-assisted neuropsychological assessment and explainable medical AI systems.

---

## Dataset Overview

The dataset includes data collected from **24 Arabic-speaking participants aged 50 years and older**.

Participants were clinically categorized based on manual MoCA assessment prior to AI evaluation.

Participant distribution:

- Dementia: 10 participants  
- Mild Cognitive Impairment (MCI): 8 participants  
- Cognitively Normal: 6 participants  

All participants completed the full assessment protocol.

---

## Data Modalities

The dataset contains multimodal records corresponding to different MoCA task domains.

### Audio Recordings

Audio responses collected during language-related tasks including:

- Verbal Fluency
- Sentence Repetition
- Abstraction
- Attention Tasks
- Delayed Recall

Each audio recording corresponds to an individual task or sub-question to enable detailed analysis.

---

### Visuospatial Drawings

Images of paper-based drawing tasks including:

- Clock Drawing Test
- Cube Copy Test

Participants completed these drawings on paper according to standard MoCA procedures, and the drawings were captured as images for computer vision analysis.

---

### Touch Interaction Data

For touchscreen-based tasks such as the Trail Making Test, the application recorded structured behavioral interaction data including:

- Stroke coordinates
- Normalized screen coordinates
- Timestamped drawing progression
- Connection order between targets
- Task completion timing

These logs allow reconstruction of drawing trajectories and validation of task execution.

---

### Label File References

Paths in each participant's `labels.json` are relative to that participant's folder. When a task has no corresponding recording in the release, its `audio_file` value is `null`.

---

## Data Anonymization

All data have been fully anonymized prior to release.

- Each participant is identified using a **Participant ID**
- No personally identifiable information (PII) is included
- All files were reviewed to remove identifying information

---

## Intended Research Use

This dataset may support research in:

- AI-assisted cognitive screening
- Multimodal medical data analysis
- Explainable artificial intelligence in healthcare
- Digital biomarkers for dementia and mild cognitive impairment

---

## Data License

Unless otherwise noted, the dataset in this repository is licensed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**.

You may share and adapt the dataset for any purpose, provided that you give appropriate credit, link to the license, and indicate whether changes were made. See the [full license](https://creativecommons.org/licenses/by/4.0/).

This license does not grant permissions for privacy, publicity, or other rights that may apply to identifiable people or third-party material. Users are responsible for confirming that their use complies with applicable laws, ethics requirements, and the rights of others.

---

## Citation

If you use this dataset in academic research, please cite the associated research work.

---

## Disclaimer

This dataset is provided for **research purposes only** and should not be used for clinical decision-making without appropriate validation.
