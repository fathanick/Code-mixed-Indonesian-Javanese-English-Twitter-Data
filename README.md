# Code-mixed-Indonesian-Javanese-English-Twitter-Data

This is a clean version of code-mixed Indonesian-Javanese-English data for token level language identification.
This dataset contains tweets that have been tokenized with the corresponding token and its language label.
There are seven language labels in the dataset, namely: 
1. ID (Indonesian), 
2. JV (Javanese), 
3. EN (English), 
4. MIX_ID_EN (mixed Indonesian-English), 
5. MIX_ID_JV (mixed Indonesian-Javanese), 
6. MIX_JV_EN (mixed Javanese-English), 
7. OTH (Other).

### Annotation Guideline

1.	The ID label is used to annotate Indonesian words, including both standard and non-standard forms of Indonesian words. 
2.	The EN label is used to annotate English words, including both standard and non-standard forms of English words.
3.	The JV label is used to annotate Javanese words, including both standard and non-standard Javanese words.
4.	The MIX_ID_EN label is used to annotate words containing mixed Indonesian-English. For example:
		
		a. diprint (printed) => di- (Indonesian prefix) + print (English).
		b. filenya (the file) => file (English) + -nya (Indonesian suffix).
		
5.	The MIX_ID_JV label is used to annotate words containing mixed Indonesian-Javanese. For instance:
		
		a. bajune (the clothes) => baju (Indonesian) + ne (Javanese suffix).
		b. penjuale (the seller) => penjual (Indonesian) + e (Javanese suffix).
		
6.	The MIX_JV_EN label is used to annotate words containing mixed Javanese-English. For example:

		a. endinge (the ending) => ending (English) + -e (Javanese suffix).
		b. ngemailke (send email) => ng- (Javanese prefix) + email (English) + -ke (Javanese prefix). 
		
7.	The OTH (Other) label is used to annotate the following:

		- symbols, punctuations, and number,
		- unknown words, words other than Indonesian, Javanese, and English,
		- Twitter entities: username or mention,
		- URL, emoji, emoticons, date, time, and currency,
		- laugh expressions (haha, xixixi, wkwkwk) and sad expressions (huhuhu, hiks). 
		
8.	If a word (w) exists in more than one language, it will be annotated as a particular language (ID, JV, or EN), depending on the context.

		- If w is preceded and followed by Javanese words, w is annotated as JV.
		- If w is preceded and followed by Indonesian words, w is annotated as ID.
		- If w is preceded and followed by English words, w is annotated as EN.
		
9.	Foreign or borrowed words that exist in all languages are identified depending on the context of tweets or sentences.
10.	A named entity followed by a possessive pronoun from a particular language can be labeled as ID or JV, depending on the context.
		
		- Macbookku (My Macbook) => Macbook (named entity) + -ku (Indonesian or Javanese suffix).
		- Macbooknya (The Macbook) => Macbook (named entity) + -nya (Indonesian suffix).

