# Documentation
## Corpus description
This corpus contains lyrics from seven songs by Arctic Monkeys. One song is selected from each album released between 2006 and 2022. The corpus is designed to explore changes in vocabulary, themes, writing style, and sentiment over time.
## Target audience
This corpus is intended for musicologists and linguists who work with digital data and are interested in the lyrical evolution of Arctic Monkeys.
## Text selection
One song per album, usually the one with the most text, was selected to keep the corpus minimal. However, including every song from all albums would ensure more accurate analysis. 
## Data collection
Lyrics were collected from Genius.com and copy/pasted into a plain .txt file. Each song is stored as a separate .txt file within the data folder.
Moreover, metadata (title, author, and year) was compiled in a CSV file. 
## Cleaning and preprocessing 
The text was normalized for the following: 
1. Lowercasing
2. Contractions (e.g., wanna -> want to)
3. Grammar (e.g., dancin' -> dancing)
## Annotations
Using spaCy (en_core_web_sm), the following annotations were added:
1. Tokens
2. Lemmas
3. Parts-of-Speech (POS)
4. Proper nouns
5. Named entities
6. NE words
## Corpus format 
1. Data folder contains raw .txt files and metadata.csv
2. annotated_dataset.csv file contains:
   - Filename
   - Title
   - Album
   - Year
   - Document (original text)
   - Text (preprocessed text for analysis)
   - Lemmas
   - POS
   - Proper_Nouns
   - Named_Entities
   - NE_Words
## Quality checks 
The annotated_dataset.csv file was checked whether it corresponds to original data as well as if spaCy's tools worked. Although I still have questions about why some of the Proper_Nouns were filtered, most of them are indeed proper nouns. Nevertheless, including contractions and grammar normalization did help for the most part.
## Additional notes 
The corpus is still very small, but this can be expanded by including the lyrics from all songs from each album. 
