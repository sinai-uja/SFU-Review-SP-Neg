===============================================================================

SFU Review SP-NEG corpus

Web site: http://sinai.ujaen.es/sfu-review-sp-neg-2/

Authors: Salud María Jiménez-Zafra, Mariona Taulé, M Teresa Martín-Valdivia, L Alfonso Ureña-López, M Antónia Martí
===============================================================================

------------------------------------
LICENSE
------------------------------------

This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.
https://creativecommons.org/licenses/by-nc-sa/4.0/

-------------
REFERENCES
-------------

Please, if you use the corpus, cite it:

Jiménez-Zafra, S. M., Taulé, M., Martín-Valdivia, M. T., Ureña-López, L. A., & Martí, M. A. (2018a). SFU Review SP-NEG: a Spanish corpus annotated with negation for sentiment analysis. A typology of negation patterns. Language Resources and Evaluation, 52(2), 533-569.

Jiménez-Zafra, S. M., Martín-Valdivia, M. T., Molina-González, M. D., & Ureña-López, L. A. (2018b). Relevance of the SFU Review SP-NEG corpus annotated with the scope of negation for supervised polarity classification in Spanish. Information Processing & Management, 54(2), 240-251.

Jiménez-Zafra, S. M., Martin, M., Lopez, L. A. U., Marti, T., & Taulé, M. (2016). Problematic cases in the annotation of negation in Spanish. In Proceedings of the Workshop on Extra-Propositional Aspects of Meaning in Computational Linguistics (ExProM) (pp. 42-48).

Martí, M. A., Martín-Valdivia, M. T., Taulé, M., Jiménez-Zafra, S. M., Nofre, M., & Marsó, L. (2016). La negación en español: análisis y tipología de patrones de negación. Procesamiento del Lenguaje Natural, 57, 41-48.

-------------
CONTACT
-------------

For any questions related to the corpus, please send an email to Salud María Jiménez-Zafra (sjzafra@ujaen.es)

------------------------------------
DESCRIPTION
------------------------------------

This corpus is an extension of the SFU Spanish Review Corpus (Brooke et al., 2009) with annotations about negation and its scope. It is a collection of 400 reviews of cars, hotels, washing machines, books, cell phones, music, computers and movies from the Ciao.es website. Each domain contains 25 positive and 25 negative reviews. Each review has been annotated at the token level with the lemma and the PoS and at the sentence level with negative keywords, their linguistic scope, the event and how the polarity of the sentence is affected by negation (if there is a change in the polarity or an increment or reduction of its value), also taking into account intensifiers and diminishers.

The SFU ReviewSP-NEG corpus (Jiménez-Zafra et al., 2018a) is an extension of the Spanish part of the SFU Review corpus (Taboada et al., 2006) and it could be considered the counterpart of the SFU Review Corpus with negation and speculation annotations (Konstantinova et al., 2012). The Spanish SFU Review corpus consists of 400 reviews extracted from the website Ciao.es that belong to 8 different domains: cars, hotels, washing machines, books, cell phones, music, computers, and movies. For each domain there are 50 positive and 50 negative reviews, defined as positive or negative based on the number of stars given by the reviewer (1-2=negative; 4-5=positive; 3-star review were not included). Later, it was extended to the SFU ReviewSP-NEG corpus in which each review was automatically annotated at the token level with pos-tags and lemmas, and manually annotated at the sentence level with negation cues and their corresponding scopes and events. Moreover, it is the first corpus in which it was annotated how negation affects the words that are within its scope, that is, whether there is a change in the polarity or an increment or reduction of its value.

The corpus was automatically tokenized, PoS tagged and lemmatized using Freeling and then, it was manually annotated with negation and polarity information applying the procedure described in (Jiménez-Zafra et al., 2018a).

-------------
FORMAT
-------------

The data are provided in CoNLL format. Each line corresponds to a token and each annotation is provided in a column; empty lines indicate end of sentence. The content of the columns given is:


Column 1: domain_filename

Column 2: sentence number within domain_filename

Column 3: token number within sentence

Column 4: word

Column 5: lemma

Column 6: part-of-speech

Column 7: part-of-speech type

Columns 8 to last:

