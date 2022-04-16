# Part-of-speech-tagging-NLP-Hackathon

## My approach for 2021 Super AI Engineer Deleveopment program. Week 2 NLP major hackathon divide into 4 task
* word segmentation
* sentence segmentation
* name entity regcognition
* part of speech tagging

This Repo is for part of speech tagging task.
## My approach

Framework use : SimpleTransformer

1. Using WangchanBERTa language model transfer to POS downstream task by training
   using data LST21 (a huge corpus about thai news , wikipedia). This data is not clean  but have a huge word dictionary.
2. Fine tuning by using open source LST20 data (apporve by linguist)
3. convert model to ONNX format
4. Revert enginnering Simpletransformer library to crate full prediction pipeline that work with ONNX format.
5. deploy a model prediction as an API(FastAPI) in ONNX format on NVIDIA Triton inference server
