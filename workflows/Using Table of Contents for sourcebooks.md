
## Description

This workflow lets you do the following things:
- search for PDFs by category
- click on a link in the Table of Contents note to open the PDF to the relevant page

## Plugins used

- Dataview
- Templater


> [!warning] You need to have purchased the relevant PDFs
> This workflow facilitates the organizing and finding part of PDFs; it doesn't give you access to the PDFs themselves. You'll still need to have purchased the PDFs of the sourcebooks mentioned. I do not condone piracy.

### Zotero

This workflow also requires another app that lets you link to pages of PDFs. Choose one of the following or similar:
- [Zotero](https://zotero.org) - my recommendation, and the app I refer to in the instructions below
	- You'll also need to download and install the following Zotero plugins:
		- [Zotero folder import](https://github.com/retorquere/zotero-folder-import)
		- [Zutilo](https://github.com/wshanks/Zutilo)
- [Skim](https://skim-app.sourceforge.io/) (macOS only)
- [DevonThink](https://www.devontechnologies.com/apps/devonthink)


## Instructions

1. In Zotero, go to Tools > Zutilo Preferences.
2. In the Interface tab, scroll down to `Copy select item links` and toggle the radio button for it that is marked *Zotero context menu*. Optionally, assign a shortcut to the same thing in the Shortcuts tab as well.
3. In Obsidian, choose a book from the `sources` folder that I have Table of Contents for and that you also have the PDF for. Check [[List of Sources]] for a list of all the sources in this vault.
4. Find the PDF in Zotero. Right click on it and select `Copy select item links`. You should have something that looks like this: `zotero://select/library/items/NJW6TEUI`. In this case, `NJW6TEUI` is your Zotero ID for this PDF.
5. In Obsidian, open up the note of the source in question. For example, [[Secrets of Magic]].
6. Copy the ID in the `[Source]` link. For example, if the link points to `zotero://select/library/items/3LHL67ZM`, the ID is `3LHL67ZM`.
7. Open up the Command Pane (`CMD/CTRL+P`) and select `Global Search and Replace: Search and Replace in all files`. In the *Search* field, enter the ID from the Obsidian note (i.e., `3LHL67ZM`). In the *Replace* field, enter YOUR Zotero ID (i.e. `NJW6TEUI` from Step 4.) Hit ENTER to replace everything in all files.
8. Give it a go by clicking on one of the `Source` links in [[Secrets of Magic]]. The relevant PDF should be opened to the right page!