- If the sentence has no negations,  column 8 has a "***" value and there are no more columns.
- If the sentence has negations, the annotation for each negation is provided in three columns. The first column contains the word that belongs to the negation cue. The second column contains the word if it belongs to the scope of the negation cue or "-" if it does not belong. The third column contains the word if it belongs to the event of the negation cue or "-" if it does not belong.

In Example 1 there is no negation so the 8th column is "***" for all tokens. Example 2 is a sentence with one negation cue and the information about negation is provided in colums 8-10. Example 3 is a sentence with two negation cues in which information for the first negation is provided in columns 8-10, and for the second in columns 11-13. 

Example 1 - Sentence without negation: the 8th column is "***" for all tokens.

	hoteles_no_1_1	1	1	Me	me	pp1cs000	personal	***	
	hoteles_no_1_1	1	2	he	haber	vaip1s0	auxiliary	***	
	hoteles_no_1_1	1	3	alojado	alojar	vmp00sm	main	***	
	hoteles_no_1_1	1	4	en	en	sps00	preposition	***	
	hoteles_no_1_1	1	5	dos	2	z	-	***	
	hoteles_no_1_1	1	6	ocasiones	ocasión	ncfp000	common	***	
	hoteles_no_1_1	1	7	en	en	sps00	preposition	***	
	hoteles_no_1_1	1	8	este	este	dd0ms0	demonstrative	***	
	hoteles_no_1_1	1	9	hotel	hotel	ncms000	common	***	
	hoteles_no_1_1	1	10	,	,	fc	-	***	
	hoteles_no_1_1	1	11	y	y	cc	coordinating	***	
	hoteles_no_1_1	1	12	lo	el	da0ns0	article	***	
	hoteles_no_1_1	1	13	único	único	aq0ms0	qualificative	***	
	hoteles_no_1_1	1	14	que	que	pr0cn000	relative	***	
	hoteles_no_1_1	1	15	destaco	destacar	vmip1s0	main	***	
	hoteles_no_1_1	1	16	es	ser	vsip3s0	semiauxiliary	***	
	hoteles_no_1_1	1	17	su	su	dp3cs0	possessive	***	
	hoteles_no_1_1	1	18	ubicación	ubicación	ncfs000	common	***	
	hoteles_no_1_1	1	19	,	,	fc	-	***	
	hoteles_no_1_1	1	20	cerca	cerca	rg	-	***	
	hoteles_no_1_1	1	21	de	de	sps00	preposition	***	
	hoteles_no_1_1	1	22	Sol	sol	np00000	proper	***	
	hoteles_no_1_1	1	23	,	,	fc	-	***	
	hoteles_no_1_1	1	24	de	de	sps00	preposition	***	
	hoteles_no_1_1	1	25	la	el	da0fs0	article	***	
	hoteles_no_1_1	1	26	Gran_Vïa	gran_vïa	np00000	proper	***	
	hoteles_no_1_1	1	27	,	,	fc	-	***	
	hoteles_no_1_1	1	28	muy	muy	rg	-	***	
	hoteles_no_1_1	1	29	bien	bien	rg	-	***	
	hoteles_no_1_1	1	30	situado	situar	vmp00sm	main	***	
	hoteles_no_1_1	1	31	.	.	fp	-	***

Example 2 - Sentence with negation: the columns for negation start at the 8th columns. There will be three columns for each negation (cue, scope, event) and three colums for each token that is not a negation cue (-, -, -).

	hoteles_no_1_4	11	1	Me	me	pp1cs000	personal	ci	2	-	-	-	
