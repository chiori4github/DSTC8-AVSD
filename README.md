# DSTC8-AVSD
DSTC8-AVSD: Sentence generation task for Audio Visual Scene-aware Dialog 

## NEWS

Test sets are now Releasing!!! 

###
1. Please register the challenge from the following link:

   https://docs.google.com/forms/d/e/1FAIpQLScbTSq9P3d_o_2aK2IKvFmrEJ3-xdORspxNyt3NcQ3oiuA8Bw/viewform

2. You can find the test sets from the following link: 

   https://drive.google.com/file/d/1IYAoCuaKDwzRJURArHh9MHU4HPRYdewo/view?usp=sharing

3. Please note that we cannot use the DSTC7 test sets for any purposes for DSTC8.

4. When you will submit the systems, please clarify training with or without the summary and caption.
###

"Any features" extracted from the given videos can be used at DSTC7 and DSTC8.

The multiple references for the DSTC7 AVSD test set in the following file:
https://drive.google.com/file/d/1nz9Pu9YIfuZHzowhASXERajRXqE6DBQx/view?usp=sharing


dstc7avsd_eval.tgz 

## - Track Description
Welcome to the follow-up challenge for Audio Visual Scene-Aware Dialog (AVSD) using Natural Language Generation (NLG) technologies of the successor of DSTC7-AVSD. This challenge is one of the track for the **8th Dialog System Technology Challenges (DSTC8) workshop.**
The task is to build a system that generates responses in a dialog about an input **video**.

### - Tasks

In this challenge, systems are required to generate responses to user input in the context of a given dialog.  
This context consists of a dialog history (previous utterances between both user and system) in addition to video and audio information that comprise the scene. 
The quality of a system response automatically generated will be evaluated using objective measures to see how good the generated responses are in terms of the naturalness and informativeness.

#### 1. Task 1: Video and Text 
    a. Use the video and text training data provided but no external data sources, 
       other than publicly available pre-trained feature extraction models.

       There are two options: with or without using the summary generated by the questioners after holding 10 QAs.

    b. External data may also be used for training.

#### 2. Task 2: Text Only 
    a. Do not use the input videos for training or testing. 
       Use only the text training data (dialogs and video descriptions) provided. 
    b. Any publicly available text data may also be used for training.
    
    
#### Validation data set:

Please train models using the training data set only.
You can tune the parameters using the validation set and confirm the performance of your systems using the DSTC7 test sets.
Notes: The official challenge doesn't allow you to use the DSTC7 test set to tune your models.

|               |    Training    |  Validation   |   DSTC7 Test  |
| ------------- | -------------- | ------------- | ------------- |
| # of Dialogs  |       7,659    |      1,787    |      1,710    |   
| # of Turns    |     153,180    |     35,740    |     13,490    |
| # of Words    |   1,450,754    |    339,006    |    110,252    |

*The number of turns for the test set is smaller than the validation
because they are not always full dialogs.

You can download the full official data set and the references for AVSD@DSTC7 from here:
https://drive.google.com/drive/folders/1SlZTySJAk_2tiMG5F8ivxCfOl_OWwd_Q?usp=sharing

1. **Text files:**
     - train_set4DSTC7-AVSD.json
     - valid_set4DSTC7-AVSD.json
     - test_set4DSTC7-AVSD.json

2. **Audio feature files:**
   - Training and validation data sets
     - vggish.tgz 
   - DSTC7 test set:
     - vggish_testset.tgz: 

3. **Visual feature files:**
   - Training and validation data sets:
     - i3d_flow.tgz 
     - i3d_rgb.tgz
   - DSTC7 test set:
     - i3d_flow_testset.tgz
     - i3d_rgb_testset.tgz

4. **DSTC7 evaluation setup**
   - dstc7avsd_eval.tgz


Although a new baseline system will be released soon, the old one is available from the following link:
https://github.com/dialogtekgeek/AudioVisualSceneAwareDialog

You can find more information in the following DSTC7-AVSD overview paper:
http://workshop.colips.org/dstc7/papers/DSTC7_Task_3_overview_paper.pdf

### - Contact Information
chori@merl.com, cherian@merl.com, tkmarks@merl.com
