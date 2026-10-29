# Demonstration: Six Fictional Cases & 12 Saved Engine Outputs

## Case 1: Ordinary Dengue (Day 3 Febrile) — Mode: Baseline (640.56s)

### Retrieved Canonical Cards (Baseline Mode — 4 Cards)
- **`DENGUE_DIAG_01`** (Dengue | `probable_diagnosis` | Score: `0.2944`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 26-28, 45-47**
- **`CHIK_DIAG_01`** (Chikungunya | `probable_diagnosis` | Score: `0.2112`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 11-15, 18-19**
- **`DENGUE_MED_01`** (Dengue | `medication_guidance` | Score: `0.1061`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 47-48**
- **`DENGUE_ADV_01`** (Dengue | `advice` | Score: `0.1056`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 28, 47-48**


**Mode:** `Baseline` | **Model:** `Qwen/Qwen2.5-1.5B-Instruct (Local)` | **Response Time:** `640.56s`

---
### 1. Missing Information & Applicability Check
The patient presents with sudden onset high continuous fever (39.5°C), severe headache, retro-orbital pain, muscle and joint pain (myalgia/arthralgia), and mild nausea. The patient has no other complaints such as abdominal pain, bleeding, vomiting, or persistent diarrhea. There is no mention of symptoms suggestive of chikungunya or malaria. The patient's vitals are stable, and there are no high-risk comorbidities listed. The patient does not have a history of diabetes, hypertension, kidney or liver disease, nor is he pregnant. 

### 2. Probable Diagnosis (cite [Card ID | Page])
Based on the presented symptoms, the most likely diagnosis is **Dengue**. This is supported by the following card:

- **DENGUE DIAG_01**: Acute onset of high-grade continuous fever (39-40°C) lasting 2-7 days, two or more of: nausea/vomiting, macular or maculopapular rash, severe headache, retro-orbital pain, myalgia/arthralgia, positive tourniquet test, or leucopenia (WBC < 5000/mm³).

### 3. Investigations (cite [Card ID | Page])
No specific investigations are mentioned in the provided data. However, typical investigations would include:

- Complete Blood Count (CBC)
- Platelet count
- Hemoglobin level
- Urinalysis
- Liver function tests (LFTs)

### 4. Medication Planning (include Name, Dose, Route, Frequency, Duration, Instructions & Contraindications; cite [Card ID | Page])
#### Paracetamol
- **Name:** Paracetamol
- **Dose:** Max 3 g/day in adults (60 mg/kg/24 hrs in children)
- **Route:** Oral
- **Frequency:** Divided doses as needed for fever
- **Duration:** During febrile period
- **Instructions:** Do not exceed 3 g/day in adults. Warn patient that fever may not fully settle with paracetamol and not to take excess.

#### Oral Rehydration Solution (ORS)
- **Name:** ORS / Electrolyte fluids
- **Dose:** 2400 mL per 24 hours for adults ≥50 kg (or 2 mL/kg/hour for 24 hours if body weight <50 kg)
- **Route:** Oral
- **Frequency:** Spread evenly across the 24-hour day
- **Duration:** Throughout acute febrile and defervescence phase
- **Instructions:** Use ORS, green coconut water, fruit juices, or soup containing electrolytes rather than plain water alone.

#### NSAIDs and Steroids
- **Contraindications:** Temporarily withhold long-term warfarin, aspirin, clopidogrel, and dipyridamole (seek expert opinion if essential).
- **Exclusion:** Avoid all NSAIDs (including COX-2 inhibitors), aspirin, and

---

## Case 1: Ordinary Dengue (Day 3 Febrile) — Mode: Improved (840.3s)

### Retrieved Canonical Cards (Improved Mode — 6 Cards)
- **`DENGUE_DIAG_01`** (Dengue | `probable_diagnosis` | Score: `0.2944`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 26-28, 45-47**
- **`CHIK_INV_01`** (Chikungunya | `investigations` | Score: `0.07`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 11, 21-22, 26**
- **`DENGUE_MED_01`** (Dengue | `medication_guidance` | Score: `0.1061`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 47-48**
- **`DENGUE_ADV_01`** (Dengue | `advice` | Score: `0.1056`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 28, 47-48**
- **`CHIK_DIAG_01`** (Chikungunya | `probable_diagnosis` | Score: `0.2112`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 11-15, 18-19**
- **`DIFF_DENGUE_CHIK_01`** (Dengue / Chikungunya | `probable_diagnosis` | Score: `0.0954`)
  - *Source:* National Guideline for Clinical Management of Dengue (5th Ed) & National Guideline on Chikungunya Management (2017), **PDF Page: Dengue Page 29; Chikungunya Pages 16-18**


**Mode:** `Improved` | **Model:** `Qwen/Qwen2.5-1.5B-Instruct (Local)` | **Response Time:** `840.3s`

---
### 1. Missing Information & Applicability Check
The patient's complaint includes sudden onset high continuous fever (39.5°C), severe headache, retro-orbital pain, muscle and joint pain (myalgia/arthralgia), and mild nausea. The patient does not have symptoms such as abdominal pain, bleeding, persistent vomiting, or persistent diarrhea. There is no mention of persistent high fever or other warning signs consistent with Dengue or Chikungunya. The patient also reports no history of diabetes, hypertension, kidney or liver disease, or pregnancy. 

### 2. Probable Diagnosis (cite [Card ID | Page])
Based on the patient’s symptoms and absence of typical Dengue or Chikungunya signs, the most likely diagnosis is **Acute Upper Respiratory Infection**. This condition presents with fever, headache, myalgia, and arthralgia but does not include gastrointestinal symptoms or the characteristic rash seen in Dengue or Chikungunya.

### 3. Investigations (cite [Card ID | Page])
Given the lack of typical Dengue or Chikungunya symptoms, the following investigations should be ordered:

- **CBC**: To assess leukocyte count and platelet levels.
- **ESR**: Elevated ESR suggests inflammation.
- **CRP**: Increased CRP indicates systemic inflammatory response.
- **SGPT**: Elevated SGPT could indicate liver involvement.

These tests will help rule out other causes of fever and guide further management.

### 4. Medication Planning (include Name, Dose, Route, Frequency, Duration, Instructions & Contraindications; cite [Card ID | Page])
Since there are no symptoms suggestive of Dengue or Chikungunya, medication planning would focus on managing the common upper respiratory infection. However, it is important to note that the patient should be monitored closely for any signs of worsening symptoms or complications.

#### Medication Details:
- **Paracetamol**: Max 3 g/day in adults (60 mg/kg/day in children).
- **Oral Rehydration Solution (ORS)**: 2400 mL per 24 hours for adults ≥50 kg (or 2 mL/kg/hr for 24 hours if body weight <50 kg).

Instructions:
- Take Paracetamol divided doses as needed for fever.
- Use ORS to maintain hydration throughout the febrile and defervescence phases.

Contraindications:
- NSAIDs, aspirin, and corticosteroids should be avoided due to potential bleeding risks.

### 5. Advice & Follow-Up (cite [Card ID | Page])
For this case, the advice and follow-up plan would be:

- Advise adequate rest under a mosquito net.
- Perform tepid sponging to manage discomfort.
- Encourage a light nutritious diet avoiding dark red/brown foods mimicking blood in vomit/stool.
- Monitor CBC results daily until afebrile for 24-48 hours.
- If any warning signs develop, instruct immediate return to hospital.

Follow-up:
- Repeat CBC once afebrile for 24-48 hours.
- Consider referral

---

## Case 2: Ordinary Hypertension (Grade 2 Primary Care) — Mode: Baseline (740.54s)

### Retrieved Canonical Cards (Baseline Mode — 4 Cards)
- **`HTN_DIAG_01`** (Hypertension | `probable_diagnosis` | Score: `0.2846`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 46-47, 64-65**
- **`HTN_ADV_01`** (Hypertension | `advice` | Score: `0.0779`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 49, 64-65**
- **`HTN_MED_01`** (Hypertension | `medication_guidance` | Score: `0.0715`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 64-65**
- **`DENGUE_MED_01`** (Dengue | `medication_guidance` | Score: `0.0629`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 47-48**


**Mode:** `Baseline` | **Model:** `Qwen/Qwen2.5-1.5B-Instruct (Local)` | **Response Time:** `740.54s`

---
### 1. Missing Information & Applicability Check
The patient's complaint is asymptomatic, but they have been diagnosed with hypertension. The patient has a sedentary lifestyle, high dietary salt intake, and no other significant medical conditions such as diabetes, kidney disease, or cardiovascular issues. The patient does not have any known allergies or pregnancy status.

### 2. Probable Diagnosis (cite [Card ID | Page])
**Probable Diagnosis:** Hypertension (Grade 1)

**Cite:** Bangladesh Guidelines on Hypertension, Page 46-47, 64-65

### 3. Investigations (cite [Card ID | Page])
No specific investigations were mentioned in the provided data.

### 4. Medication Planning (include Name, Dose, Route, Frequency, Duration, Instructions & Contraindications; cite [Card ID | Page])
#### Initial Treatment Plan
**Name:** Amlodipine
**Dose:** 5 mg (2.5 mg starting dose for elderly or low body weight)
**Route:** Oral
**Frequency:** Once daily
**Duration:** Long-term / life-long maintenance with monthly review until target reached
**Instructions:** First-line monotherapy for BP 140-159/90-99 mmHg; combine with Losartan 50 mg immediately if initial BP >= 160/100 mmHg.
**Contraindications:** Pregnant patients or women of childbearing age who may become pregnant

#### Immediate Treatment Plan
**Name:** Amlodipine 5 mg + Losartan 50 mg
**Route:** Oral
**Frequency:** Once daily
**Duration:** Immediate treatment at Step 2
**Instructions:** Combine with Amlodipine 5 mg once daily for Step 2 or as immediate initial therapy if BP >= 160/100 mmHg. Check serum creatinine and potassium.

#### Additional Medication
**Name:** Hydrochlorothiazide
**Dose:** 12.5 mg
**Route:** Oral
**Frequency:** Once daily
**Duration:** Long-term maintenance if Step 2 fails after 1 month
**Instructions:** Added to Amlodipine 5 mg + Losartan 50 mg at Step 3 after checking medication adherence.

**Exclusion:** Do not use this primary care protocol for pregnant patients or children <18 years old (refer to specialist).

**Cite:** Bangladesh Guidelines on Hypertension, Page 64-65

### 5. Advice & Follow-Up (cite [Card ID | Page])
**Advice & Follow-Up:**
- **Lifestyle Modification:** Provide comprehensive lifestyle modification advice including avoiding alcohol and tobacco, physical activity, reducing salt intake, eating a heart-healthy diet, and maintaining a healthy weight.
- **Monthly Monitoring:** Advise monitoring of blood pressure at home and reporting results to healthcare provider.
- **Referral:** Refer to a specialist if there is an acceleration or malignancy of hypertension, suspected secondary hypertension, resistant hypertension, recent target organ damage, pregnancy,

---

## Case 2: Ordinary Hypertension (Grade 2 Primary Care) — Mode: Improved (1022.58s)

### Retrieved Canonical Cards (Improved Mode — 6 Cards)
- **`HTN_DIAG_01`** (Hypertension | `probable_diagnosis` | Score: `0.2846`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 46-47, 64-65**
- **`HTN_INV_01`** (Hypertension | `investigations` | Score: `0.0354`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 51-52, 64**
- **`HTN_MED_01`** (Hypertension | `medication_guidance` | Score: `0.0715`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 64-65**
- **`HTN_ADV_01`** (Hypertension | `advice` | Score: `0.0779`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 49, 64-65**
- **`DENGUE_MED_01`** (Dengue | `medication_guidance` | Score: `0.0629`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 47-48**
- **`CHIK_DIAG_01`** (Chikungunya | `probable_diagnosis` | Score: `0.0611`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 11-15, 18-19**


**Mode:** `Improved` | **Model:** `Qwen/Qwen2.5-1.5B-Instruct (Local)` | **Response Time:** `1022.58s`

---
### 1. Missing Information & Applicability Check
The patient's pregnancy status is **Not Applicable**. The patient has no relevant medical conditions such as hypertension, diabetes, or kidney disease mentioned in the retrieved cards. There is also no mention of any other potential triggers for chikungunya infection.

### 2. Probable Diagnosis (cite [Card ID | Page])
Based on the patient’s complaint of asymptomatic high blood pressure and the retrieved card for Hypertension, the probable diagnosis is **Probable Grade 1 Hypertension**.

### 3. Investigations (cite [Card ID | Page])
To confirm the diagnosis and manage the condition effectively, the following investigations should be ordered:

- **Routine Baseline Investigations**: 
  - Blood Tests: Serum sodium, potassium, serum creatinine, and estimated glomerular filtration rate (eGFR)
  - Lipid Profile
  - Fasting Blood Glucose (if available)
  - Urine Dipstick Analysis
  - 12-Lead ECG

These investigations will help identify any underlying comorbidities and assess the need for antihypertensive therapy.

### 4. Medication Planning (include Name, Dose, Route, Frequency, Duration, Instructions & Contraindications; cite [Card ID | Page])
Given the patient's age and the absence of contraindications, the appropriate medication plan would be:

#### Initial Treatment Plan (Step 1):
- **Medication**: Amlodipine 5 mg once daily
- **Instructions**: Start with 2.5 mg in elderly or low body weight individuals. Monitor for side effects and adjust dosage accordingly.

#### Immediate Next Steps (Step 2):
- **Medication**: Amlodipine 5 mg + Losartan 50 mg once daily
- **Instructions**: This combination is used for initial BP ≥ 160/100 mmHg. Ensure monitoring of serum creatinine and potassium levels.

#### Maintenance Therapy (Step 3):
- **Medication**: Amlodipine 5 mg + Losartan 50 mg + Hydrochlorothiazide 12.5 mg once daily
- **Instructions**: Continue monitoring for efficacy and adjust dosages based on BP control and tolerability.

#### Additional Considerations:
- **Contraindications**: Do not prescribe Losartan, any ACE inhibitor, ARB, or thiazide diuretic to pregnant patients or women of childbearing age who may become pregnant.
- **Adherence Monitoring**: Regularly monitor medication adherence and ensure compliance with the prescribed regimen.

### 5. Advice & Follow-Up (cite [Card ID | Page])
For ongoing management, the following advice should be provided:

- **Lifestyle Modification**:
  - Avoid alcohol and tobacco.
  - Engage in physical activity for at least 2.5 hours per week.
  - Reduce salt intake to less than 1 teaspoon per day.
  - Maintain a heart-healthy diet rich in fruits, vegetables, whole grains, and lean proteins.
  - Lose weight if overweight.

- **Monitoring and Follow-Up**:


---

## Case 3: Ordinary Cholera (Some Dehydration - Plan B) — Mode: Baseline (589.25s)

### Retrieved Canonical Cards (Baseline Mode — 4 Cards)
- **`CHOLERA_INV_01`** (Cholera | `investigations` | Score: `0.2285`)
  - *Source:* WHO Clinical Tools for Cholera Treatment Facilities, **PDF Page: 6, 12**
- **`CHOLERA_DIAG_01`** (Cholera | `probable_diagnosis` | Score: `0.1857`)
  - *Source:* WHO Clinical Tools for Cholera Treatment Facilities, **PDF Page: 5-9, 12, 14**
- **`CHOLERA_MED_02`** (Cholera | `medication_guidance` | Score: `0.1819`)
  - *Source:* WHO Clinical Tools for Cholera Treatment Facilities, **PDF Page: 9, 12**
- **`CHOLERA_ADV_01`** (Cholera | `advice` | Score: `0.1238`)
  - *Source:* WHO Clinical Tools for Cholera Treatment Facilities, **PDF Page: 14**


**Mode:** `Baseline` | **Model:** `Qwen/Qwen2.5-1.5B-Instruct (Local)` | **Response Time:** `589.25s`

---
### 1. Missing Information & Applicability Check
The patient presents with acute profuse watery diarrhea (8 episodes in the last 24 hours), thirst, restlessness, and irritability. The patient is able to drink oral fluids but appears dehydrated based on their symptoms and vitals. There is no mention of any other significant illnesses or allergies, which could affect the diagnosis or management approach.

### 2. Probable Diagnosis (cite [Card ID | Page])
**Probable Diagnosis:** Cholera

### 3. Investigations (cite [Card ID | Page])
**Investigations:**
- **Bedside Clinical Hydration Assessment:** Perform at least every hour during Plan B ORS therapy and continuously during Plan C IV resuscitation.
- **Check Blood Glucose:** Screen for hypoglycemia defined as blood glucose < 3.0 mmol/L or < 54 mg/dL. Treat with IV dextrose if present.

### 4. Medication Planning (include Name, Dose, Route, Frequency, Duration, Instructions & Contraindications; cite [Card ID | Page])
#### Plan C - Severe Dehydration (IV Resuscitation):
- **Medication Details:**
  - **Ringer’s Lactate IV (Total 100 mL/kg):**
    - **Dose:** 100 mL/kg total (30 mL/kg initial bolus + 70 mL/kg continuation).
    - **Route:** Intravenous (IV).
    - **Frequency:** Continuous rapid infusion.
    - **Duration:** 3 hours total for children >1 yr & adults (30 mins bolus + 2.5 hrs); 6 hours total for infants <1 yr (1 hr bolus + 5 hrs).

  - **Dextrose IV (For Hypoglycaemia < 3.0 mmol/L or < 54 mg/dL):**
    - **Dose:** Adults: 25-50 mL of Dextrose 50% OR 125-250 mL of Dextrose 10%.
      - **Children:** 5 mL/kg of Dextrose 10%.
    - **Route:** Intravenous (IV).
    - **Frequency:** Bolus over 2 minutes; recheck glucose at 30 mins and give 2nd bolus if necessary.
    - **Instructions:** If no IV access, 2-5 mL of 50% dextrose fluid can be placed inside the cheek using a syringe (do not use needle or spoon).

#### Contraindications:
- **Contraindications:** None listed in the available cards.

### 5. Advice & Follow-Up (cite [Card ID | Page])
**Advice & Follow-Up:**
- **Before Discharge:**
  - **Provide Oral Rehydration Solution (ORS) Packets:** At least 4 packets for all discharged patients to use at home.
  - **Zinc Tablets:** Sufficient for completing the 10-day treatment.
  - **Counsel Patients and Care

---

## Case 3: Ordinary Cholera (Some Dehydration - Plan B) — Mode: Improved (969.56s)

### Retrieved Canonical Cards (Improved Mode — 6 Cards)
- **`CHOLERA_DIAG_01`** (Cholera | `probable_diagnosis` | Score: `0.1857`)
  - *Source:* WHO Clinical Tools for Cholera Treatment Facilities, **PDF Page: 5-9, 12, 14**
- **`CHOLERA_INV_01`** (Cholera | `investigations` | Score: `0.2285`)
  - *Source:* WHO Clinical Tools for Cholera Treatment Facilities, **PDF Page: 6, 12**
- **`CHOLERA_MED_02`** (Cholera | `medication_guidance` | Score: `0.1819`)
  - *Source:* WHO Clinical Tools for Cholera Treatment Facilities, **PDF Page: 9, 12**
- **`CHOLERA_ADV_01`** (Cholera | `advice` | Score: `0.1238`)
  - *Source:* WHO Clinical Tools for Cholera Treatment Facilities, **PDF Page: 14**
- **`DENGUE_MED_01`** (Dengue | `medication_guidance` | Score: `0.1188`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 47-48**
- **`CHIK_MED_01`** (Chikungunya | `medication_guidance` | Score: `0.0937`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 18-20, 26**


**Mode:** `Improved` | **Model:** `Qwen/Qwen2.5-1.5B-Instruct (Local)` | **Response Time:** `969.56s`

---
### 1. Missing Information & Applicability Check
The patient presents with acute profuse watery diarrhea (8 episodes in the last 24 hours), thirst, restlessness, irritability, and elevated blood glucose levels (4.5 mmol/L or 81 mg/dL). The patient is able to drink oral fluids but does not appear dehydrated based on the available information. The patient is not pregnant or elderly, nor do they have any documented history of hypoglycemia. However, there is insufficient information to determine the exact dehydration severity or whether the patient falls into the high-risk category for cholerazyme.

### 2. Probable Diagnosis (cite [Card ID | Page])
**Probable Diagnosis:** Cholera

### 3. Investigations (cite [Card ID | Page])
**Investigations:** 
- **Bedside Hydration Assessment**
- **Baseline Blood Glucose Measurement**

### 4. Medication Planning (include Name, Dose, Route, Frequency, Duration, Instructions & Contraindications; cite [Card ID | Page])
#### Plan A - Oral ORS at Home/Outpatient
- **Name:** Oral Rehydration Solution (ORS)
- **Dose:** 2400 mL per 24 hours for adults >=50 kg (or 2 mL/kg/hour for 24 hours if body weight <50 kg)
- **Route:** Oral
- **Frequency:** Spread evenly across the 24-hour day
- **Duration:** Throughout acute febrile and defervescence phase
- **Instructions:** Use ORS, green coconut water, fruit juices, or soup containing electrolytes rather than plain water alone.
- **Contraindications:** None specified

#### Plan B - Monitored 4-Hour ORS Therapy in Facility
- **Name:** Oral Rehydration Solution (ORS)
- **Dose:** 2400 mL per 24 hours for adults >=50 kg (or 2 mL/kg/hour for 24 hours if body weight <50 kg)
- **Route:** Oral
- **Frequency:** 4-hourly throughout the day
- **Duration:** Until signs of improvement
- **Instructions:** Monitor closely for signs of worsening dehydration or other complications
- **Contraindications:** None specified

#### Plan C - Immediate IV Ringer's Lactate Resuscitation
- **Name:** Intravenous Ringer's Lactate
- **Dose:** Total 100 mL/kg (e.g., for >=55 kg: 2000 mL in 30 mins + 4000 mL in 2.5 hrs)
- **Route:** Intravenous (IV)
- **Frequency:** Continuous rapid infusion
- **Duration:** 3 hours total for children >1 yr & adults (30 mins bolus + 2.5 hrs); 6 hours total for infants <1 yr (1 hr bolus + 5 hrs)
- **Instructions:** Administer through an appropriate infusion set
- **Contraindications:** None specified

### 

---

## Case 4: Ordinary Chikungunya (Acute Symmetric Arthritis) — Mode: Baseline (640.95s)

### Retrieved Canonical Cards (Baseline Mode — 4 Cards)
- **`CHIK_DIAG_01`** (Chikungunya | `probable_diagnosis` | Score: `0.1829`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 11-15, 18-19**
- **`CHIK_MED_01`** (Chikungunya | `medication_guidance` | Score: `0.1353`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 18-20, 26**
- **`DIFF_DENGUE_CHIK_01`** (Dengue / Chikungunya | `probable_diagnosis` | Score: `0.1252`)
  - *Source:* National Guideline for Clinical Management of Dengue (5th Ed) & National Guideline on Chikungunya Management (2017), **PDF Page: Dengue Page 29; Chikungunya Pages 16-18**
- **`DENGUE_DIAG_01`** (Dengue | `probable_diagnosis` | Score: `0.1054`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 26-28, 45-47**


**Mode:** `Baseline` | **Model:** `Qwen/Qwen2.5-1.5B-Instruct (Local)` | **Response Time:** `640.95s`

---
### 1. Missing Information & Applicability Check
The patient presents with sudden high fever (39.0°C) accompanied by severe symmetric joint pain and swelling in wrists, ankles, and small hand joints, which are typical symptoms of chikungunya. The patient also mentions that he resides in the Dhaka area, which indicates exposure to the virus due to its active transmission there. However, the patient does not mention any history of travel outside the region or recent contact with infected individuals.

### 2. Probable Diagnosis (cite [Card ID | Page])
Based on the patient's symptoms and location, the probable diagnosis is **Chikungunya**. This is supported by the following card:

- **Card ID**: CHIK_DIAG_01
- **Category**: probable_diagnosis
- **Prerequisites**: Sudden/acute onset of high fever (> 38.5°C / 101.3°F, typically lasting 24-48 hours), Severe arthralgia or arthritis (typically symmetric, involving ankles, wrists, and small joints of hands, worse in the morning, relieved by mild exercise, or causing a stooped/bending posture).
- **Action**: Categorize diagnosis as: Possible Case (meets clinical criteria of acute fever >38.5°C + severe arthralgia/arthritis), Probable Case (meets clinical criteria + epidemiological criteria of residing in/visiting an epidemic area within 15 days), or Confirmed Case (laboratory confirmed).

### 3. Investigations (cite [Card ID | Page])
Given the probable diagnosis of Chikungunya, the necessary investigations include:

- **Laboratory Tests**:
  - **Serology**: To confirm the presence of specific antibodies against Chikungunya virus (IgM/IgG tests).
  - **Viral Load Testing**: PCR testing for Chikungunya RNA to determine viral load levels.
  - **Immunoglobulin G (IgG) Antibody Titers**: Elevated titers suggest past infection but do not definitively diagnose current infection.
  
- **Blood Tests**:
  - Complete Blood Count (CBC): To assess hematologic parameters such as platelets, white blood cells, and hemoglobin levels.
  - Coagulation Profile: To evaluate clotting factors and screen for potential complications like disseminated intravascular coagulation (DIC).
  - Liver Function Tests (LFTs): To rule out hepatic involvement.
  - Renal Function Tests: To exclude renal involvement.

### 4. Medication Planning (include Name, Dose, Route, Frequency, Duration, Instructions & Contraindications; cite [Card ID | Page])
For Chikungunya, the medication planning includes:

- **Paracetamol**:
  - **Name**: Paracetamol
  - **Dose**: Adults: up to 1000 mg per dose (up to 4 times daily, max 4000 mg/day if no liver/kidney disease)
  - **Route**: Oral
  - **Frequency**: Up to 4 times daily

---

## Case 4: Ordinary Chikungunya (Acute Symmetric Arthritis) — Mode: Improved (854.46s)

### Retrieved Canonical Cards (Improved Mode — 6 Cards)
- **`CHIK_DIAG_01`** (Chikungunya | `probable_diagnosis` | Score: `0.1829`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 11-15, 18-19**
- **`CHIK_INV_01`** (Chikungunya | `investigations` | Score: `0.0565`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 11, 21-22, 26**
- **`CHIK_MED_01`** (Chikungunya | `medication_guidance` | Score: `0.1353`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 18-20, 26**
- **`CHIK_ADV_01`** (Chikungunya | `advice` | Score: `0.1021`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 18-22, 26-27**
- **`DIFF_DENGUE_CHIK_01`** (Dengue / Chikungunya | `probable_diagnosis` | Score: `0.1252`)
  - *Source:* National Guideline for Clinical Management of Dengue (5th Ed) & National Guideline on Chikungunya Management (2017), **PDF Page: Dengue Page 29; Chikungunya Pages 16-18**
- **`DENGUE_DIAG_01`** (Dengue | `probable_diagnosis` | Score: `0.1054`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 26-28, 45-47**


**Mode:** `Improved` | **Model:** `Qwen/Qwen2.5-1.5B-Instruct (Local)` | **Response Time:** `854.46s`

---
### 1. Missing Information & Applicability Check
The patient presents with sudden high fever (39.0°C) accompanied by severe symmetric joint pain and swelling in wrists, ankles, and small hand joints, worsening in the morning and causing a stooped posture. The patient's history includes recent travel to areas with active chikungunya transmission, which suggests this could be a case of chikungunya. However, there is no mention of any other diseases that might complicate the diagnosis or necessitate further investigation.

### 2. Probable Diagnosis (cite [Card ID | Page])
Based on the patient’s symptoms and travel history, the most likely diagnosis is **chikungunya**. This is supported by the sudden onset of high fever, severe joint pain, and the presence of a rash typical of chikungunya.

### 3. Investigations (cite [Card ID | Page])
To confirm the diagnosis and rule out other potential causes, the following investigations should be ordered:

- **CBC**: To assess leukocyte and platelet counts.
- **ESR**: Elevated ESR indicates inflammation.
- **CRP**: Increased CRP levels suggest infection.
- **SGPT**: Elevated SGPT levels indicate liver involvement.

Additionally, if necessary, real-time RT-PCR for Chikungunya viral RNA or virus isolation can be performed within 5 days of symptom onset to confirm the diagnosis.

### 4. Medication Planning (include Name, Dose, Route, Frequency, Duration, Instructions & Contraindications; cite [Card ID | Page])
For chikungunya, the following medications are recommended:

- **Paracetamol**: Up to 1000 mg per dose (up to 4 times daily, max 4000 mg/day if no liver/kidney disease).
- **Oral Rehydration Solutions (ORS)**: Approximately 2 liters per 24 hours.
- **Antihistamines**: Standard symptomatic dose if skin itching or pruritus is present.

These treatments are given during the acute phase (first 7-10 days).

### 5. Advice & Follow-Up (cite [Card ID | Page])
Advice for the patient during the acute phase includes:

- Adequate rest in a warm environment.
- Refrain from exertion and applying cold compresses to painful joints to reduce joint damage.
- Strictly avoid heat application and do not perform formal physiotherapy in the acute phase.

After 7-10 days (post-acute phase):

- Recommend mild exercises such as walking on level ground, active hand movements, and proper joint posturing to prevent stiffness.
- Refer patients with persistent arthralgia or loss of autonomy to an arthralgia clinic or physical medicine specialist for rehabilitation.
- Prevent mosquito transmission by daytime-biting Aedes control and mosquito net use.

Follow-up is important to monitor for complications and adjust management accordingly. If the patient develops any new symptoms or worsens, they should seek medical attention promptly.

### Conclusion
Given the patient's presentation and travel history, chikungunya appears to be the most likely diagnosis. Immediate investigations and appropriate medication planning are essential.

---

## Case 5: Ambiguous / Incomplete Febrile Case — Mode: Baseline (564.65s)

### Retrieved Canonical Cards (Baseline Mode — 4 Cards)
- **`CHIK_DIAG_01`** (Chikungunya | `probable_diagnosis` | Score: `0.1375`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 11-15, 18-19**
- **`CHIK_ADV_01`** (Chikungunya | `advice` | Score: `0.0776`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 18-22, 26-27**
- **`DENGUE_DIAG_01`** (Dengue | `probable_diagnosis` | Score: `0.0747`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 26-28, 45-47**
- **`DIFF_DENGUE_CHIK_01`** (Dengue / Chikungunya | `probable_diagnosis` | Score: `0.0633`)
  - *Source:* National Guideline for Clinical Management of Dengue (5th Ed) & National Guideline on Chikungunya Management (2017), **PDF Page: Dengue Page 29; Chikungunya Pages 16-18**


**Mode:** `Baseline` | **Model:** `Qwen/Qwen2.5-1.5B-Instruct (Local)` | **Response Time:** `564.65s`

---
### 1. Missing Information & Applicability Check
The patient's complaint includes fever, headache, generalized body and joint ache, and mild skin rash. The duration is unknown, and no specific medical history or allergies have been reported. The patient's demographics include age 30, sex female, and weight unknown. There is no mention of pregnancy status or vital signs. The medications, allergy history, and other relevant health information are also absent.

### 2. Probable Diagnosis (cite [Card ID | Page])
Based on the patient’s complaints of fever, headache, generalized body and joint ache, and mild skin rash, the most probable diagnosis is **Chikungunya**. This is supported by the card "CHIK_DIAG_01" which states that the patient should be categorized as either a possible case, probable case, or confirmed case based on their clinical presentation and epidemiological criteria. 

### 3. Investigations (cite [Card ID | Page])
Given the probable diagnosis of Chikungunya, the following investigations would be appropriate:

- **Laboratory Tests**: 
  - **Serology**: Perform serological tests such as IgM antibodies against Chikungunya virus to confirm the diagnosis. These tests may show a higher titre compared to Dengue.
  - **NS1 Antigen Test**: Detects viral antigens in serum samples, indicating recent infection.
  - **RT-PCR**: Amplifies the viral genome directly from blood or tissue samples, providing rapid results but requires specialized equipment.
  
- **Imaging Studies**: 
  - **X-ray or MRI**: To rule out other causes of joint pain and assess for any complications like osteoarthritis or sepsis.
  
- **Other Tests**: 
  - **Complete Blood Count (CBC)**: To monitor platelets and haemoglobin levels, which might indicate hematologic changes associated with Chikungunya.
  - **Lymphocyte Count**: Lower than normal in Chikungunya due to immune system activation.

### 4. Medication Planning (include Name, Dose, Route, Frequency, Duration, Instructions & Contraindications; cite [Card ID | Page])
For Chikungunya, the medication planning involves managing the symptoms and preventing complications. However, there are no contraindications mentioned for standard antipyretics, analgesics, and nonsteroidal anti-inflammatory drugs (NSAIDs) in this context. Here is a general approach:

- **Antipyretics**: Use acetaminophen or paracetamol for fever reduction. Avoid aspirin and NSAIDs due to increased risk of bleeding when the condition is undetermined.
- **Analgesics**: Apply cold compresses to relieve joint pain and inflammation.
- **Non-Steroidal Anti-Inflammatory Drugs (NSAIDs)**: If necessary, consider low-dose ibuprofen or naproxen sodium, but under close supervision to avoid potential side effects.
- **Vitamin B Complex**: May help manage fatigue and muscle weakness associated with Chikungunya.

### 5. Advice & Follow-Up (cite [Card ID | Page])
Advice for the patient includes:

- **Rest**:

---

## Case 5: Ambiguous / Incomplete Febrile Case — Mode: Improved (811.18s)

### Retrieved Canonical Cards (Improved Mode — 6 Cards)
- **`CHIK_DIAG_01`** (Chikungunya | `probable_diagnosis` | Score: `0.1375`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 11-15, 18-19**
- **`DENGUE_INV_01`** (Dengue | `investigations` | Score: `0.0402`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 37-39, 41, 45, 48**
- **`DENGUE_MED_01`** (Dengue | `medication_guidance` | Score: `0.0613`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 47-48**
- **`CHIK_ADV_01`** (Chikungunya | `advice` | Score: `0.0776`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 18-22, 26-27**
- **`DENGUE_DIAG_01`** (Dengue | `probable_diagnosis` | Score: `0.0747`)
  - *Source:* National Guideline for Clinical Management of Dengue, **PDF Page: 26-28, 45-47**
- **`DIFF_DENGUE_CHIK_01`** (Dengue / Chikungunya | `probable_diagnosis` | Score: `0.0633`)
  - *Source:* National Guideline for Clinical Management of Dengue (5th Ed) & National Guideline on Chikungunya Management (2017), **PDF Page: Dengue Page 29; Chikungunya Pages 16-18**


**Mode:** `Improved` | **Model:** `Qwen/Qwen2.5-1.5B-Instruct (Local)` | **Response Time:** `811.18s`

---
### 1. Missing Information & Applicability Check
The patient's complaint includes fever, headache, generalized body and joint ache, and mild skin rash. The duration of the complaints is unknown, but it seems they have been ongoing for some time. The patient's demographics include age 30, sex female, and weight unknown. There is no mention of any pregnancy status or vials. Additionally, there is no record of any medical history, allergies, or medications taken by the patient.

### 2. Probable Diagnosis (cite [Card ID | Page])
Based on the patient’s symptoms and the available card information, the most likely diagnoses are **Chikungunya** and **Dengue**. However, since the patient does not meet the specific criteria for either condition, we will proceed with ruling out Dengue first.

#### Card ID: CHIK_DIAG_01
- **Category**: probable_diagnosis
- **Prerequisites**: Sudden/acute onset of high fever (> 38.5 C / 101.3 F, typically lasting 24-48 hours), Severe arthralgia or arthritis (typically symmetric, involving ankles, wrists, and small joints of hands, worse in the morning, relieved by mild exercise, or causing a stooped/bending posture) and/or maculopapular rash.
- **Action**: Categorize diagnosis as: Possible Case (meets clinical criteria of acute fever >38.5 C + severe arthralgia/arthritis), Probable Case (meets clinical criteria + epidemiological criteria of residing in/visiting an epidemic area within 15 days), or Confirmed Case (laboratory confirmed).
- **Medication Details**: []
- **Exclusions or Missing Info**: Check Hospital Admission Criteria (Page 19): hemodynamic instability (syncope, SBP <90 mmHg, pulse pressure <30 mmHg), oliguria (<500 mL/24 hrs), altered sensorium, bleeding, persistent disabling joint pain after 3 days of treatment, age >60 years, infants <1 year, pregnancy, or high-risk comorbidities (HTN, diabetes, CAD/CVD, COPD, co-infection with Dengue/TB/Malaria).

#### Card ID: DENGUE_INV_01
- **Category**: investigations
- **Prerequisites**: Suspected or probable Dengue fever, Duration of fever known (<= 5 days vs. > 5 days from onset)
- **Action**: Order baseline Complete Blood Count (CBC) with Haematocrit (Hct) and platelet count, Dengue NS1 Antigen test (or RT-PCR), and liver transaminases (SGOT/AST, SGPT/ALT).
- **Medication Details**: []
- **Exclusions or Missing Info**: Missing information to check: Exact day of fever onset is mandatory to choose between NS1 Antigen (days 1-5) and Dengue IgM/IgG antibody (day 6+)

### 3. Investigations (cite [Card ID | Page])
- **Card

---

## Case 6: Modified Case 2 (Hypertension in Pregnant / Childbearing Female) — Mode: Baseline (790.9s)

### Retrieved Canonical Cards (Baseline Mode — 4 Cards)
- **`HTN_DIAG_01`** (Hypertension | `probable_diagnosis` | Score: `0.2076`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 46-47, 64-65**
- **`HTN_MED_02`** (Hypertension | `medication_guidance` | Score: `0.1536`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 64-65**
- **`HTN_MED_01`** (Hypertension | `medication_guidance` | Score: `0.1297`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 64-65**
- **`CHIK_MED_01`** (Chikungunya | `medication_guidance` | Score: `0.0924`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 18-20, 26**


**Mode:** `Baseline` | **Model:** `Qwen/Qwen2.5-1.5B-Instruct (Local)` | **Response Time:** `790.89s`

---
### 1. Missing Information & Applicability Check
The patient's complaint includes asymptomatic elevated blood pressure detected today. The patient is 29 years old, female, and currently 8 weeks pregnant. She does not report any headaches, visual disturbances, or chest pain. Her vital signs show an office systolic blood pressure (SBP) of 165 mmHg and diastolic blood pressure (DBP) of 102 mmHg. The patient has no history of chronic kidney disease, diabetes, or cardiovascular disease. The pregnancy status is noted as being within the first trimester.

### 2. Probable Diagnosis (cite [Card ID | Page])
Based on the patient’s symptoms, vitals, and pregnancy status, the probable diagnosis is **Probable Grade 1 Hypertension**. This classification is supported by the following card:

- **Card ID:** HTN_DIAG_01
- **Page:** Bangladesh Guidelines on Hypertension, Page 46-47, 64-65

This card outlines the management strategy for patients with elevated blood pressure, including the need for confirmation through multiple readings over time and consideration of potential complications such as hypertensive-mediated organ damage (HMOD).

### 3. Investigations (cite [Card ID | Page])
Given the patient’s condition, the necessary investigations include:

- **Office Blood Pressure Measurement:** To confirm the elevated reading and monitor progression.
- **Lying and Standing Blood Pressure Measurements:** To rule out orthostatic hypotension.
- **Pregnancy Test:** To ensure the patient is indeed in her first trimester and to assess for gestational hypertension.

These tests will help determine whether the patient meets the criteria for referral to a specialist or initiation of treatment according to the guidelines.

### 4. Medication Planning (include Name, Dose, Route, Frequency, Duration, Instructions & Contraindications; cite [Card ID | Page])
#### Initial Treatment Plan
For the patient, the initial treatment plan should follow the recommendations from Card ID HTN_MED_02:

- **Medication:** Losartan 50 mg once daily.
- **Instructions:** Refer to a specialist if the target blood pressure is not achieved within two months.
- **Duration:** Long-term maintenance.

#### Additional Considerations
Since the patient is pregnant, she should not take losartan or other medications that can cause fetal harm. Therefore, the next step would be to consult a specialist to discuss alternative options based on her pregnancy status.

### 5. Advice & Follow-Up (cite [Card ID | Page])
After initiating the initial treatment, the patient should be advised to:

- **Monitor Blood Pressure Regularly:** At least three readings per visit across two to three visits, or after two weeks per primary care protocol, or via ambulatory blood pressure monitoring (ABPM).
- **Adherence to Medication:** Ensure proper adherence to the prescribed regimen.
- **Gestational Complications Monitoring:** Keep track of any additional symptoms or concerns related to pregnancy, such as swelling, shortness of breath, or unusual fatigue.

The patient should also be informed about the importance of maintaining

---

## Case 6: Modified Case 2 (Hypertension in Pregnant / Childbearing Female) — Mode: Improved (1061.26s)

### Retrieved Canonical Cards (Improved Mode — 6 Cards)
- **`HTN_DIAG_01`** (Hypertension | `probable_diagnosis` | Score: `0.2076`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 46-47, 64-65**
- **`HTN_INV_01`** (Hypertension | `investigations` | Score: `0.069`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 51-52, 64**
- **`HTN_MED_02`** (Hypertension | `medication_guidance` | Score: `0.1536`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 64-65**
- **`HTN_ADV_01`** (Hypertension | `advice` | Score: `0.0556`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 49, 64-65**
- **`HTN_MED_01`** (Hypertension | `medication_guidance` | Score: `0.1297`)
  - *Source:* Bangladesh Guidelines on Hypertension, **PDF Page: 64-65**
- **`CHIK_MED_01`** (Chikungunya | `medication_guidance` | Score: `0.0924`)
  - *Source:* National Guideline on Chikungunya Management, **PDF Page: 18-20, 26**


**Mode:** `Improved` | **Model:** `Qwen/Qwen2.5-1.5B-Instruct (Local)` | **Response Time:** `1061.26s`

---
### 1. Missing Information & Applicability Check
The patient's pregnancy status is noted as being 8 weeks pregnant, which places her in the category of "women of childbearing age" according to the guidelines. However, there is no mention of whether she is currently pregnant or if she might become pregnant soon. Additionally, the patient does not have any documented comorbid conditions such as diabetes, CKD, or other cardiovascular diseases that would affect the choice of medications.

### 2. Probable Diagnosis (cite [Card ID | Page])
The probable diagnosis based on the patient’s complaint and findings is **Hypertension**. The patient’s blood pressure reading of 165/102 mmHg indicates Stage 2 Hypertension, which falls under the category of **Probable Grade 1 Hypertension** according to the Bangladesh Guidelines on Hypertension.

### 3. Investigations (cite [Card ID | Page])
To confirm the diagnosis and assess potential complications, the following investigations should be ordered:

- **Routine Baseline Investigations**: 
  - Serum sodium, potassium, serum creatinine, and estimated glomerular filtration rate (eGFR).
  - Lipid profile and fasting blood glucose (if available).
  - Urine dipstick analysis (and urine albumin:creatinine ratio if renal disease suspected).

These tests will help identify any underlying conditions that could contribute to or exacerbate the patient’s hypertension.

### 4. Medication Planning (include Name, Dose, Route, Frequency, Duration, Instructions & Contraindications; cite [Card ID | Page])
Given the patient’s pregnancy status and the need to avoid certain medications due to their contraindications, the recommended medication plan is as follows:

#### Initial Treatment Plan (for a woman of childbearing age):
- **Amlodipine 5 mg once daily** (Step 1 of the Women of Childbearing Age Pathway).
- **Losartan 50 mg once daily** (immediate initiation if initial BP ≥ 160/100 mmHg).

#### Maintenance Therapy:
- **Amlodipine 5 mg once daily** (Step 1 of the Women of Childbearing Age Pathway).
- **Losartan 50 mg once daily** (Step 2 of the Women of Childbearing Age Pathway).
- **Hydrochlorothiazide 12.5 mg once daily** (Step 3 of the Women of Childbearing Age Pathway) if necessary.

#### Additional Considerations:
- **Monitoring**: Regular monitoring of blood pressure, serum creatinine levels, and potassium concentrations.
- **Adherence**: Ensure consistent medication adherence, particularly focusing on taking the prescribed doses correctly.
- **Special Considerations**: Pregnant women should avoid the use of Losartan and any ACE inhibitors, ARBs, and thiazides. They should also avoid aspirin and NSAIDs during the first 10 days of the acute stage of chikungunya infection.

### 5. Advice & Follow-Up (cite [Card ID | Page])
For ongoing management, the following advice and follow-up

---

