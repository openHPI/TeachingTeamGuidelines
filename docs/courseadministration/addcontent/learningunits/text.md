# Text

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/787824320?h=1f73c65841&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="openHPI-guidelines-14-text"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>


All reading material of the course can be carried out in three different formats: 

 - directly as a text page
 - as a PDF download
 - as a web link

To be properly displayed in mobile apps, text pages cannot contain other formatting options than markdown.
Although HTML is allowed to be used for particular purposes, we strongly discourage its use as it will not be rendered but shown as source code in the mobile apps.
  
Next to simple formatting options such as headlines, bold and italic text, lists, etc., the supported markdown allows to include images and links to download files, create weblinks, and insert tables. 

Icon type:
You can select different icon types from the icon type dropdown to be shown to the participants in the item menu.

# Some Markdown examples

## Headlines

# H1  `# H1`

## H2 `## H2`

### H3 `### H3`

#### H4 `#### H4`

##### H5 `##### H5`

###### H6 `###### H6`

## Paragraph and Linebreaks

I am a 

paragraph (Add two "linebreaks" at the end of the line)

I am a (forced)  
Linebreak (Add two "spaces" at the end of the line before the linebreak)

I am 
nothing (Just a simple linebreak)

## Horizontal lines

---
A line can be created by three consecutive minus signs (-).

## Lists

 - I 
 - am 
    - an 
    - unordered
 - List 

` - I` (space + minus sign)  
` - am` (space + minus sign)  
&nbsp;&nbsp;&nbsp;`- an`  (Add additional spaces to create hierarchy levels)  
&nbsp;&nbsp;&nbsp;` - unordered`   
` - List` (Or remove them again to jump back to the higher hierarchy level) 

 

 1. I 
 2. am  
    a. an  
    b. ordered 
 3. List 

` 1. I` (space + 1.)  
` 2. bin` (space + 2.)  
&nbsp;&nbsp;&nbsp;`a. eine`  (Add additional spaces to create hierarchy levels)  
&nbsp;&nbsp;&nbsp;`b. geordnete`   
` 3. Liste` (Or remove them again to jump back to the higher hierarchy level) 

Lists with nested hierarchy levels can become tricky. If necessary, experiment with the proper amount of spaces. Make sure to add a paragraph (two line breaks) before and after a list.

## Links

Links werden am besten mittels des Link Tools in der Tool-Leiste eingefügt. Komplette URLs werden in der Regel zwar auch automatisch in Links konvertiert, verhalten sich aber nicht immer identisch zu explizit angelegten Links.

Hier ist das [HPI][1].

Explizit angelegte Links bestehen aus zwei Komponenten:  

 1. Der Aufruf des Links im Text  
\[HPI\]\[1\]

 2. Die Definition des Links am Ende des Texts (für den Nutzer nicht sichtbar)  
  \[1\]\: https://www.google.de/maps/place/Hasso+Plattner+Institute/@52.3939998,13.1311717,17z/data=!3m1!4b1!4m5!3m4!1s0x47a85f365d286349:0x1da4e14975e45e72!8m2!3d52.3939965!4d13.1333657


## Bilder

Bilder werden mittels der Drop-Area rechts zunächst hochgeladen und stehen dann im Kontext der aktuellen Textseite über den "Bild einfügen" Button zur Verfügung. hochgeladene Bilder werden erst dann persistiert wenn das Bild tatsächlich in den Text eingebunden wurde. Nicht verwendete Bilder werden früher oder später wieder vom Server gelöscht.

Bilder werden mittels des Image-Selectors in der Tool-Leiste der Text-Area eingebunden.

Das eingefügte Bild wird im Text folgendermaßen dargestellt:    
\!\[enter image description here]\[1]

Hier muss der Text in den vorderen eckigen Klammern:   
"enter image description here"  
durch einen dem Bild entsprechenden Alt-Text getauscht werden.  
\!\[Plastikschaf auf Rasenmähroboter]\[1]

![Plastikschaf auf Rasenmähroboter][2]

## Downloads

Andere Dateiformate die zum Download bereitgestellt werden sollen, werden identisch zu den Bildern eingebunden. 

![enter image description here][3]   
\!\[enter image description here\]\[2]

Im Nachgang muss das `!` vor den eckigen Klammern entfernt werden und ein vernünftiger Text zur Beschriftung des Download-Links eingefügt werden.

[Download][4]  
\[Download]\[2]

To link a file for download:

- Upload the file via the file upload drop zone next to the text input field.
- Click on the add image icon and select the file that you have just uploaded.
- In the text field: **remove** the "!" in front of the download link and add some meaningful text within the brackets


## Tabellen

|Month|Savings|Spending|
|--- |--- |--- |
|January|$100|$900|
|July|$750|$1000|
|December|$250|$300|
|April|$400|$700|

\|Month|Savings|Spending|  
|- - - |- - - |- - - |  (Leerzeichen sind nur zur besseren Lesbarkeit eingefügt)   
|January|$100|$900|  
|July|$750|$1000|  
|December|$250|$300|  
|April|$400|$700|  

Um Markdown-Tabellen zu benutzen, empfiehlt es sich einen [Konverter][5] zu benutzen.


  [1]: https://www.google.de/maps/place/Hasso+Plattner+Institute/@52.3939998,13.1311717,17z/data=!3m1!4b1!4m5!3m4!1s0x47a85f365d286349:0x1da4e14975e45e72!8m2!3d52.3939965!4d13.1333657
  [2]: s3://moochouse-public/courses/5IrTNQ46jTgyCZkhYpzOYI/rtfiles/7mIXt6yWtw4ILOvNdnVATS/dolly.png
  [3]: s3://moochouse-public/courses/5IrTNQ46jTgyCZkhYpzOYI/rtfiles/5uEwOdjFkmM3VheUmEYUCH/1_UploadTest-Ludwigshafen.pdf
  [4]: s3://moochouse-public/courses/5IrTNQ46jTgyCZkhYpzOYI/rtfiles/5uEwOdjFkmM3VheUmEYUCH/1_UploadTest-Ludwigshafen.pdf
  [5]: https://jmalarcon.github.io/markdowntables/

![HPI Logo](../../../img/HPI_Logo.png)
