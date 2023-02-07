# Extended GPT2 Output Detector

The project is currently running at: https://michaelgithubhype.github.io/Extended-GPT2-Output-Detector/

Related blog: https://michaelsheinman.medium.com/how-i-improved-the-gpt2-output-detector-6e47ba133235

![project example](https://miro.medium.com/max/640/1*oQigM3yqYRowYANCkb1UNA.gif)


## Background 
This project extends the [GPT-2 Output Detector](https://github.com/openai/gpt-2-output-dataset/tree/master/detector) made by OpenAI. I added three features on top of the original detector:

* No token limit. This version splits tokens into batches and then computes the average accuracy across the batches. 
* Custom file upload. Allows the ability to upload files. Currently supports text and pdf files. 
* Zip file support. The app can run through multiple submissions and compute a real probability for each one. 


## Disclaimers 

* This project is simply my changes to the GPT-2 Output Detector. You can find out more about how the original project works in the [GitHub repository](https://github.com/openai/gpt-2-output-dataset/tree/master/detector).
* It's possible that splitting the main text into batches would lower the accuracy of the tool in some cases. While this tool is a convenient way to identify potential AI content, you shouldn't blindly rely on this tool. Especially if the subject is students.
* I did not deploy the backend of the program. I am currently simply sending requests in batches to the [GPT-2 Output Detector](https://openai-openai-detector.hf.space/). If that site goes down, this application would also stop working.
* Like the original program, this model only supports text. Submissions that contain code may fail to complete.

## Exporting Results:

A simple script to get a list of probabilities, run from command line (I'll add a proper import at some point):
```
var filenames = document.getElementsByClassName("file-name")
var real = document.getElementsByClassName("real-probability")

var filesnames = [];
var realProbabilities = [];

for (var i = 0; i < elements.length; i++) {
  innerTexts.push(elements[i].innerText);
  realProbabilities.push(real[i].innerText);
}
```
