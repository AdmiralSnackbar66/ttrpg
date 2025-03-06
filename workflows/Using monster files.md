
## Description

This workflow shows you how to get the monster files in `monsters` to show the following things:
- full frontmatter including its name, HP, size, environment, etc-- all the stats you need to know
- a Source link to the book it came from, which opens to the page in the PDF if you have it
- an embed of the PDF within the note

## Plugins used

- Better PDF
- Templater
- Dataview

![[Using Table of Contents for sourcebooks#Zotero]]

## Instructions

1. Follow the instructions in [[Using Table of Contents for sourcebooks]] to replace the Zotero IDs for the relevant book with *your* Zotero ID.
2. Create a *symlink* from wherever your PDFs are stored on your machine to the `sources/pdfs` folder in this vault. You'll need to search for how to do this in your operating system. At the end of it, you should have a symlink of all your PDFs from your Obsidian vault (although they're not actually stored in your vault).
3. Use the Global Search and Replace plugin to search for the *filename* of the PDF that's in the monster file and replace it with *your filename*. For example, in the monster [[Aalpamac]], this line shows the filename it's looking for: `"url": "[[Tome of Beasts 2.pdf]]",`. However, your Tome of Beasts 2 PDF might be named something else. Replace it with `[[Tome_of_Beasts_2.pdf]]` or however yours is named.

That's it! You should be able to see the page of the PDF embedded into the note.

