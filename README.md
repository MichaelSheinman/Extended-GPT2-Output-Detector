# Extended GPT2 Output Detector

The project is currently running at: https://michaelgithubhype.github.io/Extended-GPT2-Output-Detector/
Related blog: TODO 


This project extends the [GPT-2 Output Detector](https://github.com/openai/gpt-2-output-dataset/tree/master/detector) made by OpenAI. I added two features on top of the original detector:

* No token limit. This version splits tokens into batches and then computes the average accuracy across the batches. 
* Zip file support. The app can run through multiple submissions and compute a real probability for each one. 





