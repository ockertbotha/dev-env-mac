# General Mac OS Settings

## Add User Language 

> Based on info from here adding Afrikaans: https://binary.coffee/blog/2016/10/14/afrikaans-on-a-mac.html

### 1. Clone LibreOffice/dictionaries
 -  https://github.com/LibreOffice/dictionaries

### 2. Copy dictionary files
 -  In cloned project go to ```/dictionaries/af_ZA/``` copy both ```af_ZA.aff``` and ```af_ZA.dic```
 - To ```~/Library/Spelling```, this is hidden by default and can be accesed in Finder by opening the ```Go``` menu while pressing the ```option``` key and selecting ```Library```, ```Spelling``` is now available as a sub-directory

 ### 3. Update System Preferences
 ### 3.1 Language & Region
 - Add Preferred language: ```+```, then select ```Afrikaans```
### 3.2 Keyboard
 - On ```Text``` tab under ```Spelling``` either select ```Afrikaans (Library)``` if you only want to use that, or select the last option ```Set Up...``` and configure the automatic detection order of precedence.

 >Having just set this up on Big Sur (April 2021), it works for spell checking when Afrikaans as the only language selected and the application being typed in is language aware, but results in no Touch Bar suggestions. It doesn't feel as good an experience as I'd hoped. Will update this if I find further info to improve things.