hoteles_no_1_4	11	2	quedé	quedar	vmis1s0	main	sentence	0	-	-	-	
hoteles_no_1_4	11	3	pensando	pensar	vmg0000	main	cc	2	-	-	-	
hoteles_no_1_4	11	4	como	como	cs	subordinating	cc	3	-	-	-	
hoteles_no_1_4	11	5	seria	seriar	vmip3s0	main	s.a	4	-	-	-	
hoteles_no_1_4	11	6	para	para	sps00	preposition	cc	3	-	-	-	
hoteles_no_1_4	11	7	un	uno	di0ms0	indefinite	spec	8	-	-	-	
hoteles_no_1_4	11	8	minusválido	minusválido	ncms000	common	sn	6	-	-	-	
hoteles_no_1_4	11	9	tener	tener	vmn0000	main	sn	6	-	-	-	
hoteles_no_1_4	11	10	que	que	cs	subordinating	cd	11	-	-	-	
hoteles_no_1_4	11	11	subir	subir	vmn0000	main	S	9	-	-	-	
hoteles_no_1_4	11	12	aquellas	aquel	dd0fp0	demonstrative	spec	13	-	-	-	
hoteles_no_1_4	11	13	escaleras	escalera	ncfp000	common	cd	11	-	-	-	
hoteles_no_1_4	11	14	mal	mal	rg	-	cc	15	-	-	-	
hoteles_no_1_4	11	15	hechas	hacer	vmp00pf	main	S	13	-	-	-	
hoteles_no_1_4	11	16	y	y	cc	coordinating	coord	3	-	-	-	
hoteles_no_1_4	11	17	sin	sin	sps00	preposition	S	3	sin	sin	-	
hoteles_no_1_4	11	18	rampa	rampa	ncfs000	common	sn	17	-	rampa	rampa	
hoteles_no_1_4	11	19	.	.	fp	-	f	2	-	-	-

Example 3 - Sentence with two negations: the information for the first negation is provided in columns 8-10, and for the second in columns 11-13. There will be three columns for each negation (cue, scope, event) and three colums for each token that is not a negation cue (-, -, -).

hoteles_no_2_6	9	1	Aun	aun	np00000	proper	cc	3	-	-	-	-	-	-	
hoteles_no_2_6	9	2	estoy	estar	vaip1s0	auxiliary	v	3	-	-	-	-	-	-	
hoteles_no_2_6	9	3	esperando	esperar	vmg0000	main	sentence	0	-	-	-	-	-	-	
hoteles_no_2_6	9	4	que	que	cs	subordinating	suj	6	-	-	-	-	-	-	
hoteles_no_2_6	9	5	me	me	pp1cs000	personal	ci	6	-	-	-	-	-	-	
hoteles_no_2_6	9	6	carguen	cargar	vmsp3p0	main	S	3	-	-	-	-	-	-	
hoteles_no_2_6	9	7	los	el	da0mp0	article	spec	8	-	-	-	-	-	-	
hoteles_no_2_6	9	8	puntos	punto	ncmp000	common	suj	6	-	-	-	-	-	-	
hoteles_no_2_6	9	9	en	en	sps00	preposition	cc	6	-	-	-	-	-	-	
hoteles_no_2_6	9	10	mi	mi	dp1css	possessive	spec	11	-	-	-	-	-	-	
hoteles_no_2_6	9	11	tarjeta	tarjeta	ncfs000	common	sn	9	-	-	-	-	-	-	
hoteles_no_2_6	9	12	más	más	rg	-	sadv	11	-	-	-	-	-	-	
hoteles_no_2_6	9	13	,	,	fc	-	f	3	-	-	-	-	-	-	
hoteles_no_2_6	9	14	no	no	rn	negative	mod	15	no	no	-	-	-	-	
hoteles_no_2_6	9	15	sé	saber	vmip1s0	main	S	3	-	sé	sé	-	-	-	
hoteles_no_2_6	9	16	dónde	dónde	pt000000	interrogative	cc	17	-	dónde	-	-	-	-	
hoteles_no_2_6	9	17	tienen	tener	vmip3p0	main	cd	15	-	tienen	-	-	-	-	
hoteles_no_2_6	9	18	la	el	da0fs0	article	spec	19	-	la	-	-	-	-	
hoteles_no_2_6	9	19	cabeza	cabeza	ncfs000	common	cd	17	-	cabeza	-	-	-	-	
hoteles_no_2_6	9	20	pero	pero	cc	coordinating	coord	17	-	-	-	-	-	-	
hoteles_no_2_6	9	21	no	no	rn	negative	S	17	-	-	-	no	no	-	
hoteles_no_2_6	9	22	la	lo	pp3fsa00	personal	S	17	-	-	-	-	la	-	
hoteles_no_2_6	9	23	tienen	tener	vmip3p0	main	S	17	-	-	-	-	tienen	tienen	
hoteles_no_2_6	9	24	donde	donde	pr000000	relative	cc	25	-	-	-	-	donde	-	
hoteles_no_2_6	9	25	deberían	deber	vmic3p0	main	S	17	-	-	-	-	deberían	-	
hoteles_no_2_6	9	26	.	.	fp	-	f	3	-	-	-	-	-	-	

===============================================================================