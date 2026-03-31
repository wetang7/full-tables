<details>
<summary>Results on more ECG foundation models. </summary>

Table 1: Performance comparison of different fine-tuning methods on VTaC dataset for ECG_JEPA model. Results show AUC (%) across five different signal length.

| ECG_JEPA | VTaC-10s | VTaC-30s | VTaC-60s | VTaC-120s | VTaC-180s | 
| --- | ---: | ---: | ---: | ---: | ---: |
| Logit Pooling | 80.30 | 79.14 | 77.95 | 76.90	| 76.23	| 	
| Token Pooling | 80.79	| 79.18	| 78.48	| 77.50 | 76.76 |
| Full Fine-tuning | 76.07 | 79.78 | 82.10 | 88.54 | 88.32 |
| Linear Probing | 78.59 | 80.58 | 80.4	| 78.23 |	77.21	|
| Partial Tuning | 76.29 | 82.23 | 85.37 | 88.80 | 88.89 |
| Bias Tuning | 74.85	| 81.62	| 87.53	| 87.58	| 86.83	|
| Adapter | 65.37	| 66.01	| 67.19	| 70.40 | 70.57 |
| VPT | 70.66	| 78.44	| 84.53	| 88.73	| 89.87	| 
| LSTM Tuning | 79.67 | 80.26	| 82.82	| 85.41	| 85.17	|			
| Ours | 78.86 | 82.93 | 86.09 | 89.36 | 91.02 |

Table 2: Performance comparison of different fine-tuning methods on MCMED dataset (ED discharge) for ECG_JEPA model. Results show AUC (%) across five different signal length.

| ECG_JEPA | MC-MED-10s | MC-MED-30s | MC-MED-60s | MC-MED-120s | MC-MED-180s |
| --- | ---: | ---: | ---: | ---: | ---: |
| Logit Pooling | 63.52	| 67.33 |	68.95 |	69.32	| 69.23	| 	
| Token Pooling | 63.04 | 66.42	| 68.33 | 69.31	| 69.75	|
| Full Fine-tuning | 61.97 | 64.93 | 65.54 | 66.81 | 67.96 |	
| Linear Probing | 62.14 | 65.58 | 66.30 | 68.10 | 70.32 |
| Partial Tuning | 63.18 | 67.00 | 68.29 | 70.29 | 70.19 | 
| Bias Tuning | 65.00	| 69.18 | 70.06	| 71.26 | 72.14	|
| Adapter | 57.27 | 59.44 | 61.35 | 62.28 |	63.06	|		
| VPT | 57.46	| 65.34	| 70.37	| 70.80	| 72.48	|		
| LSTM Tuning | 63.01	| 68.27	| 69.69	| 70.27	| 70.72	|
| Ours | 66.32 | 67.96 | 72.77 | 73.96 | 72.48 |

Table 3: Performance comparison of different fine-tuning methods on CPSC2021 dataset for ECG_JEPA model. Results show AUC (%) across five different signal length.

| ECG_JEPA | CPSC2021-10s | CPSC2021-30s | CPSC2021-60s | CPSC2021-120s | CPSC2021-180s |
| --- | ---: | ---: | ---: | ---: | ---: |
| Logit Pooling | 90.00	| 90.51	| 91.44	| 90.27	| 90.14	|			
| Token Pooling | 90.16	| 90.44	| 91.58	| 90.45	| 90.75	|		
| Full Fine-tuning | 89.04 | 90.40 | 90.53 | 89.32 | 88.67 | 
| Linear Probing | 89.49 | 89.55 | 89.14 | 89.66 | 88.83 |	
| Partial Tuning | 88.81 | 89.90 | 89.83 | 88.40 | 88.33 |			
| Bias Tuning | 81.01	| 85.84	| 86.56	| 85.50	| 85.41 |					
| Adapter | 66.18	| 73.36	| 74.06	| 76.35	| 75.88	|				
| VPT | 70.32	| 78.37	| 89.16	| 92.77	| 93.65	|			
| LSTM Tuning | 90.14	| 90.79	| 90.91	| 91.49	| 91.26	|			
| Ours | 84.08 | 87.00 | 92.97 | 94.25 | 94.65 |

Table 4: Performance comparison of different fine-tuning methods on VTaC dataset for CSFM-Base model. Results show AUC (%) across five different signal length.

| CSFM-Base | VTaC-10s | VTaC-30s | VTaC-60s | VTaC-120s | VTaC-180s |
| --- | ---: | ---: | ---: | ---: | ---: |
| Logit Pooling | 82.75 | 79.95 | 79.64 | 78.01| 77.83 |
| Token Pooling | 83.19 | 80.23 | 79.56 | 78.26 | 77.94 |
| Full Fine-tuning | 62.81 | 64.03 | 70.89 | 80.33	| 84.23 |
| Linear Probing | 79.61 | 80.68 | 78.00 | 74.87 | 74.35	|
| Partial Tuning | 69.39 | 73.38 | 80.83 | 86.05 | 88.81 |			
| Bias Tuning | 65.83	| 72.93	| 83.89	| 89.93	| 90.55	| 			
| Adapter | 69.84	| 72.79	| 78.27	| 85.42 | 88.43 | 		
| VPT | 70.60	| 75.02	| 82.11	| 85.65	| 90.24	|		
| LSTM Tuning | 83.67 | 84.16 | 85.33 | 86.01 | 86.93 |
| Ours | 87.38 | 89.15 | 89.50 | 90.85 | 91.23 |

