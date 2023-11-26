# HeartXtract

HeartXtract is a Python based framework that can used to characterize heart structure categories and patient descriptors from MIMIC-III notes following a hierarchical numerical coding system.

# Demo
The MIMIC-III data is hosted on BigQuery and the framework is integrated with Google BigQuery and Google Colab. 

Run the Demo on Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]([https://colab.research.google.com/drive/your-notebook-id (https://colab.research.google.com/drive/1FEmWGK37qSav4puFaiCZycHiLUcq-6_1))


<img width="630" alt="sample_note" src="https://github.com/danamouk/HeartXtract/assets/49573192/c381f916-6c6a-4cb4-8ea8-4174a44a0111">

<img width="641" alt="heart_categories" src="https://github.com/danamouk/HeartXtract/assets/49573192/e33cbe8e-c2cb-4b8c-b7a3-7e19cd7ccd0e">

HeartXtract extracts the following heart characteristics and patient descriptors from patient echo notes:

| Column Name            | Description                                                           |
|------------------------|-----------------------------------------------------------------------|
| subject_id             | De-identified patient ID                                              |
| hadm_id                | De-identified hospital admission ID                                  |
| row_id                 | Echocardiogram report ID                                             |
| category               | Clinical note type (e.g., echocardiogram)                            |
| text                   | Raw clinical note text                                               |
| chartdate              | De-identified clinical note charted date                             |
| LA_cavity              | Left atrium cavity                                                    |
| RA_dilated             | Right atrium dilated                                                 |
| LV_systolic            | Left ventricle systolic                                              |
| LV_cavity              | Left ventricle cavity                                                 |
| LV_wall                | Left ventricle wall                                                   |
| RV_cavity              | Right ventricle cavity                                                |
| RV_systolic            | Right ventricle systolic                                              |
| AV_stenosis            | Aortic valve stenosis                                                |
| MV_stenosis            | Mitral valve stenosis                                                |
| TV_regurgitation       | Tricuspid valve regurgitation                                        |
| TV_stenosis            | Tricuspid valve stenosis                                             |
| TV_pulm_htn            | Tricuspid valve pulmonary hypertension                              |
| AV_regurgitation       | Aortic valve regurgitation                                           |
| MV_regurgitation       | Mitral valve regurgitation                                           |
| RA_pressure            | Right atrium pressure                                                |
| LV_diastolic           | Left ventricle diastolic                                             |
| RV_volume_overload     | Right ventricle volume overload                                      |
| RV_wall                | Right ventricle wall                                                 |
| RV_pressure_overload   | Right ventricle pressure overload                                    |
| height (in)            | Measurement of patient height in inches                               |
| weight (lb)            | Measurement of patient weight in pounds                               |
| heart rate (bpm)       | Measurement of heart rate in beats per minute                         |
| status                 | Patient status at the time of echocardiogram (inpatient or outpatient)|
| sbp (mmHg)            | Systolic blood pressure                                              |
| dbp (mmHg)            | Diastolic blood pressure                                             |
| date_time              | De-identified clinical note charted date and time                     |
| technical_quality      | Assessment of technical quality of echocardiogram                     |
| contrast               | Use of contrast agents during echocardiogram                          |
| test                   | Specific type of echocardiogram conducted                             |
| doppler                | Doppler measurements during echocardiogram                           |
| BSA (m^2)           | Body surface area in square meters                                    |

