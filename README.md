
# cra-template-brandsite
This project is a cra-template-based website template to 
quickly setup a personal, non-profit, or company website.

## To use this template to build your site
1. Create an empty directory and CD into it
2. Run "npx create-cra-template-app <app name> --template brandsite" 
3. Run npm install
4. Customize site as described below
5. Run npm start

### To customize the site
1. Open the code in Visual Studio Code. 
Find and update all instances of [%REPLACE%]
2. Change any of the stock images you want to change. 
Replace text in post1.html, post2.html, and post3.html
3. Change the video links in Portfolio.js page


### To add a new blog post
1. Create a html with a unique name in all lowercase in posts folder. 
Copy over or create the html of the content. LinkedIn is a great service 
to use to author drafts. https://html-online.com/editor/ is good editor for html creation
2. Take care with the case of html file being created. It should match 
the case of the "name" attribute in articleindex.js in next step.
3. Add an entry in articleIndex.js. Once again, the jpg file should 
match the exact case of the file name on disk and the name attribute 
should match the case of the html file name (without extension) created in step 2.
4. Any embedded image link should be a publicly available URL
5. Use div with className=quote for quotes
6. If you want a header image served with the content, add the image 
with the same name as the html file to the images folder, and refer to it in articleIndex.js file

## Starting the application

In the directory created by the template <app name>, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### To test the application
Note that the test suites need enzyme. Before running tests:

Add the following lines to package.json file in the 
app directory <app name> created by the template:
```  
  "devDependencies": {
    "enzyme": "^3.11.0",
    "enzyme-adapter-react-16": "^1.15.2"
  }
```

Then run:
  `npm install`
  `npm start`
  
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

