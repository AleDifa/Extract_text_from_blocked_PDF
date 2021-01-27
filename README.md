# Extract text from blocked PDF

PDFMiner is a text extraction tool for PDF documents. 
This simple script help you to read and extract text from PDF file.<br/>

### A typical way to parse a PDF file is the following:
<br>
<br>
Create a PDF resource manager object that stores shared resources.

```python
resource_manager = PDFResourceManager()

fake_file_handle = io.StringIO()
converter = TextConverter(resource_manager, fake_file_handle, laparams=LAParams())
page_interpreter = PDFPageInterpreter(resource_manager, converter)
```

Create a PDF page aggregator object.

```python
with open('C:/Users/Alessandro/Desktop/Sacha Baron Cohen Actor.pdf', 'rb') 
```
> in this row you can insert your route folder to get to the file:<br/>
>In my case, is Disk C, Alessandro folder, in Desktop and the name of Pdf is Sacha Baron Cohen Actor.<br/>
>For have the same result you can copy this code and change the route with your pdf. <br/>
<br>
<br>
Process each page contained in the document.

```python
for page in PDFPage.get_pages(fh,
                                  caching=True,
                                  check_extractable=True):
        page_interpreter.process_page(page)
        
print(text)
```
> See in output the pdf 


Sacha Baron Cohen’s Political Cinema 

Sacha Baron Cohen’s political views have never been a mystery to his international audience. Source: 
POLITICO  

Sacha Baron Cohen‟s films have proved wild and eye-opening time and time again. While creating 
his most prominent characters in the 1990s, the actor and comedian kickstarted his iconic 
filmography in 2002 with Ali G. Indahouse. Since then, Baron Cohen has written, produced and 
starred in films that, despite their extreme characters and plots, are all commonly laced with 
political commentary and satire. His latest instalment, Borat Subsequent Moviefilm, is yet another 
comedy that explores several political issues.  

This article looks at some of Sacha Baron Cohen‟s most prominent work, exploring whether the 
political satire transgressing these films is in fact mere satire, or if it can qualify as political 
activism. Where Sacha assumes the role of activist, what exactly does he contribute to politics 
through his films?  

BORAT (2006)  

If you are unfamiliar with some of Sacha Baron Cohen‟s early skits, the first Borat film introduces 
the character of Kazakh journalist Borat Sagdiyev, who travels to the United States of America to 
learn about American culture. Set against the context of the US‟ War in Iraq, also termed the War 
on Terror, and shot only a few years after 9/11, the film explores American attitudes to foreigners 
and those perceived as not American. While Sacha Baron Cohen‟s interpretation of a foreigner in 
the US is extreme, conceiving bizarre cultural differences and expressing the character‟s own racist, 
sexist, and anti-Semitic views along the way, his performance successfully elicits concrete feelings 
and attitudes from the Americans he encounters.  

