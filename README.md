INSTRUCTIONS

1. In the ./Chapter folder, copy the chapters.  Remove "\label{Chaptername} \lhead{Chapter x. \emph{CHAPTERNAME}}" in each file.
2. In the ./Appendices folder, remove "\label{Appendix} \lhead{Appendix x. \emph{APPENDIXNAME}}" in each file.
3. In bethesis.tex, 
	a. Specify your project tilte in \settitle{your project title}
	b. Specify number of authors in \setnauthor{n}
	c. Specify your names and rollnumbers  in \setauthorone{name}{num}, \setauthortwo{name}{num}, \setauthorthree{name}{num} -- as many as needed.
	d. Specify your guide name and designation in \setguide{guide's name}{guide's designation}

4. Front matter
	a. Edit your abstract in ./FrontMatter/abstract.tex
	b. Edit your acknowledgements in ./FrontMatter/ack.tex

5. Add your citations in bethesis.bib

6. Add your acronyms in the ./FrontMatter/acronyms.tex file. Specify the longest acronym as parameter in \listofacronyms[longest acronym].

TO COMPILE LATEX
Linux
In the terminal, run:
	$ pdflatex bethesis.tex
	$ bibtex bethesis
	$ pdflatex bethesis.tex # needed only if citations in bethesis.tex or bethesis.bib is changed
	$ pdflatex bethesis.tex

In case of changes in main content only
	$ pdflatex bethesis.tex  # should suffice

Windows
Should be pretty much the same

For acronyms, check ftp://ftp.tex.ac.uk/tex-archive/macros/latex/contrib/acronym/acronym.pdf
http://en.wikibooks.org/wiki/LaTeX/ covers most things you'll need to work with LaTeX

# fyp-thesis
Thesis on Second Order Predictive Commoning in LLVM
Thesis guidelines

A. General: 
1. READ your thesis. 

B. Thesis contents:

1. Every figure, table, reference, or whatever SHOULD be referred in the text.

2. Abstract should preferably be less than a page. Three paragraphs if possible. Possibly: First para to briefly set the background to your work, middle para to describe your work, and the final paragraph to highlight your work, if any. 

3. The page after the English Abstract is for the Tamil Abstract(Thittappani Churukkam).  
You will have to type it out separately and insert that page here while printing/binding. (LaTeX does not support Tamil yet?)

Make sure you use the correct technical term in Tamil. You may refer to www.agaraadhi.com for technical terms in Tamil. 

The Tamil abstract is not expected to be a word-for-word translation. The Tamil abstract should describe your project on its own. 

C. Thesis format:
1. Cover should be pink. Choose the pink carefully. Not too pale, not too bright. A pleasant pink. 

2. A translucent butter paper will have to be inserted immediately after the cover page. 

The cover page content will be repeated again as the first page immediately after this first butter paper. 

There is one more butter paper immediately after this page.

Then the contents go in the natural flow as formulated in thesis.tex

3. LaTeX related:

Most of the LaTeX related doubts can be cleared by first finding a similar place in the bethesis.pdf, and then looking at the appropriate place in the .tex or .bib.  The bethesis covers most of the situations that are likely to occur. 

(For example, to force a upper case letter in an article title, enclose it in braces. That is, to get 'Reiser', use '{R}eiser'. So if you had found that your list of references shows it as 'reiser', you should have looked in bethesis.pdf, seen whether there is a similar situation, and then looked at the .tex or .bib to see how it is done. )

Most of the other issues are likely to be with your usage of LaTeX, rather than with the style file. Please check on the internet whether what you are doing is correct. Even if what you are doing is correct and there is some problem, find a "work around" to get what you want. 

( 
The following changes are only for next year's FYP batches, since it does not directly affect the output. 

The .bib file: 
Use some uniform style for the reference identifier eg authoryearkeyword eg ho2001future. 

Remember to separate author names with 'and'.  

Use 'others' if you need a 'et al' in the output. 
)

D. Submission: 

1. Print and bind the Thesis ONLY after approval by your guide.

2. Number of copies: 3 

(No need to submit a copy to your guide. One of these copies will be given to him/her by the committee.)

3. Sign the appropriate pages and get your guide's and HoDs signatures and submit the hard copy.

4. Deadline: Mon 13 May afternoon. Bound, signed copies signed by guide and HoD. 

5. Email the PDF to cse.fyp@gmail.com with cc: to your guide.
