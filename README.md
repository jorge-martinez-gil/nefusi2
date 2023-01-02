# nefusi
 Source code from the NEFUSI project
 
 Please note that this is an intermediate version to work with <b>sentences</b>.
 
 It is recommended to import the project with an IDE such as Eclipse. When this is not possible, you can proceed manually as follows:
 
 ## Compilation
 ``` ...\nefusi-sentences\src>javac -cp combined-sentences.jar nefusi/*.java```
 
 ## Execution
 ``` ...\nefusi-sentences\src>java -cp .;combined-sentences.jar nefusi.nefusi_Sentences```
 
 Then, you will see something like this:
 ```
 Execution time in milliseconds : 377719
 Training    Cosine   	Test
 0.8611 	 0.911      0.7805
 ```
 
 What means that the neurofuzzy model completed the training phase with 86.11% accuracy, a cosine similarity (between ground truth and generated solution) with 91.1% accuracy and the test phase with 78.05% accuracy. By default, We use the lawSentence200 dataset that compares 200 sentences in the legal field. The inputs of the neural part have been generated with BERT. Please note that this accuracy is closed to state-of-the-art for the dataset lawSentence200. For more information, please refer to the publication mentioned below.
 
 (Please be aware that the running the software under current configuration takes more than 5 minutes (11th Gen Intel(R) Core(TM) i7-1185G7 @ 3.00GHz   1.80 GHz))
 
  ## Citation
```
 @inproceedings{martinez2021,
  author    = {Jorge Martinez-Gil and
               Riad Mokadem and
               Josef K{\"{u}}ng and
               Abdelkader Hameurlain},
  editor    = {Matteo Golfarelli and
               Robert Wrembel and
               Gabriele Kotsis and
               A Min Tjoa and
               Ismail Khalil},
  title     = {A Novel Neurofuzzy Approach for Semantic Similarity Measurement},
  booktitle = {Big Data Analytics and Knowledge Discovery - 23rd International Conference,
               DaWaK 2021, Virtual Event, September 27-30, 2021, Proceedings},
  series    = {Lecture Notes in Computer Science},
  volume    = {12925},
  pages     = {192--203},
  publisher = {Springer},
  year      = {2021},
  url       = {https://doi.org/10.1007/978-3-030-86534-4\_18},
  doi       = {10.1007/978-3-030-86534-4\_18},
  timestamp = {Thu, 14 Oct 2021 10:06:19 +0200},
  biburl    = {https://dblp.org/rec/conf/dawak/GilMKH21.bib},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```

 
  ## Funding
  The development of NEFUSI is funded in the project NGI Zero Discovery by the NLnet Foundation and the European Commission. Project number: 2021-04-069
 
  ## License
  MIT