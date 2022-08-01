# NLP
# Named Entity Recognition (NER) - BILSTM - CRF


## <img src="https://img.icons8.com/external-smashingstocks-flat-smashing-stocks/64/000000/external-manager-hotel-smashingstocks-flat-smashing-stocks-2.png"/> **`Slamet Riyanto S.Kom., M.M.S.I.`**

## <img src="https://img.icons8.com/external-fauzidea-flat-fauzidea/64/undefined/external-man-avatar-avatar-fauzidea-flat-fauzidea.png"/> **`Dimas Dwi Putra`**

## Architecture
<p align="center"><img src="NER-BILSTM-CRF%20Architecture.png" width="3900"></p>

## Dataset<br>[View Dataset .csv](input/)
| Sentence #  | Word        | POS | Tag       |
| ----------- | ----------- | --- | --------- |
| Sentence: 0 | studies     | NNS | O         |
| Sentence: 0 | on          | IN  | O         |
| Sentence: 0 | magnesium   | NN  | O         |
| Sentence: 0 | s           | NN  | O         |
| Sentence: 0 | mechanism   | NN  | O         |
| Sentence: 0 | of          | IN  | O         |
| Sentence: 0 | action      | NN  | O         |
| Sentence: 0 | in          | IN  | O         |
| Sentence: 0 | digitalis   | NN  | B-plant   |
| Sentence: 0 | induced     | VBD | O         |
| Sentence: 0 | arrhythmias | NNS | B-disease |
...

## Eval<br>[View Eval Report .xlsx](Model%20Report.xlsx)
| Entities     | precision | recall   | f1-score | support | excecution time | processor | ram  | model | batch size | epochs | embedding | Length | Uji |
| ------------ | --------- | -------- | -------- | ------- | --------------- | --------- | ---- | ----- | ---------- | ------ | --------- | ------ | --- |
| PAD          | 1,000000  | 1,000000 | 1,000000 | 131     | 4.49.57         | cpu       | high | 2     | 16         | 40     | 128       | 3000   | 7   |
| Disease      | 0,774775  | 0,623188 | 0,690763 | 140     |                 |           |      |       |            |        |           |        |     |
| Plant        | 0,892857  | 0,892857 | 0,892857 | 135     |                 |           |      |       |            |        |           |        |     |
| micro avg    | 0,895288  | 0,836186 | 0,864728 | 406     |                 |           |      |       |            |        |           |        |     |
| macro avg    | 0,889211  | 0,838682 | 0,861207 | 406     |                 |           |      |       |            |        |           |        |     |
| weighted avg | 0,887332  | 0,836186 | 0,858986 | 406     |                 |           |      |       |            |        |           |        |     |
| F-1 Scores   |           |          | 86,5%    |         |                 |           |      |       |            |        |           |        |     |

## Predict
```yaml
Word           ||True ||Pred
==============================
the            : O     O
mutagen        : O     O
sensitivity    : O     O
assay          : O     O
msa            : O     O
a              : O     O
phenotypic     : O     O
marker         : O     O
of             : O     O
dna            : O     O
damage         : O     O
response       : O     O
and            : O     O
repair         : O     O
capacity       : O     O
has            : O     O
been           : O     O
consistently   : O     O
shown          : O     O
to             : O     O
associate      : O     O
with           : O     O
risk           : O     O
tobacco        : plant plant
related        : O     O
cancers        : disease disease
```

## Output<br>[View Model Directory](output/)
### Save model output as [.hdf5](output/)

# **Other Content**

### **Websites Prediction**
#### [1. Django Websites Prediction For NER dan RE](https://github.com/Dimas263/Django-Websites_NER_RE)


### **Named Entity Recognition (NER)**
#### [1. NER Dataset Biomedical Plant-Disease Corpus](https://github.com/Dimas263/NLP_NER_Dataset_Biomedical_Plant-Disease_Corpus)
#### [2. NER CRF Named Entity Recognition](https://github.com/Dimas263/NLP_NER_CRF_Named_Entity_Recognition)
#### [3. NER BiLSTM Named Entity Recognition](https://github.com/Dimas263/NLP_NER_BILSTM_Named_Entity_Recognition)
#### [4. NER BERT Named Entity Recognition](https://github.com/Dimas263/NLP_NER_BERT_Named_Entity_Recognition)
#### [5. NER BiLSTM CRF Named Entity Recognition](https://github.com/Dimas263/NLP_NER_BILSTM_CRF_Named_Entity_Recognition)
#### [6. NER BERT BiLSTM CRF Named Entity Recognition](https://github.com/Dimas263/NLP_NER_BERT_BILSTM_CRF_Named_Entity_Recognition)


### **Relation Extraction (RE)**
#### [1. RE Dataset Biomedical Plant-Disease Corpus](https://github.com/Dimas263/NLP_RE_Dataset_Biomedical_Plant-Disease_Corpus)
#### [2. RE BERT Relation Extraction Biomedical](https://github.com/Dimas263/NLP_RE_BERT_Relation_Extraction_Biomedical)
#### [3. RE BiLSTM CRF Relation Extraction Biomedical](https://github.com/Dimas263/NLP_RE_BILSTM_CRF_Relation_Extraction_Biomedical)