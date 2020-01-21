# -Language-Generator-for-Turkish
We require a system to generate words and sentences in Turkish based on certain calculations and rules. Assume that ascending order Turkish alphabet is assigned numerical values starting from 1. (e.g. letter_values = {'a':1, 'b':2, 'c':3, 'ç':4, 'd':5, 'e':6, ...} ).

# Prerequisites

pip install import_ipynb
pip install Jpype1
pip install pandas 
pip install re
download Zemberek.jar file and reference it's path into modules

# Module 1: 
Generates given number of words whose sum of letter values equal to a given number.
(e.g. sum of letter values for "yabancılar" or "şirket" is 100)

# Module 2: 
Generate a sentence whose sum of letter values equal to a given number.
This sentence obey the grammatical rules of Turkish language. From this step on you can work with a corpus of Turkish documents. You can parse sentences and words, assign Part of Speech (POS) tags to words, create dictionaries of for different POS labels and choose appropriate words from these dictionaries to form a sentence (e.g. "Ali" from Subject dictionary, "topu" from Object dictionary, and "tut" from verb dictionary --> "Ali topu tut". )
For this module, you can not see meaningful sentences but the sentences are syntactically correct in the basic level (on the most basic level obey the subject object verb order)

# Module 3: 
Generate a sentence whose sum of letter values equal to a given number. This sentence are both syntactically and semantically correct (as much as possible!).
There are an algorithm to combine words + suffixes in a meaningful order. You may extend this to not just neighboring words but the words co-occur in the sentences or in the documents.

# Input Files:

closeMeaningVerbs keep synonyms verbs together.
synonyms.txt keep synonyms nouns and sentences.txt keep sentences that are parsed from corpus(1150haber.rar).
