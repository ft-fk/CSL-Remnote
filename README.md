# CSL-Remnote: Structure your document's metadata in Remnote
CSL (citation language style) to cite document from Mendeley/Zotero in Remnote-Md  
for : remnote.com

_If you are not familiar with CSL or github, do not fear: there is a section at the bottom with detailled installation procedure._

## How does it work?
### Offers a structure to import PDF's metadata (via library manager) in Remnote.   
In short 2 things are acheived (for a full list of actions performed see below):
- Authors, Journals, year of Issue are created (or linked if they already exist in your Remnote) as child of top-level rems with according name:_Authors_ or _Journals_ etc. This is so that all authors, journals etc are always in a single rem.
- it creates a rem, with the following structure (see below), containing all necessary references (Authors etc) under which you can take notes about the PDF. V2 adds an Alias to the rem, in the format of "Authors, date", making citing while writing easier on the eye.


### An example of what this CSL does
You want to add a paper you have in Zotero/Mendeley to your remnote knowledge base.
Using the CSL, your paper "Weaver, W. Science and Complexity. Am. Sci. 36, 536–544 (1948)" now have this format:  

>**Science and Complexity**, Weaver, [[Issued/1948]]   
>
>      [[~/Aliases]]  
>           Weaver, 1948              
>      [[People/Authors/Weaver, Warren]]
>      [[Issued/1948]], in [[Journals/American Scientist]]      
>      ##1-line-abstract      
>      ##Topics


Once pasted into remnote, this is what you get  
<img src="https://user-images.githubusercontent.com/79699896/151702900-e8144539-b933-43b7-a5d9-95e78c2cb2ed.png" width="700" />

### Complete description of what this CSL does when used  
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

## To use do the following: 
  - Install CSL in you library manager if you don't know how see below)
  - don't forget to select the "Remnote Remnote-MD" style in your style manager
  - paste (CTRL+SHIFT+V) the bibliography created by your library manager (make sure you are using the bibliography, and not the CWYW)


## installing the CSL (zero prior knowledge)
### Do this
1. Download the CSL
![image](https://user-images.githubusercontent.com/79699896/151703648-9acae273-aeb9-4145-8b9f-0a8869d8d343.png)
2. Save the zip file somwhere you know of
3. unzip the file, and locate the file with extension CSL
4. head to you library manager : Zotero or Mendeley

### then, for Zotero
After you have performer action 1 -> 4
- ![image](https://user-images.githubusercontent.com/79699896/151704020-14af5846-43aa-4086-a0d2-d4fd5527ba65.png)
- locate the file with extension CSL you just downloaded
- ignore warning about compability

### or, then, for Mendeley
After you have performer action 1 -> 4
- ![image](https://user-images.githubusercontent.com/79699896/151704211-48f43fe1-c9d7-44bb-a31a-d2dbfeaf6c7a.png)
- click and drag the CSL file you just downloaded in the window that appeared in Mendeley
