# Toxic Comments Detection in Russian

This repository contains the fine-tuned Multilingual Bidirectional Encoder Representations from Transformers (M-BERT) (Devlin et al., 2019), ruBERT (Kuratov et al., 2019), and two versions of Multilingual Universal Sentence Encoder (M-USE) (Yang et al., 2019) for toxic comments detection in Russian. As a source of data, we utilized anonymously published [Kaggle dataset](https://www.kaggle.com/blackmoon/russian-language-toxic-comments) and additionally validated its annotation quality.  

| System  | P | R | F<sub>1</sub> | 
| ------------- | ------------- | ------------- | ------------- | 
| MNB-Toxic | 87.01% | 81.22% | 83.21% |
| M-BERT<sub>Base</sub>-Toxic | 91.19% | 91.10% | 91.15% |
| ruBERT-Toxic | 91.91% | 92.51% | 92.20% |
| M-USE<sub>CNN</sub>-Toxic | 89.69% | 90.14% | 89.91% |
| M-USE<sub>Trans</sub>-Toxic | 90.85% | 91.92% | 91.35% |

## Toxic Comments Dataset

[Kaggle Russian Language Toxic Comments Dataset](https://www.kaggle.com/blackmoon/russian-language-toxic-comments) is the collection of annotated comments from [2ch](https://2ch.hk/) and [Pikabu](https://pikabu.ru/), which was published on Kaggle in 2019. It consists of 14412 comments, where 4826 texts were labeled as toxic, and 9586 were labeled as non-toxic. The average length of comments is ~175 characters; minimum length is 21, and the maximum is 7403. 

## Trained Models
To download fine-tuned models for Russian, please follow the link [https://yadi.sk/d/nmGpvIrzwdDC-Q](https://yadi.sk/d/nmGpvIrzwdDC-Q).
* M-BERT-Base-128-FiT-KRLRCD – Multilingual BERT<sub>Base</sub> fine-tuned on Kaggle Russian Language Toxic Comments Dataset.
* ruBERT-Base-128-FiT-KRLRCD – ruBERT fine-tuned on Kaggle Russian Language Toxic Comments Dataset.
* M-USE-CNN-FiT-KRLRCD – Multilingual USE<sub>CNN</sub> fine-tuned on Kaggle Russian Language Toxic Comments Dataset.
* M-USE-Trans-FiT-KRLRCD – Multilingual USE<sub>Trans</sub> fine-tuned on Kaggle Russian Language Toxic Comments Dataset.

## References
1. Jacob Devlin, Ming-Wei Chang, Kenton Lee, and 950 Kristina Toutanova. 2019. BERT: Pre-training of deep bidirectional transformers for language understanding. In Proceedings of the 2019 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long and Short Papers), pages 4171–4186, Minneapolis, Minnesota. Association for Computational Linguistics.
2. Yuri Kuratov and Mikhail Arkhipov. Adaptation of deep bidirectional multilingual transformers for Russian language. In Computational Linguistics and Intellectual Technologies: Papers from the Annual International Conference “Dialogue”, pages 333–340, Moscow, Russia, 2019. RSUH.
3. Yinfei Yang, Daniel Cer, Amin Ahmad, Mandy Guo, Jax Law, Noah Constant, Gustavo Herna ́ndez A ́brego, SteveYuan, ChrisTar, Yun-HsuanSung, Brian Strope, and Ray Kurzweil. 2019. Multilingual universal sentence encoder for semantic retrieval. CoRR, abs/1907.04307.


## Documentation and How to report bugs
* TensorFlow documentation: [https://www.tensorflow.org/api_docs](https://www.tensorflow.org/api_docs).
* Scikit-learn documentation: [http://scikit-learn.org/stable/documentation.html](http://scikit-learn.org/stable/documentation.html). 
* BERT repository: [https://github.com/google-research/bert](https://github.com/google-research/bert). 
* If you find any issues, please open a bug here on GitHub.

## License
See [LICENSE](LICENSE.txt).