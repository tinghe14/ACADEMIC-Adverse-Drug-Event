# Using SemRep to Detect Adverse Drug Events in Biomedical Abstracts 
This research was to determine whether automated tools might efficiently support the retrieval of Adverse Drug Event (ADE) information from biomedical abstracts. We used SemRep to process all biomedical abstracts and retrieve full adverse drug event information for aliskiren. Aliskiren was withdrawn from the market due to angioedema. We processed the 1,203 abstracts published for aliskiren in PubMed until the time of this study and were able to detect the safety issue associated with Aliskiren.

There is one file for Python code:semantic_types_and_relationahips.ipynb

The codes process the 1203 XML formated abstracts. We found the IDs for aliskiren, drug, symptom, aliskiren relevant drug, aliskiren unrelevant drug. We plotted the frequenct tables and plots for each types of outcome. After that, we process abstracts to get information anout CUI pairs: aliskiren & symptom and print out the symptom name. We also ran the code for 23 papers using keywords "aliskiren & angioedema" in the pubmed. This aimed to detect the similar patterns in "aliskiren & angioedema" relevant paper. 

# Requirement
1. xml.etree.ElementTree: The ElementTree XML API
2. lxml.etree

# How to execute
Users need to download the abstracts from PubMed. Then ran the texts through SemRep, which also requires to download MetaMap and signed the agreement form for the UMLS agreement. Detialed information can check here: https://semrep.nlm.nih.gov/SemRep.v1.5_Installation.html. After that you can get the XML formated result and run the "semantic_types_and_relationahips.ipynb"
