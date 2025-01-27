# Phrase Sense Disambiguation for NLP using PhraseBase
A Hadoop MapReduce java implementation for disambiguating entities from simple English sentences using a phrasal knowledge base.


# Requirements
- Download datasets from https://www.kaggle.com/rushabhmishra/phrasebase
- Stanford CoreNLP 2018-2-27
- Hadoop 3.0

# Steps
- Clone the repository
- Run in terminal
  ``` hadoop com.sun.tools.javac.Main PhraseBase.java ```
- Run
  ``` jar cf PhraseBase.jar PhraseBase*.class ```
- Create input.txt and write any simple sentence that has
  - subject
  - verb phrase 
  - object
 
   eg. Sachin Tendulkar was born in Mumbai.

   You can provide multiple sentences in the input file but be sure to write each sentence on a different line 
   and end them with a period (.)
- Run
  ``` hadoop jar PhraseBase.jar PhraseBase input.txt ```  
For more detailed theory and documentation about the project read the attached PDF
