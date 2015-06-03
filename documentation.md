<h1>Franz Richard Behrens‘ <em>Feldtagebuchgedichte (1915/1916)</em> in <em>Emophon</em></h1>

<p><strong>Nora Lötscher, Michèle Steiner, Birgit Zehnder</strong></p>

<p>The computer program Emophon was developed by Arash Aryani, Arthur M. Jacobs and Markus Conrad (see Arash Aryani, Arthur M. Jacobs, Markus Conrad: "Extracting salient sublexical units from written texts. „Emophon,“ a corpus-based approach to phonological iconicity". In: <em>Frontiers in psychology 01/2013 04:654</em>). It allows us to examine the intended emotional meaning of a text which is based on sublexical phonological salience. «Salience» means an overproportional use of an element in a text. The frequencies of some elements get compared with a linguistic corpus (SUBTLEX-DE) – the higher the difference between the relative frequency of a specific element in a given text and the linguistic reference corpus, the more important this may element be. The relationship between linguistic form and emotional content is called «iconicity».
The whole tool was written in Python (V2.5).</p>

<p>For her Bachelor thesis, Birgit would like to search Franz Richard Behrens’ „Feldtagebuchgedichte“ with Emophon. He was a German poet who was born 1895 and died 1977. To get an overview of his poems and to form the hypotheses it is very helpful to count the words and letters and to bring them in an order of frequency. Therefore, we made a little program as a project in the course „Tools and Techniques for Digital Humanities“.               </p>

<h2>Our Project</h2>

<p>First of all, we needed to digitize all the poems to be able to work with them. We did this with OCR recognition of speech. As well as this tool may work, we still needed to check every poem by hand to make sure they are all correctly digitized and to change anything that was still incorrect.</p>

<p>In a second step, we read all the poems into an iPython Notebook and wrote our program that allows us to analyse the following aspects:</p>

<ul>
<li>count the total words in a poem</li>
<li>count the periods in a poem (which will probably not be useful for the thesis, we were just playing around a little)</li>
<li>show the frequencies of the used words in graphs</li>
<li>show the frequencies of the used letters in graphs (which could be helpful in order to investigate the emotional meaning of the poems)</li>
<li>tag the poems according to parts of speech and show their frequencies in graphs</li>
</ul>

<p>Unfortunately some problems occurred with the POS-tagging, since the NLTK tool that is available in iPython is not very good at tagging German. Consequently, most of the words have been tagged as NNPs (which are proper nouns), because the tagger didn’t recognize some words and therefore simply interpreted them as names. We tried solving this problem by using another tagger, namely the TreeTagger, but we didn’t manage to run this in iPython, so we had to stick to the partly incorrect tags of the NLTK POS tagger in the end. Thus, the graphs depicting the POS frequencies are not correct either.</p>

<p>To make parts of our project graphically visible, we designed some graphs (again in an iPython notebook) that show the letters used most frequently in six randomly chosen poems. One graph just shows the three most used letters and the final one shows the three vowels and the three consonants that were used the most for each poem, which yields a more interesting result.
The advantage of our analysis program is that more poems (or other texts as well) could be added very easily since they only need to be available in .txt format and can then be read into the iPython notebook without any problems. The program knows how to split the poems (if they are separated by more than two line breaks), so they don’t even have to be in individual files, which makes life much easier if one looks at so many poems at the same time.</p>

<p>Finally, we are hoping that our little project or at least some parts of it will help Birgit with her Bachelor thesis and wish her all the best for finishing it :)</p>
