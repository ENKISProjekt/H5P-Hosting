# ENKIS Project H5P for Moodle
Host H5P file with Github pages and import it to moodle.

FAQ: Why can't I just use the all-in-one HTML?
A: You can! However, this HTML file gets very large from time to time, which makes it very difficult to upload to Github. If you managed to upload an html file, Great! You won't need this information. To do that with this repository, please upload your html file to the root directory (of the main branch of course). To link that html file to Moodle, Please jump ahead to section 4.

Knowledge with Github is assumed for this instruction.
If something doesn't work, send your h5p file to Hans, he will take care of it then ;)

## Section 1. Break H5P into Pieces
After you finished editing your H5P file, make a copy of it. Change its file type (e.g. something.h5p --> something.zip). Then unzip the file. 

### In MAC
Sorry, I haven't used MAC and do not exactly know if the same will work in Mac, but this should work similarly for other compression methods. 

## Section 2. Download this Repository
Your unzipped folder will probably contain very many subfolders and files. By drag and drop to Github, you can only upload up to 100 files, which won't be enough.

Make an empty folder on your computer. Clone this repo to your folder. 

## Section 3. Put your H5P to the Git-linked Folder
In 'h5p-standalone-1.3.x/workspace', make a new folder. IMPORTANT: remember this name exactly, let's call this EXAMPLE for now. In 'h5p-standalone-1.3.x/workspace/EXAMPLE' copy all of the folders and files. 

In 'h5p-standalone-1.3.x/demo', copy "Template.html" and name your copied file to "EXAMPLE.html". Of course, change EXAMPLE to your folder name from above. In "Replace me with H5P name" part, change this to "EXAMPLE". Don't forget to un-comment it. 

Push this to the repo. Wait for a few minutes. Your H5P file should be hosted at https://enkisprojekt.github.io/H5P-Hosting/h5p-standalone-1.3.x/demo/Example.html


## Section 4. Link this to Moodle.
Go to the Moodle page you want to add your H5P to.  
Add the following source code to the part you want to insert your H5P.
Change the first src of iframe to your URL from above.
<div>
    <iframe src="https://hyunchangoh.github.io/h5p/Supervised%20Learning%20-%20Biology.html" width="3000" height="1720" frameborder="0" allowfullscreen="allowfullscreen" title="Explore the Data" style="width: 100%; height: 193px;"></iframe>
    <script src="https://moodle.mi.fu-berlin.de/moodle/mod/hvp/library/js/h5p-resizer.js" charset="UTF-8"></script><br>
</div>

### Disclaimer

 This repository was built using the same code from tunapanda https://github.com/tunapanda/h5p-standalone/tree/1.3.x. And Got help from the tutorial https://isu.pressbooks.pub/openpedagogy/chapter/self-hosting-h5p/, from which I cloned this repository originally.
