# nefusi
 Source code from the NEFUSI project
 
 Please note that this is an intermediate version to work with sentences
 
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
 
 What means that the neurofuzzy model completed the training phase with 86.11% accuracy, a cosine similarity (between ground truth and generated solution) with 91.1% accuracy and the test phase with 78.05% accuracy.
 Please note that this accuracy is closed to state-of-the-art.
 
 (Please be aware that the running the software under current configuration takes more than 5 minutes (11th Gen Intel(R) Core(TM) i7-1185G7 @ 3.00GHz   1.80 GHz))
 
  ## Related papers
 - Jorge Martinez-Gil: A Novel Neurofuzzy Model for the Comparison of Legal Texts. Preprint (2022)
 [LINK](http://eprints.rclis.org/43487/1/legal_neurofuzzy.pdf)

 
  ## Funding
  The development of NEFUSI is funded in the project NGI Zero Discovery by the NLnet Foundation and the European Commission. Project number: 2021-04-069
 
  ## License
  MIT
