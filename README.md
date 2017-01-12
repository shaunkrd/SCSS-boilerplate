# hanover digital : SCSS Boilerplate #

This repo can be used as a starting point for any Sass/SCSS Compass project.

### Installation ###

1. Open Terminal and navigate to the site project directory.

2. Paste in the following (replacing username and password with the Bitbucket connection details) and click enter:

            git clone https://username:password@bitbucket.org/hanoverdigital/hd-boilerplate-scss.git

3. This will create a directory named 'hd-boilerplate-scss' - check that it contains a 'config.rb' file and a populated 'src/scss' directory

4. Move the contents of the 'hd-boilerplate-scss' directory (there is no need to copy the '.git' directory or the 'README.md' file) into wherever the SCSS needs to be, perhaps the WordPress custom theme directory or the project's web root directory

5. Delete the now not needed 'hd-boilerplate-scss' directory

6. For the project specific SCSS and variables, create a directory inside 'src/scss' named 'project', and a directory within 'project' named 'templates' for the template specific SCSS

7. Now you need to install the node elements in order to be able to use Grunt to compile the CSS and the Javascript. Firstly, open Terminal and navigate to theme directory

8. Run the following command which will create a directory named 'node_modules' (500MB approx) with content dependent on the dependencies defined in the package.json. It might take 20 to 30 minutes for the process to complete:

            npm install

9. You can check the installed packages and their versions by running the command:

            npm list --depth=0

10. You can check for and apply any updated versions of the packages by just running the command (it is sometimes necessary to run the command more than once for it to find and update versions):

            updtr

11. If the command doesn't work then you'll need to install the package which you can do with:

            sudo npm install -g updtr

12. Now to enable the grunt commands (eg grunt watch, 'grunt grunticon') via terminal run the command:

            sudo npm install -g grunt-cli