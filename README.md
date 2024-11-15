# Language Model Evaluation Harness with Medical Specialities Classification

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10256836.svg)](https://doi.org/10.5281/zenodo.10256836)

---
Fork from the official lm-evaluation-harness repo with the task medical_specialities included to classify different questions into their medical specialities.
---

## How to use it

Follow the official lm-evaluation-harness guide with the task **medical_specialities**

```bash
lm_eval --model hf \
    --model_args pretrained=EleutherAI/pythia-160m \
    --tasks medical_specialities \
    --device cuda:0 \
    --batch_size 8
```

With you will get a list of the metrics per speciality, which can help you identify if there is one category underrepresented, or other biases.

|       Tasks       |Version|Filter|n-shot|Metric|   |Value |   |Stderr|
|-------------------|------:|------|-----:|------|---|-----:|---|-----:|
|Allergy            |      0|none  |     0|acc   |↑  |0.3200|±  |0.0469|
|Anatomy            |      0|none  |     0|acc   |↑  |0.2862|±  |0.0186|
|Anesthesiology     |      0|none  |     0|acc   |↑  |0.2577|±  |0.0344|
|Biochemistry       |      0|none  |     0|acc   |↑  |0.2388|±  |0.0104|
|Cardiology         |      0|none  |     0|acc   |↑  |0.2659|±  |0.0211|
|Chemistry          |      0|none  |     0|acc   |↑  |0.2587|±  |0.0193|
|Dermatology        |      0|none  |     0|acc   |↑  |0.2660|±  |0.0323|
|Emergency          |      0|none  |     0|acc   |↑  |0.2871|±  |0.0319|
|Endocrinology      |      0|none  |     0|acc   |↑  |0.2456|±  |0.0216|
|Gastroenterology   |      0|none  |     0|acc   |↑  |0.2364|±  |0.0207|
|Genetics           |      0|none  |     0|acc   |↑  |0.2776|±  |0.0192|
|Geriatrics         |      0|none  |     0|acc   |↑  |0.2609|±  |0.0532|
|Gynecology         |      0|none  |     0|acc   |↑  |0.3015|±  |0.0395|
|Hematology         |      0|none  |     0|acc   |↑  |0.2220|±  |0.0184|
|Microbiology       |      0|none  |     0|acc   |↑  |0.2576|±  |0.0141|
|Nephrology         |      0|none  |     0|acc   |↑  |0.2747|±  |0.0271|
|Neurology          |      0|none  |     0|acc   |↑  |0.2801|±  |0.0210|
|Nursing            |      0|none  |     0|acc   |↑  |0.2374|±  |0.0303|
|Obstetrics         |      0|none  |     0|acc   |↑  |0.2655|±  |0.0235|
|Odontology         |      0|none  |     0|acc   |↑  |0.3337|±  |0.0149|
|Oncology           |      0|none  |     0|acc   |↑  |0.2367|±  |0.0272|
|Ophthalmology      |      0|none  |     0|acc   |↑  |0.2500|±  |0.0367|
|Orthopedics        |      0|none  |     0|acc   |↑  |0.3180|±  |0.0317|
|Otorhinolaryngology|      0|none  |     0|acc   |↑  |0.2775|±  |0.0310|
|Pathology          |      0|none  |     0|acc   |↑  |0.2680|±  |0.0452|
|Pediatrics         |      0|none  |     0|acc   |↑  |0.2959|±  |0.0267|
|Pharmacology       |      0|none  |     0|acc   |↑  |0.2772|±  |0.0158|
|Physiology         |      0|none  |     0|acc   |↑  |0.2559|±  |0.0254|
|Psychiatry         |      0|none  |     0|acc   |↑  |0.2601|±  |0.0143|
|Psychology         |      0|none  |     0|acc   |↑  |0.2686|±  |0.0202|
|Radiology          |      0|none  |     0|acc   |↑  |0.3371|±  |0.0504|
|Respiratory        |      0|none  |     0|acc   |↑  |0.2600|±  |0.0235|
|Rheumatology       |      0|none  |     0|acc   |↑  |0.2110|±  |0.0393|
|Surgery            |      0|none  |     0|acc   |↑  |0.2697|±  |0.0334|
|Urology            |      0|none  |     0|acc   |↑  |0.2727|±  |0.0427|


* More info about the datasets: https://huggingface.co/datasets/HPAI-BSC/medical-specialities 
* More info about the code to classify the questions: https://github.com/HPAI-BSC/medical-specialities
* Notebook with usage example: [link](https://docs.hpai.cloud/s/cWDQZ8TdPKT67K9)