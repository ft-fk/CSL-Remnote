# CSL-Remnote v2
CSL (citation language style) to cite document from Mendeley/Zotero in Remnote-Md

for : remnote.io

**Offer a structure for the import of PDF (via library manager) in Remnote**. 
Authors, Journals, year of Issue are created as child rem of document with according name.
**New in V2:**) adds an Alias to the rem, in the format of "Authors, date", making citing while writing easier on the eye.



**To use do the following:**
  - Install CSL in you library manager
  - don't forget to select the "Remnote Remnote-MD v2" style in your style manager
  - paste (CTRL+SHIFT+V) the bibliography created by your library manager (make sure you are using the bibliography, and not the CWYW)

**example**
>    **Science and Complexity**, Weaver, [[Issued/1948]]
   
>      [[~/Aliases]]       
>              Weaver, 1948              
>      [[People/Authors/Weaver, Warren]]
>      [[Issued/1948]], in [[Journals/American Scientist]]      
>      ##1-line-abstract      
>      ##Topics




**Complete description of what this CSL does when used:**
- Add each author separately by the structure "Last name, First Name" under the rem "Authors", which is nested under the top-rem "People". If not existing, this structure will be created.
- Add the  year of publication under the top-rem "Issued". If not existing, this structure will be created.
- Add the journal under the top-rem "Journals". If not existing, this structure will be created.
- Rem creation: where you paste the bibliographical information using this CSL, a new rem is created with the following structure "Title, short authors, year". (short authors means the author last name or, if there are multiples athors : first author last name et al.)
- Creates an alias for the rem created with the following structure "last name 1st author, year" → allows easy citation
- Nested under the above mentioned rem, are listed :
   - all authors in one line as reference to the adequate rem (see above)
   - year of issue, as reference to the adequate rem (see above)
   - the journal, as reference to the adequate rem (see above)
   - a blank line, tagged with "1-line-abstract", fot the purpose of writing down a very brief summary of document objectives. 
   - a blank line, tagged with "Topics", to list all possible connection to majors "topics" of your knowledge base