</details>


<details>
<summary>Results on the comparison of different FM guidance to MERL</summary>

Table 5: Effect of different guidance source for MERL on the VTaC dataset.

| Guidance | VTaC-10s | VTaC-30s | VTaC-60s | VTaC-120s | VTaC-180s |
| --- | ---: | ---: | ---: | ---: | ---: |
| MERL Self-guided | 61.23 | 76.03 | 80.27 | 83.68 | 82.60 |
| CSFM-Tiny guided | 62.67 | 79.64 | 83.46 | 84.64 | 85.19 |
| CSFM-Base guided | 63.16 | 81.33 | 84.51 | 84.99 | 86.07 |


</details>

<details>
<summary>Results on the predictive performance against different background ratios of "foreground" and "background"</summary>

Table 6: Performance evaluation of various foreground (fg) and background (bg) sampling strategies across the VTaC, MCMED, and CPSC datasets with varying foreground ratios. All experiments were conducted using 3-minute ECG sequences for both training and testing. Features derived from the bg-only, fg-only, and fg+bg strategies were averaged to train a linear classification head.

| VTaC | 10% as fg | 25% as fg | 50% as fg | 75% as fg |
|------------------------| ---: | ---: | ---: | ---: |
| bg-only                | 67.93 | 67.25 | 66.58 | 63.37 |
| fg-only                | 71.98 | 71.73 | 72.03 | 72.49 |
| fg+bg                  | 74.05	| 74.05	| 74.05	| 74.05	|

| MCMED | 10% as fg | 25% as fg | 50% as fg | 75% as fg |
| --- | ---: | ---: | ---: | ---: |
| bg-only | 69.06 | 68.93 | 68.99 | 67.28 |
| fg-only | 68.44 | 69.39 | 69.85 | 70.02 |
|  fg+bg | 70.80 | 70.80 | 70.80 | 70.80 |

| CPSC | 10% as fg | 25% as fg | 50% as fg | 75% as fg |
| --- | ---: | ---: | ---: | ---: |
| bg-only | 96.38 | 94.53 | 90.15 | 87.06 |
| fg-only | 96.58 | 96.25 | 96.66 | 96.53 |
|  fg+bg  | 96.81 | 96.81 | 96.81 | 96.81 |

</details>

<details>
<summary>Results of embedding space differences between "background" and "foreground", under different ratios. </summary>

Table 13: Mean L2 distance between foreground and background feature pairs across different datasets and foreground ratios. For each record, we compute the L2 distance between the averaged foreground (fg) features and averaged background (bg) features, then report the mean across all records.

| VTaC | 10% as fg | 25% as fg | 50% as fg | 75% as fg |
|------| ---: | ---: | ---: | ---: |
|      | 0.4506 | 0.2585 | 0.1607 | 0.1408 |

| MC-MED | 10% as fg | 25% as fg | 50% as fg | 75% as fg |
|--------| ---: | ---: | ---: | ---: |
|        | 0.3797 | 0.2038 | 0.1372 | 0.1236 |

| CPSC | 10% as fg | 25% as fg | 50% as fg | 75% as fg |
|------| ---: | ---: | ---: | ---: |
|      | 0.3568 | 0.1970 | 0.1383 | 0.1267 |

</details>

<details>
<summary>Results of extended model performance with different ratios, on VTaC, based on CSFM-Tiny</summary>

Table 7: Performance of fine-tuning CSFM_Tiny model under different foreground ratio. Results show AUC (%) across five different signal length.

| **CSFM-Tiny** | **VTaC-10s** | **VTaC-30s** | **VTaC-60s** | **VTaC-120s** | **VTaC-180s** |
| --- | ---: | ---: | ---: | ---: | ---: |
| 5%  | 81.15 | 86.39 | 88.98 | 88.26 | 88.18 |
| 25% | 84.10 | 88.29 |	89.01 |	89.76 |	89.50 |
| 50% | 83.48 | 86.89 |	87.47 |	87.73 |	86.79 |
| 75% | 82.09 | 85.50 |	86.60 |	87.16 |	86.02 |

</details>

<details>
<summary>Results of different locality-aware contrastive strategies on MC-MED (ED discharge)</summary>

Table 8: Comparison of different contrastive learning strategies for CSFM-Tiny model in MCMED dataset. We evaluate three contrastive approaches: Batch Contrast (standard batch-level contrastive learning), Intra-subject Contrast (contrasting samples within the same subject), and Inter-subject Contrast (contrasting samples across different subjects).

