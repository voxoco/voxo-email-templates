### Package contains

After purchase you downloaded a package with UI Kit. This package contains:

*   `images` directory with icons and pictures used in our templates
*   `emails` directory with templates. Every template has its own subdirectory with
    *   `assets` directory that contains images used only in this specific template
    *   `source.html` - not compiled HTML file
    *   `compiled.html` - HTML file ready to be send
    *   `screenshot.jpg` and `screenshot-mobile.jpg` - preview of this specific email
*   `gulpfile.js` scripts you can use to compile your own emails, based on our templates

### How to change template content

If you only want to change a text or image in an email, all you need to do is edit the file `compiled.html`. After changing image make sure to add it to assets folder.

Having a basic knowledge about html you can design an email of your own by using elements from different templates. In order to do it, follow the steps:

1.  Copy your desirable template folder which would be your basis. Paste it into emails folder and name it.
2.  Edit the file `source.html` by adding to it elements from different templates and save it.
3.  Compile a new template with Gulp. All you need to do is call the compiling script by giving a parameter name in which you will give the name of a newly created email `gulp compile --email $name`.
4.  Compilation will create a file `compiled.html` which is ready to be send.