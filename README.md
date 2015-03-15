# Clay

Clay is a computable document creation tool that allows you to write text and
arbitrary Javascript code and see the results of that code. Clay is the
document and also the tool; when you create a document using clay and save it
as another HTML file, that HTML file can also create documents.

Specifically, it's a single HTML file with zero outside dependencies that
allows you to experiment with arbitrary Javascript code and also save all your
work including the output, ready to edit when the saved file is loaded again.

## Notes from the beginning of the project

**Goal:** an easy to share, easy to use document-creating tool, where the document is also the tool to create documents and you can write code and see the output and then save the code and the output... all of it as data.

Where you can have arbitrary code blocks that are syntax highlighted and look like those programming blog posts, but you can edit the code of existing blocks and recompute the output or add new code blocks.

**Design goal:** no needless dependencies! Only dependencies that are actually crucially needed, and even then include them grudgingly! It's a great thing to not depend on too much code, it forces you to say no to features for one, and it teaches you about the underlying platform, and if you go native-first, you only add that stuff that actually solves a DRYness probably or actually provided a useful abstraction, rather than a whole abstraction of which you only need a small part

**Design goal:** code is data, data is code. Save the html file as a single file and then run it! Perhaps even a button to allow saving
