# All About Guidelines
 
Since AI chat model seems to have reasonable understanding of medical terminology, we think it can be seriously considered for use in the medical field.
However, there are several problems with using the chat tool in a medical. 
  
 
## Hallucination
The problem of Hallucination is serious.
Hallucination is a problem that chat AI responds plausibly with false information.
For example, ask about the content of Fleischner's guidelines.
We’ve got a very specific and detailed response as shown here. 

![demo](asset/chatgpt_1.png)

However, it was found there were some details thought to be a bit mistake.
For example, the Fleischner’s guidelines clearly state that follow-up CT scan is after 3 months for solid nodules larger than 8 mm, but the response was 3,6,12 months.

 

- pydicom >= 2.1
- numpy >= 1.20 
- scipy >= 1.6 
- scikit-image >= 0.18.1 
- scipy >= 1.6 
- opencv-python >= 4.5 
- simpleitk >= 1.2
- pytorch (cuda enabled)

## Hardware 
NVIDIA GPU (>=12GB) with CUDA toolkit

## Usage

1\. Put synthetic raw DICOM data files into "ios/input" folder (any folder structure is allowed but one series must be in the same folder)

2\. From command line
```cmd
>>>python cmd.py 
``` 
3\. The synthetic MRA output will be in ios/output with the same folder structure.
## Examples 
The test input data (magic_sample) is provided here <a href="https://www.dropbox.com/s/fw2ghn5poriac9l/magic_sample.zip?dl=0" target="_blank">magic_sample</a>.

Download & unzip, and copy in ios/input. Then, 
```cmd
>>>python cmd.py 
``` 
Output sample will be created in ios/output.