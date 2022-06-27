# NLP - BILSTM-CRF Named-Entity_Recognition

<center><img src="model_bilstm_crf.png" width=400 ></center>

| Averages | Entities | Precision    | Recall       | F-1 Scores   |
| -------- | -------- | ------------ | ------------ | ------------ |
| Micro    | PAD      | 1            | 1            | 1            |
| Micro    | O        | 0,9700065203 | 0,956698821  | 0,9633067127 |
| Micro    | plant    | 0,9884940778 | 0,9884940778 | 0,9884940778 |
| Micro    | disease  | 0,9884940778 | 0,9884940778 | 0,9884940778 |
|          |          |              |              |              |
| Macro    | PAD      | 1            | 1            | 1            |
| Macro    | O        | 0,9700065203 | 0,956698821  | 0,9633067127 |
| Macro    | plant    | 0,9001643335 | 0,9170404243 | 0,9074482884 |
| Macro    | disease  | 0,9001643335 | 0,9170404243 | 0,9074482884 |
|          |          |              |              |              |
| Weighted | PAD      | 1            | 1            | 1            |
| Weighted | O        | 0,9700065203 | 0,956698821  | 0,9633067127 |
| Weighted | plant    | 0,9892060224 | 0,9884940778 | 0,988767089  |
| Weighted | disease  | 0,9892060224 | 0,9884940778 | 0,988767089  |
