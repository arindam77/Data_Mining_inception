# Document_classifier


Flask-api-Classification-and-NER
Proof of concept:

Description: Before a drug is released Pharmaceutical companies have to go through a process of submitting various regulatory documents in order to release the drug. In the process of doing the same our company already has a product where in a user has to do the following things:-

Upload the document in a specific category(depending on the document by opening each and every file and checking the category it belongs to

Open each and every document and check the drug substance it is talking about and upload the drug subtsnce name and the same process is to be followed for mentioning the Companies manufacturing the drug

If a document gets uploaded in a wrong category the consequences lead to no submission of document and wastage of time

Doing this for 100000 documents a day leads to manual efforts and the rate of error is very high. Even if one document gets submitted in the wrong category or name of substance/substance manufacturer is wrong

Solution:-

The document can be scanned or a normal pdf(please check repository pdf to text)
number of document types are 53(that is a huge number)
Upon exploring the data it was observed that a lot of documents had a consistent format as they were supposed to be submitted in a specific format for which regular expression was used to capture the data (Machine Learning was not required in this step).
Rest of the documents were not standard across the industry so had to use a ML based approach.
Based upon the category predicted extract substance name , Manufacturer etc.
Built Custom trained NER models to extract entities like Substance Name, Address etc from documents.
Built a flask api to perform above mentioned things.
