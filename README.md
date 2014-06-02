phonegap-angular-tutorial
=========================

Setting up an Angular project in phonegap :)  Readers should have a knowledge of how to create an angular app using Yeoman.  If you don't know how to do this yet, don't worry... it's quite easy.  There are lots of tutorials, but here is one for you just in case: http://www.thinkster.io/angularjs/eqq96ECqkT/1-getting-your-project-set-up-with-yeoman

1)  Install phonegap via npm
``` html
sudo npm install -g phonegap
```
2) Create your iphone project inside the directory you want to store your project in.  Mine in this case is ~/dev/devmtn/teach/phonegap-angular-tutorial and create your phonegap project.  These parameters must be passed into the 'phonegap' command and are as follows $ phonegap create <directory> <identifier> <projectName>
```html
phonegap create tutorialApp com.johndangerstorey.tutorialApp Tutorial-App
```
3)Enter into your newly created 'tutorialApp' directory and create an IOS project for your App.  I'm using the following:
```html
cd tutorialApp/
phonegap build ios
```
4) Enter into the platforms/ios directory and test out the project to make sure everything is working correctly.  This next step is pretty janky... so if you are squimish it will probably be best to exit the tutorial now.  We'll be creating an angular app using yeoman and going from there, but we'll start with the install.  Make sure you npm yeoman:
```html
npm install -g yeoman
```
then go into your directory and create your app and pass in the following parameter: yo angular <appName>

```html
yo angular tutorialApp
```
5) Make sure you install things like grunt (npm install -g grunt-cli) so that you can build your app project on the web, then copy and paste the files from your yeoman generator into the www folder and/or platforms/ios/www folder.  Basically you will be building the core functionality in the main yeoman file then customizing the code for each platform respectively. Then using something like the Phonegap Developer App see your changes live and test via iphone: http://phonegap.com/blog/2014/04/23/phonegap-developer-app/

6) email me with questions: johndangerstorey@gmail.com
