# EYT
Algorithm:

1. Input sentence. 
2. Split the sentence into tokens using NLTK's word_tokenize(). 
3. Tag those tokens into their corresponding PART-OF-SPEECH tags using post_tag(). 
Now here's the critical parts for me: 
4. Since ENGLISH commonly follows the S-V-O agreement,using the tags of each tokens, parse the SUBJECT, VERB, OBJECT of the sentence or the NOUN PHRASE and VERB PHRASE. 
5. Next step is the RULE-BASED REORDERING, From S-V-O, reorder it to V-S-O, the sentence pattern commonly follows of Ibanag sentence structure. 
6. So here's now where the knowledge-based approach comes in, Ibanag speakers or linguist knowledge will formulate a grammar rules on how the input sentence will be translated. For example in OBJECT part of the sentence, if there is ADJECTIVE NOUN sequence, linking word 'tu' will be added to link the ADJECTIVE and NOUN (ADJECTIVE <tu> NOUN). 
7. Then after the reordering, query each tokens their IBANAG value from database and apply the grammar rules. 
8. Display the output. 