| **CSFM-Tiny** | **10s** | **30s** | **60s** | **120s** | **180s** |
| --- | ---: | ---: | ---: | ---: | ---: |
| Batch Contrast         | 64.38 | 69.55 | 71.12 | 71.88 | 72.02 |
| Intra-subject Contrast | 58.96 | 67.88 | 69.46 | 71.12 | 71.93 |
| Inter-subject Contrast | 59.93 | 66.48 | 70.49 | 71.57 | 72.04 |

</details>


<details>
<summary>Comparison of computational cost between full-finetuning and ours, across different backbone foundation models</summary>

Table 9: Comparison of the number of trainable parameters between full fine-tuning and the proposed method across different model architectures.

| Training Parameters | Full Fine-tuning | Ours |
| --- | ---: | ---: |
| CSFM-Tiny | 91,270,969 | 3,891,201 |
| MERL | 5,473,152 | 3,891,201 |
| CSFM-Base | 157,389,625 | 4,352,001 |
| ECG-JEPA | 85,374,720 | 3,891,201 |

</details>


<details>
<summary>Results of additional tasks on MC-MED (5 class Triage_Acuity, based on CSFM-Tiny)</summary>

Table 10: Performance comparison of different fine-tuning methods on MC-MED dataset (ED triage) for CSFM-Tiny model. Results show AUC (%) across five different signal length.

| CSFM-Tiny | ED triage-10s | ED triage-30s | ED triage-60s | ED triage-120s | ED triage-180s |
| --- | ---: | ---: | ---: | ---: | ---: |
| Logit Pooling | 59.19 | 59.82 | 60.25 | 60.41 | 60.13 |
| Token Pooling | 58.77 | 59.09 | 60.20 | 60.92 | 61.00 |
| Full Fine-tuning | 62.10 | 61.89 | 63.02 | 63.54 | 64.80 |
| Linear Probing | 58.38 | 60.78 | 60.01 | 60.56 | 60.66 |
| Partial Tuning | 61.40 | 62.07 | 63.09 | 65.33 | 63.43 |			
| Bias Tuning | 51.65	| 52.12	| 55.63	| 56.35	| 56.71	| 			
| Adapter | 60.31	| 59.36	| 60.02	| 61.42 | 61.55 |
| VPT | 56.33	| 60.39	| 61.51	| 63.38	| 64.50	|
| LSTM Tuning | 51.08 | 58.29 | 61.66 | 60.98 | 61.97|
| Ours | 60.17 | 62.54 | 64.14 | 64.74 | 65.18 | 
</details>


<details>
<summary>Results of different drop strategies (Affinity drop vs Random drop) </summary>

Table 11: Comparison of drop strategies for the consistency module, evaluated on CSFM-Tiny model.

| **Training Data** | **Drop Method** | **VTaC-10s** | **VTaC-30s** | **VTaC-60s** | **VTaC-120s** | **VTaC-180s** |
| --- | --- | ---: | ---: | ---: | ---: | ---: |
| **50%** | Affinity Drop | 80.39 | 83.79 | 86.02 | 86.10 | 86.25 |
|  | Random Drop | 77.77 | 79.97 | 82.28 | 84.24 | 85.20 |
| **100%** | Affinity Drop | 84.10 | 88.29 | 89.01 | 89.76 | 89.50 |
|  | Random Drop | 84.00 | 87.19 | 88.35 | 90.03 | 89.01 |
</details>

<details>
<summary>Results of additional baseline comparisons on VTaC based on CSFM-Tiny</summary>

Table 12: Comparison of temporal modeling approaches on VTaC dataset with varying sequence lengths. We compare ResNet1D, 3-layer LSTM models, and MIL methods.

| **CSFM-Tiny**                                             | **VTaC-10s** | **VTaC-30s** | **VTaC-60s** | **VTaC-120s** | **VTaC-180s** |
|-----------------------------------------------------------| ---: | ---: | ---: | ---: | ---: |
| ResNet1d-50 (train using 10s CSFM-Tiny feature sequence)  | 54.01 | 68.20 | 64.16 | 60.87 | 73.67 |
| 3-layer LSTM (train using 10s CSFM-Tiny feature sequence) | 67.97 | 72.42 | 74.30 | 73.54 | 72.73 |
| Multi-instance Learning                                   | 80.01 | 80.31 | 79.56 | 77.37 | 77.40 |
| Ours                                                      | 84.10 | 88.29 | 89.01 | 89.76 | 89.50 |

</details>

<details>
<summary>Results of setting upper bound as 5 minutes, on VTaC (note: decreased batch size)</summary>

Table 13: Performance of fine-tuning CSFM_Tiny model under different foreground ratio. Results show AUC (%) across five different signal length.

| **CSFM-Tiny** | **VTaC-1 mins** | **VTaC-2 mins** | **VTaC-3 mins** | **VTaC-4 mins** | **VTaC-5 mins** |
| --- | ---: | ---: | ---: | ---: | ---: |
| Full Fine-tuning  | 66.71 | 66.86 | 73.00 | 75.78 | 78.07 |
|       Ours      | 85.55 | 86.24 | 85.97 | 86.09 | 85.45 | 
</details>