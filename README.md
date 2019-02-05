#### Quora Insincere Questions Classification

This is the code I used for [Quora Insincere Questions Classification](https://www.kaggle.com/c/quora-insincere-questions-classification) Natural Language Processing.

#### Ideas that worked:
1. Not removing punctuations Tokenizer(fiters = 'None')
2. Captalize to find more Embeddings, 
3. Mean Embeddings
4. Concat Embeddings
3. Adding more Features
4. Reducing batch size and n_epochs (512,5) to (256,4) helps saving time and improving score.
5. Dynamic meta embeddings(DME)
6. DME + Focal Loss



##### Todo:
- [x] Add more preprocessing [Improve your Score with some Text Preprocessing \| Kaggle](https://www.kaggle.com/theoviel/improve-your-score-with-some-text-preprocessing)
- [x] Merge Concat, no_filter, rev, More Features
- [x] Check Different Embedding Combinations
- [x] Add insincere words  --> No Diff
- [x] Check n_split==1 and ensemble (Reverse + Simple)
- [x]`torch.backends.cudnn.benchmark = True
- [x] Check different loss functions
- [x] Check different architectures
- [x] Check [Fork of Mix of NN models \| Kaggle](https://www.kaggle.com/shujian/fork-of-mix-of-nn-models)
- [x] max_feature=None when Tokenizer;
- [x] Reverse words
- [x] Spacy Tokenizer, Punctuation in tokenisation
- [x] Double the negatives (Does not work)
- [x] 1) concat emb not mean; 
- [x] 2)max_feature=None when Tokenizer;
- [x] 3)Add statistic feature
- [x] 4) CLR
- [x] 5) Capsule



### Notebooks:
1. [Fork from attent](https://www.kaggle.com/harmandeepsingh01/fork-from-bilstm-attention-kfold-0115-81a8d9) 
2. [Check Concat](https://www.kaggle.com/harmandeepsingh01/check-concat)
3. [Check Rev](https://www.kaggle.com/harmandeepsingh01/check-rev)
4. [Check BSZ](https://www.kaggle.com/harmandeepsingh01/check-batchsz)
5. [Check rev 6847 ](https://www.kaggle.com/harmandeepsingh01/check-rev-6847)
6. [Check vocab coverage](https://www.kaggle.com/harmandeepsingh01/check-vocab-coverage)
7. [Merge Attention](https://www.kaggle.com/harmandeepsingh01/merge-attention/) v1--6832  `v2--6843`  `v3--6850` v4--6837 v5--6792 v6--isv2withFL--6834
8. [Merge2 reset](https://www.kaggle.com/harmandeepsingh01/merge2-reset/) `v1--6849`  `v2--6846` v3--6834 v4--6827 v5--6803  v6--6828  v7--isv1 with focal loss--6835 v8--6770  v9--6829
9. [DME1111](https://www.kaggle.com/harmandeepsingh01/dme1111)  `v1-6867` `v6-6869` `v9-6872`  v10--6794  v11--6820  v12-6839
10. [Dme2222](https://www.kaggle.com/harmandeepsingh01/dme2222) v9 of Dme111  v2--6872  v3--6854  v4--6862  `v5--6875` `v6--6877`  `v7--6876`
11. [Dme embedding Combination](https://www.kaggle.com/harmandeepsingh01/dme-embedding-combination) `glove,fast--6872`    g,p-6852    f,p --6866
12. [Rarewords](https://www.kaggle.com/harmandeepsingh01/add-insincere-words-merge2reset) --no--diff
13. [Compress Pred](https://www.kaggle.com/harmandeepsingh01/compress-pred/edit)
14. [1](https://www.kaggle.com/harmandeepsingh01/once-check-1/edit)
15. [2](https://www.kaggle.com/harmandeepsingh01/once-check-2/edit)
15. [3](https://www.kaggle.com/harmandeepsingh01/once-check-3/edit)
16. [4](https://www.kaggle.com/harmandeepsingh01/once-check-4/edit)
17. [5](https://www.kaggle.com/harmandeepsingh01/once-check-5/edit)
18. [6](https://www.kaggle.com/harmandeepsingh01/once-check-6/edit)
------
Subs:
1. [Merge-atten-6843](https://www.kaggle.com/harmandeepsingh01/merge-attention-sub)
2. [Final Sub](https://www.kaggle.com/harmandeepsingh01/once111) `v2--6943`   v3--6929
4. [6](https://www.kaggle.com/harmandeepsingh01/once-check-6/edit) `6843`
5. [Once222](https://www.kaggle.com/harmandeepsingh01/once222)



-------------------
1. `Done`
#1 6774 512 5
#2  6790 4 512
#3  `6799 4 256`
#4  6798 3 256


---------------------
2. `Done` `Final`
#1 6765 5 512 
#2 6807 4 512
#3 6762 3 512
#4 `6828 3 256`


-------------------

3.`Done` 
#1 6747 512 5

#2 6782 512 4

#3 6768 512 3

#4` 6809 256 3`

#5 6800 256 4
 
 
-----------------------



4.
#1 6793 512 5

#2 6766 512 4

#3 6816 512 3

#4 0000 256 3


 
------------


5.`Done` `Final`

#1 6834 512 6

#2 `6859 512 5`  600s/epoch

#3 6825 256 4

#4 6834 256 5


----------

6.   
#1 `6843 512  6`
