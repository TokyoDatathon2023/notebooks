| name                           | type    | description                                                                                                | 説明                                       |
| ------------------------------ | ------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| subject_id                     | int64   | Unique identifier for each patient                                                                         | 各患者の固有の識別子                               |
| stay_id                        | int64   | Unique identifier for each ward stay                                                                       | 各病棟への入院（入室）ごとの固有の識別子                     |
| SaO2_timestamp                 | object  | Timestamp for SaO2 measurement                                                                             | SaO2測定のタイムスタンプ                           |
| SaO2                           | float64 | Arterial oxygen saturation                                                                                 | 動脈血酸素飽和度                                 |
| delta_SpO2                     | int64   | Time offset (in minutes) in the measurement of peripheral oxygen saturation                                | 末梢血酸素飽和度測定の時間オフセット（分）                    |
| SpO2                           | int64   | Peripheral oxygen saturation                                                                               | 末梢血酸素飽和度                                 |
| hidden_hypoxemia               | int64   | Indicates if the patient had hypoxemia without clinical signs                                              | 患者が潜在性低酸素血症であったかどうか                      |
| hadm_id                        | int64   | Unique identifier for each hospital admission                                                              | 各入院の固有の識別子                               |
| gender                         | object  | Gender of the patient                                                                                      | 患者の性別                                    |
| sex_female                     | int64   | Indicates if the patient is female                                                                         | 患者が女性であるかどうか                             |
| anchor_age                     | int64   | Age of the patient at the time of admission                                                                | 入院時の患者の年齢                                |
| race                           | object  | Race of the patient                                                                                        | 患者の人種                                    |
| race_group                     | object  | Grouping of race into broader categories                                                                   | より広範な人種のカテゴリ                             |
| language                       | object  | Primary language spoken by the patient                                                                     | 患者が主に話す言語                                |
| insurance                      | object  | Type of insurance of the patient                                                                           | 患者の保険の種類                                 |
| weight                         | float64 | Weight of the patient in kilograms                                                                         | 患者の体重（キログラム）                             |
| height                         | float64 | Height of the patient in centimeters                                                                       | 患者の身長（センチメートル）                           |
| BMI                            | float64 | Body Mass Index of the patient                                                                             | 患者のBMI                                   |
| anchor_year_group              | object  | Grouping of admission year into broader categories                                                         | 入院年をより広いカテゴリに分類したもの                      |
| first_hosp_stay                | bool    | Indicates if this is the first hospital stay for the patient                                               | 患者の初めての入院かどうか                            |
| first_icu_stay                 | bool    | Indicates if this is the first ICU stay for the patient                                                    | 患者の初めてのICU入室かどうか                         |
| icustay_seq                    | int64   | Sequence number of ICU stay for the patient                                                                | 患者のICU入室の通し番号                            |
| admittime                      | object  | Timestamp for hospital admission                                                                           | 入院のタイムスタンプ                               |
| dischtime                      | object  | Timestamp for hospital discharge                                                                           | 退院のタイムスタンプ                               |
| icu_intime                     | object  | Timestamp for ICU admission                                                                                | ICU入室のタイムスタンプ                            |
| icu_outtime                    | object  | Timestamp for ICU discharge                                                                                | ICU退室のタイムスタンプ                            |
| los_hospital                   | int64   | Length of hospital stay in days                                                                            | 入院期間（日数）                                 |
| los_icu                        | float64 | Length of ICU stay in days                                                                                 | ICU入室期間（日数）                              |
| CCI                            | int64   | Charlson Comorbidity Index                                                                                 | チャールソン合併症指数                              |
| SOFA_admission                 | int64   | Sequential Organ Failure Assessment (SOFA) score at admission                                              | 入院時の SOFA スコア                            |
| mortality_in                   | int64   | Indicates if the patient died during the hospital stay                                                     | 入院中に患者が死亡したかどうか                          |
| delta_vent_start               | float64 | Time since ventilation started (in minutes) at the time of the measurement                                 | 測定時点での人工呼吸開始からの経過時間（分）                   |
| ventilation_status             | object  | Indicates if the patient was on mechanical ventilation                                                     | 患者に人工呼吸を行ったかどうか                          |
| invasive_vent                  | int64   | Indicates if the patient was on invasive mechanical ventilation                                            | 患者に侵襲的人工呼吸を行ったかどうか                       |
| delta_FiO2                     | float64 | Time offset (in minutes) in the measurement of inspired oxygen (FiO2)                                      | 吸入酸素濃度（FiO2）測定の時間オフセット（分）                |
| FiO2                           | float64 | Fraction of inspired oxygen                                                                                | 吸入酸素濃度                                   |
| delta_rrt                      | float64 | Time since renal replacement therapy (in minutes) at the time of the measurement                           | 測定時点での腎代替療法開始からの経過時間（分）                  |
| rrt                            | int64   | Indicates if the patient was on renal replacement therapy                                                  | 患者が腎代替療法を受けていたかどうか                       |
| delta_vp_start                 | float64 | Time since vasopressor therapy started (in minutes) at the time of the measurement                         | 測定時点での血管収縮薬開始からの経過時間（分）                  |
| norepinephrine_equivalent_dose | float64 | Dose of norepinephrine equivalent to other vasopressors (in mcg/kg/min)                                    | ノルアドレナリン換算の血管収縮薬の投与量（mcg/kg/min）         |
| delta_sofa_coag                | float64 | Time offset (in minutes) in the measurement of SOFA score for coagulation from the previous measurement    | 前回の測定からの凝固能SOFAスコア測定の時間オフセット（分）          |
| sofa_coag                      | float64 | SOFA score for coagulation                                                                                 | 凝固能のSOFAスコア                              |
| delta_sofa_liver               | float64 | Time offset (in minutes) in the measurement of SOFA score for liver from the previous measurement          | 前回の測定からの肝機能SOFAスコア測定の時間オフセット（分）          |
| sofa_liver                     | float64 | SOFA score for liver                                                                                       | 肝機能のSOFAスコア                              |
| delta_sofa_cv                  | int64   | Time offset (in minutes) in the measurement of SOFA score for cardiovascular from the previous measurement | 前回の測定からの循環器SOFAスコア測定の時間オフセット（分）          |
| sofa_cv                        | int64   | Cardiovascular component of Sequential Organ Failure Assessment (SOFA) score                               | 循環器SOFAスコア                               |
| delta_sofa_cns                 | float64 | Time offset (in minutes) in the measurement of central nervous system component of SOFA                    | 前回の測定からの中枢神経系のSOFAスコア測定の時間オフセット（分）       |
| sofa_cns                       | float64 | Central nervous system component of SOFA score                                                             | 中枢神経系のSOFAスコア                            |
| delta_sofa_renal               | float64 | Time offset (in minutes) in the measurement of renal component of SOFA                                     | 前回の測定からの腎機能のSOFAスコア測定の時間オフセット（分）         |
| sofa_renal                     | float64 | Renal component of SOFA score                                                                              | 腎機能のSOFAスコア成分                            |
| delta_sofa_resp                | float64 | Time offset (in minutes) in the measurement of respiratory component of SOFA                               | 前回の測定からの呼吸器系のSOFAスコア測定の時間オフセット（分）        |
| sofa_resp                      | float64 | Respiratory component of SOFA score                                                                        | 呼吸器系のSOFAスコア成分                           |
| delta_hemoglobin               | float64 | Time offset (in minutes) in the measurement of hemoglobin level                                            | ヘモグロビン値測定の時間オフセット（分）                     |
| hemoglobin                     | float64 | Hemoglobin level                                                                                           | ヘモグロビン値                                  |
| delta_hematocrit               | float64 | Time offset (in minutes) in the measurement of Change in hematocrit level                                  | ヘマトクリット値の変化測定の時間オフセット（分）                 |
| hematocrit                     | float64 | Hematocrit level                                                                                           | ヘマトクリット値                                 |
| delta_mch                      | float64 | Time offset (in minutes) in the measurement of mean corpuscular hemoglobin                                 | 平均赤血球ヘモグロビン（MCH）測定の時間オフセット（分）            |
| mch                            | float64 | Mean corpuscular hemoglobin                                                                                | 平均赤血球ヘモグロビン                              |
| delta_mchc                     | float64 | Time offset (in minutes) in the measurement of mean corpuscular hemoglobin concentration                   | 平均赤血球ヘモグロビン濃度（MCHC）測定の時間オフセット（分）         |
| mchc                           | float64 | Mean corpuscular hemoglobin concentration                                                                  | 平均赤血球ヘモグロビン濃度                            |
| delta_mcv                      | float64 | Time offset (in minutes) in the measurement of mean corpuscular volume                                     | 平均赤血球体積（MCV）測定の時間オフセット（分）                |
| mcv                            | float64 | Mean corpuscular volume                                                                                    | 平均赤血球体積                                  |
| delta_platelet                 | float64 | Time offset (in minutes) in the measurement of platelet count                                              | 血小板数測定の時間オフセット（分）                        |
| platelet                       | float64 | Platelet count                                                                                             | 血小板数                                     |
| delta_rbc                      | float64 | Time offset (in minutes) in the measurement of red blood cell count                                        | 赤血球数測定の時間オフセット（分）                        |
| rbc                            | float64 | Red blood cell count                                                                                       | 赤血球数                                     |
| delta_rdw                      | float64 | Time offset (in minutes) in the measurement of Change in red cell distribution width                       | 赤血球分布幅の変化測定の時間オフセット（分）                   |
| rdw                            | float64 | Red cell distribution width                                                                                | 赤血球分布幅                                   |
| delta_wbc                      | float64 | Time offset (in minutes) in the measurement of white blood cell count                                      | 白血球数測定の時間オフセット（分）                        |
| wbc                            | float64 | White blood cell count                                                                                     | 白血球数                                     |
| delta_d_dimer                  | float64 | Time offset (in minutes) in the measurement of Change in D-dimer                                           | D-ダイマーの変化測定の時間オフセット（分）                   |
| d_dimer                        | float64 | D-dimer level                                                                                              | D-ダイマー値                                  |
| delta_fibrinogen               | float64 | Time offset (in minutes) in the measurement of fibrinogen level                                            | フィブリノゲン値測定の時間オフセット（分）                    |
| fibrinogen                     | float64 | Fibrinogen level                                                                                           | フィブリノゲン値                                 |
| delta_thrombin                 | float64 | Time offset (in minutes) in the measurement of thrombin time                                               | トロンビン時間測定の時間オフセット（分）                     |
| thrombin                       | float64 | Thrombin time                                                                                              | トロンビン時間                                  |
| delta_inr                      | float64 | Time offset (in minutes) in the measurement of Change in international normalized ratio (INR)              | 国際標準化比（INR）の変化測定の時間オフセット（分）              |
| inr                            | float64 | International normalized ratio (INR)                                                                       | 国際標準化比（INR）                              |
| delta_pt                       | float64 | Time offset (in minutes) in the measurement of prothrombin time (PT)                                       | プロトロンビン時間（PT）測定の時間オフセット（分）               |
| pt                             | float64 | Prothrombin time (PT)                                                                                      | プロトロンビン時間（PT）                            |
| delta_ptt                      | float64 | Time offset (in minutes) in the measurement of partial thromboplastin time (PTT)                           | 部分トロンボプラスチン時間（PTT）測定の時間オフセット（分）          |
| ptt                            | float64 | Partial thromboplastin time (PTT)                                                                          | 部分トロンボプラスチン時間（PTT）                       |
| delta_alt                      | float64 | Time offset (in minutes) in the measurement of alanine transaminase (ALT) level                            | アラニンアミノトランスフェラーゼ（ALT）測定の時間オフセット（分）       |
| alt                            | float64 | Alanine transaminase (ALT) level                                                                           | アラニンアミノトランスフェラーゼ（ALT）の値                  |
| delta_alp                      | float64 | Time offset (in minutes) in the measurement of hhange in alkaline phosphatase (ALP) level                  | アルカリホスファターゼ（ALP）の変化測定の時間オフセット（分）         |
| alp                            | float64 | Alkaline phosphatase (ALP) level                                                                           | アルカリホスファターゼ（ALP）の値                       |
| delta_ast                      | float64 | Time offset (in minutes) in the measurement of aspartate transaminase (AST) level                          | アスパラギン酸アミノトランスフェラーゼ（AST）測定の時間オフセット（分）    |
| ast                            | float64 | Aspartate transaminase (AST) level                                                                         | アスパラギン酸アミノトランスフェラーゼ（AST）の値               |
| delta_bilirubin_total          | float64 | Time offset (in minutes) in the measurement of total bilirubin level                                       | 総ビリルビン値測定の時間オフセット（分）                     |
| bilirubin_total                | float64 | Total bilirubin level                                                                                      | 総ビリルビン値                                  |
| delta_bilirubin_direct         | float64 | Time offset (in minutes) in the measurement of direct bilirubin level                                      | 直接ビリルビン値測定の時間オフセット（分）                    |
| bilirubin_direct               | float64 | Direct bilirubin level                                                                                     | 直接ビリルビン値                                 |
| delta_bilirubin_indirect       | float64 | Time offset (in minutes) in the measurement of indirect bilirubin level                                    | 間接ビリルビン値の測定における時間オフセット（分）                |
| bilirubin_indirect             | float64 | Indirect bilirubin level                                                                                   | 間接ビリルビン値                                 |
| delta_ck_cpk                   | float64 | Time offset (in minutes) in the measurement of creatine kinase (CPK) level                                 | クレアチンキナーゼ（CPK）値の測定における時間オフセット（分）         |
| ck_cpk                         | float64 | Creatine kinase (CPK) level                                                                                | クレアチンキナーゼ（CPK）値                          |
| delta_ck_mb                    | float64 | Time offset (in minutes) in the measurement of creatine kinase MB (CK-MB) level                            | クレアチンキナーゼMB（CK-MB）値の測定における時間オフセット（分）     |
| ck_mb                          | float64 | Creatine kinase MB (CK-MB) level                                                                           | クレアチンキナーゼMB（CK-MB）値                      |
| delta_ggt                      | float64 | Time offset (in minutes) in the measurement of gamma-glutamyl transferase (GGT) level                      | γ-グルタミルトランスペプチダーゼ（GGT）値の測定における時間オフセット（分） |
| ggt                            | float64 | Gamma-glutamyl transferase (GGT) level                                                                     | γ-グルタミルトランスペプチダーゼ（GGT）値                  |
| delta_ld_ldh                   | float64 | Time offset (in minutes) in the measurement of lactate dehydrogenase (LDH) level                           | 乳酸デヒドロゲナーゼ（LDH）値の測定における時間オフセット（分）        |
| ld_ldh                         | float64 | Lactate dehydrogenase (LDH) level                                                                          | 乳酸デヒドロゲナーゼ（LDH）値                         |
| delta_albumin                  | float64 | Time offset (in minutes) in the measurement of albumin level                                               | アルブミン値の測定における時間オフセット（分）                  |
| albumin                        | float64 | Albumin level                                                                                              | アルブミン値                                   |
| delta_aniongap                 | float64 | Time offset (in minutes) in the measurement of anion gap                                                   | アニオンギャップの測定における時間オフセット（分）                |
| aniongap                       | float64 | Anion gap                                                                                                  | アニオンギャップ                                 |
| delta_bicarbonate              | float64 | Time offset (in minutes) in the measurement of bicarbonate level                                           | 重炭酸塩値の測定における時間オフセット（分）                   |
| bicarbonate                    | float64 | Bicarbonate level                                                                                          | 重炭酸塩値                                    |
| delta_bun                      | float64 | Time offset (in minutes) in the measurement of blood urea nitrogen (BUN) level                             | 血液尿素窒素（BUN）値の測定における時間オフセット（分）            |
| bun                            | float64 | Blood urea nitrogen (BUN) level                                                                            | 血液尿素窒素（BUN）値                             |
| delta_calcium                  | float64 | Time offset (in minutes) in the measurement of calcium level                                               | カルシウム値の測定における時間オフセット（分）                  |
| calcium                        | float64 | Calcium level                                                                                              | カルシウム値                                   |
| delta_chloride                 | float64 | Time offset (in minutes) in the measurement of chloride level                                              | クロール（Cl）値の測定における時間オフセット（分）               |
| chloride                       | float64 | Chloride level                                                                                             | クロール（Cl）値                                |
| delta_creatinine               | float64 | Time offset (in minutes) in the measurement of creatinine level                                            | クレアチニン値の測定における時間オフセット（分）                 |
| creatinine                     | float64 | Creatinine level                                                                                           | クレアチニン値                                  |
| delta_glucose_lab              | float64 | Time offset (in minutes) in the measurement of glucose level from laboratory                               | 検査室で測定した血糖値における時間オフセット（分）                |
| glucose_lab                    | float64 | Glucose level from laboratory measurement                                                                  | 検査室で測定した血糖値                              |
| delta_sodium                   | float64 | Time offset (in minutes) in the measurement of sodium level                                                | ナトリウム値の測定における時間オフセット（分）                  |
| sodium                         | float64 | Sodium level                                                                                               | ナトリウム値                                   |
| delta_potassium                | float64 | Time offset (in minutes) in the measurement of potassium level                                             | カリウム値の測定における時間オフセット（分）                   |
| potassium                      | float64 | Potassium level                                                                                            | カリウム値                                    |
| delta_ph                       | float64 | Time offset (in minutes) in the measurement of pH level                                                    | pHの測定における時間オフセット（分）                      |
| ph                             | float64 | pH level                                                                                                   | pH                                       |
| delta_lactate                  | float64 | Time offset (in minutes) in the measurement of lactate level                                               | 乳酸値の測定における時間オフセット（分）                     |
| lactate                        | float64 | Lactate level                                                                                              | 乳酸値                                      |
| delta_heart_rate               | int64   | Time offset (in minutes) in the measurement of heart rate                                                  | 心拍数の測定における時間オフセット（分）                     |
| heart_rate                     | float64 | Heart rate                                                                                                 | 心拍数                                      |
| delta_mbp                      | int64   | Time offset (in minutes) in the measurement of mean blood pressure (MBP)                                   | 平均血圧（MBP）の測定における時間オフセット（分）               |
| mbp                            | float64 | Mean blood pressure (MBP)                                                                                  | 平均血圧（MBP）                                |
| delta_resp_rate                | float64 | Time offset (in minutes) in the measurement of respiratory rate                                            | 呼吸数の測定における時間オフセット（分）                     |
| resp_rate                      | float64 | Respiratory rate                                                                                           | 呼吸数                                      |
| delta_temperature              | float64 | Time offset (in minutes) in the measurement of body temperature                                            | 体温の測定における時間オフセット（分）                      |
| temperature                    | float64 | Body temperature                                                                                           | 体温                                       |
| delta_glucose                  | float64 | Time offset (in minutes) in the measurement of glucose level                                               | 血糖値の測定における時間オフセット（分）                     |
| glucose                        | float64 | Glucose level                                                                                              | 血糖値                                      |
| delta_heart_rhythm             | float64 | Time offset (in minutes) in the measurement of heart rhythm                                                | 心拍リズムの測定における時間オフセット（分）                   |
| heart_rhythm                   | object  | Heart rhythm                                                                                               | 心拍リズム                                    |