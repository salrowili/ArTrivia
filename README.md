# ArTrivia
ArTrivia: Harvesting ArabicWikipedia to Build A New Arabic Question Answering Dataset.
# Dataset
The directory Data has the following files (to see a sample of the dataset, use Firefox since its json friendly browser):
* ArTrivia-Dev.json --> Raw ArTrivia development dataset
* ArTrivia-Dev-pre.json --> Pre-processed ArTrivia development dataset
* ArTrivia-Train.json --> Raw ArTrivia training dataset
* ArTrivia-Train-pre.json --> Pre-processed ArTrivia training dataset

  

The pro-processing of the dataset is done following the same steps that AraELECTRA adapted and can be followed through this notebook : 
https://colab.research.google.com/drive/1hik0L_Dxg6WwJFcDPP1v74motSkst4gE?usp=sharing 

The notebook to pre-process the dataset is from AraBERT Github Page: https://github.com/aub-mind/arabert/tree/master/examples
# Things to do in the Future on this repo page :
* Update ArTrivia to Huggginface Hub
* Create and share notebooks to evaluate ArTrivia and TyDi using both ELECTRA and T5 models.
* Share the ArTrivia pipeline after organizing the code.
* Share API codes to retrieve structured datasets from Wikipedia (e.g., Wikipedia Entity Description, WikiData).
* ChatGPT API anntoation code.
* Evaluate ArTrivia in the Open-Domain setting (no passage given) and compare to LLMs.


# Acknowledgment
We would like to acknowledge the support from the TPU Research Cloud (TRC) team for granting us access to TPUv3 units.

# Citation
```bibtex
@inproceedings{alrowili-vijay-shanker-2023-artrivia,
    title = "{A}r{T}rivia: Harvesting {A}rabic {W}ikipedia to Build A New {A}rabic Question Answering Dataset",
    author = "Alrowili, Sultan  and
      Vijay-Shanker, K",
    editor = "Sawaf, Hassan  and
      El-Beltagy, Samhaa  and
      Zaghouani, Wajdi  and
      Magdy, Walid  and
      Abdelali, Ahmed  and
      Tomeh, Nadi  and
      Abu Farha, Ibrahim  and
      Habash, Nizar  and
      Khalifa, Salam  and
      Keleg, Amr  and
      Haddad, Hatem  and
      Zitouni, Imed  and
      Mrini, Khalil  and
      Almatham, Rawan",
    booktitle = "Proceedings of ArabicNLP 2023",
    month = dec,
    year = "2023",
    address = "Singapore (Hybrid)",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.arabicnlp-1.17",
    pages = "191--207",
    abstract = "We present ArTrivia, a new Arabic question-answering dataset consisting of more than 10,000 question-answer pairs along with relevant passages, covering a wide range of 18 diverse topics in Arabic. We created our dataset using a newly proposed pipeline that leverages diverse structured data sources from Arabic Wikipedia. Moreover, we conducted a comprehensive statistical analysis of ArTrivia and assessed the performance of each component in our pipeline. Additionally, we compared the performance of ArTrivia against the existing TyDi QA dataset using various experimental setups. Our analysis highlights the significance of often overlooked aspects in dataset creation, such as answer normalization, in enhancing the quality of QA datasets. Our evaluation also shows that ArTrivia presents more challenging and out-of-distribution questions to TyDi, raising questions about the feasibility of using ArTrivia as a complementary dataset to TyDi.",
}
```
