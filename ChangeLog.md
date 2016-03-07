## Changelog
This changelog describes minor changes and updates for each release version.

### 5.0.224

* **Add Print media query for print output from Web pages**    
Added @media print to CSS to hide sidebar and a few other items from the print view.

* **Fix local CHM Links not loading**  
Fixed regression bug where local links in CHM file and from disk would not load properly. Now properly reloading topic from disk for local pages rather than loading AJAX

* **Fix Alt-K (Insert HyperLink) Keyboard jumping**  
Fixed bug where Ace Alt-K behavior of next selection was screwing up insertion of hyper links.

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