# CreateReactAppWithSass
Included is a zshell/bash shell script for creating a template workspace for building Progressive Web Apps (PWAs) using Facebook's React components with a SASS CSS pre-processor.

## Requirements
This script was written for execution in a linux environment, running on bash in a oh-my-zshell terminal. It may not work without zsh and bash as the if statements and syntax were designed for that combination specifically. Feel free to provide different versions for different terminal, operating system environments, and scripting languages.  

This program requires that you have Node.js and npm installed and working globally. For more info on getting those up and running on your system see their respective repositories/websites. 

## Usage
place CreateReactAppWithSass.sh in your projects folder. By running the command, a new project folder will be created with the same name as you give to the application.
```
bash CreateReactAppWithSass.sh sitename
```

This will create a new project folder called sitename/ which will be auto-populated with the directory structure and files needed to develop a React web application with SASS. From there you can
```
cd sitename
```

To create the first Sass-derived stylesheet, you'll need to create the style.css output file first. This is a Sass command and there are other ways to do it but this works. Open a new terminal window:
```
sass src/styles/scss/style.scss:src/styles/css/style.css
```

If everything worked a browser should have opened to http://localhost:3000 Navigate here to see the demo. 


### Notes and Recommendations
You may have to open src/index.js and comment out the serviceWorker lines during development
```
// import registerServiceWorker from './registerServiceWorker';
//registerServiceWorker();
```

Sass watch runs (like nodemon) and updates automatically on any file change save. While developing and making frequent updates have Sass watch running:
```
sass src/styles/scss/style.scss:src/styles/css/style.css --watch
```

to start editing the App.js file, add your own React components to the src/components/ directory, and make adjustments to the SASS styling in the src/scss/ directory. 

## Contact 
Feel free to send any commits, problems/bugs/issues, praise and beer money to ididnotknowicoulddothat[at]gmail.com

## Demo
To see a live demo visit https://usarneme-cra-sass.surge.sh/

Thanks!
