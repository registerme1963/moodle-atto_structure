MarvinJS atto plugin (atto_structure) for Moodle.
Alows users to create chemical structures and reactions then easily
insert image into Moodle.

Quick Installation
1) Download and install MarvinJS from www.chemaxon.com.
2) Place the structure folder in your lib/editor/atto/plugins folder.
3) Proceed to the notifications section of the admin panel.
4) Confirm installation of moodle-atto_structure
5) Set the path to MarvinJS in the settings page that appears 
   or proceed to admin setting for this filter and set path).
6) Proceed to Site administration > Plugins > Text editors > Atto HTML 
   editor > Atto toolbar settings and add the new plugin to the tool bar
   config, by adding "structure" at the end of one of the rows of buttons.


By Axel Schorcht Thu, Apr 8, 2021, 6:26 PM posted https://moodle.org/plugins/atto_structure comments:
Hi for all of you trying to get this plugin to work on a current version of moodle and marvinjs:
1. Download the zip and extract
2. to resolve the mixed content error (https->http) replace in structure\lib.php line 57 "http://" with "https://"
3. the name of the marvin scripts are hardcoded, so in order to make the newest version (1.0.0) work replace in the following documents promise-0.1.1.min.js with promise-1.0.0.min.js
structure\yui\build\moodle-atto_structure-button\moodle-atto_structure-button-debug.js - line 218
structure\yui\build\moodle-atto_structure-button\moodle-atto_structure-button-min.js - line 1
structure\yui\build\moodle-atto_structure-button\moodle-atto_structure-button.js - line 215
structure\yui\src\button\js\button.js - line 216
4. re-zip the files and install
5. enjoy!
