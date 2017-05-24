## Changelog
This changelog describes minor changes and updates for each release version.

### 5.01

* **Spell Checking Improvements**  
The spellchecker now only spell checks the active text that is on screen and a buffer area before and after the visible text. This improves editor performance on large documents as spell checks only affect a small portion of the entire document.

* **Support for Image Pasting**  
You can now paste images from the clipboard into Markdown content. Simply copy an image to the clipboard from your browser or image editing program, and then **ctrl-v** into the active markdown document at the location you want to embed the image.

* **PNG Image Compression**  
When pasting images into the editor or adding images by filename in the image dialog, images saved as PNG are automatically compressed using **optipng**. Image compression occurs in the background.

* **Scroll Sync**  
The HTML Preview now stays in sync with the editor's content in most situations. To move the preview simply navigate in the edit document and the preview will reflect the approximate location of the text with the editor selection showing in the top quarter of the preview.

* **Html PreviewWindow Setting Remembered between Restarts**  
The HTML Preview window setting is now remembered between restarts of the application. If you had the external preview open when you shut down, it will be opened when you start back up the next time.


### 5.0.230

* **Switch to HighlightJs for outputSyntax Coloring**  
We've switched to highlighJs for output syntax coloring on generated help and HTML content. Highlight is much smaller in size and doesn't require a number of workaround quirks to render properly.

* **External Preview more frequently**  
The preview now updates for all toolbar operations in addition to save operations. Previously only save forced an update. Especially useful when linking images and  links to immediately see added content.

* **Ctrl-Shift-Up/Ctrl-Shift-Down scrolls Preview Window**  
Added support to allow these keys to scroll the preview window up and down quickly with the keyboard.

* **Additional Preview Theme Tweaking**  
Fixed a number of sizing issues in the preview themes. Base size stays the same but large screen sizes now are a little more modest in their scale up size.

* **Fix Preview Timing**  
Updated the preview timing to allow for quicker and more reliable preview updates.

* **Preview Theme Updates**  
Many editor tweaks to improve performance and smoother typing while editing text.

### 5.0.225

* **Add Print media query for print output from Web pages**    
Added @media print to CSS to hide sidebar and a few other items from the print view.

* **Fix local CHM Links not loading**  
Fixed regression bug where local links in CHM file and from disk would not load properly. Now properly reloading topic from disk for local pages rather than loading AJAX

* **Fix Alt-K (Insert HyperLink) Keyboard jumping**  
Fixed bug where Ace Alt-K behavior of next selection was screwing up insertion of hyper links.

* **Fix Code Highlighting for various language Shortcuts (c#,vfp etc.)**  
Fixed bug that didn't run the language translation code when parsing languages to Ace language ids.

* **Fix .NET Import Bug with Generated Types**  
Fix .NET bug caused by generated anonymous types that don't have a proper name. Overriding code to use plain name property instead of FullName.

### 5.0.222
* **Add IE Edge Meta Tag to Layout page**  
Add IE Edge header to force latest version of IE to be used for rendering even in CHM file. Note there are still some issues in IE due to reporting invalid IE version (7.0) inside of the CHM viewer. Ace will have a fix in the next Ace-builds update.

* **Ctrl-Tab to switch between Edit and Preview Modes**    
Added ctrl-tab key combo to allow switching quickly between edit and browser views, or to completely reload the editor.

* **Fix Alt-V Preview Toggle**  
Fixed the reload of the preview window so it properly resets itself. Previously the preview window froze up at reloads. The preview now also remembers scroll position on same page reloads.

### 5.0.218
* **Major Overhaul of CHM and HHK Import Feature**  
Updated the import feature which can now import CHM or HHK files and create a new HelpBuilder project. Import is more reliable and auto-converts - as best as possible - HTML content into Markdown.

* **Switch Spell Checking Dictionaries**  
Switched spell checking dictionaries over to FireFox rather than Open Office ones.

* **Allow Adding new Words to Spell Dictionaries**  
You can now add new words to spelling dictionaries.

### 5.0.215 
* **Remove Unused Images Tool**  
Added new tool dialog that shows all images that are not referenced from your help topics. Images can optionally be removed in bulk to keep your project tidy. Only looks in then /images folder.

* **FTP Improvements: Single Topic and TOC Upload**   
Added support for uploading individual topics and table of contents in addition to uploading an entire project.