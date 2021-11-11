<h4> 👋 Hello, I'm Anisul Islam </h4>

A full time content creator on & web developer

<!-- Contact me section starts here  -->

[<img align="left" alt="website" title="website" width="45" hspace="5" src="./images/website.svg" />][website]
[<img align="left" alt="youtube" title="youtube link" width="45" hspace="5" src="./images/youtube.svg" />][youtube]
[<img align="left" alt="facebook" title="facebook" width="45" hspace="5" src="./images/facebook.svg" />][facebook]
[<img align="left" alt="linkedin" title="linkedin" width="45" hspace="5" src="./images/linkedin.svg" />][linkedin]
<br />
<br />
<br />

<!-- Contact me section ends here  -->

# ESLint

### 1. What is ESLint?

- A linter - tool for identifying and reporting programmatic, stylistic errors.
- ESLint does static error checking before running the program

### 2. Example of Popular Linters

- [JSLint](https://www.jslint.com/)
- [ESLint](https://eslint.org/)
- [JSHint](https://jshint.com/)

### 3. Prerequisities for setting up ESLint

- install Node.js
- install VSCode (as we will use VSCode)

### 4. Installing & using ESLint

1. Create package.json: `npm init`
2. Install eslint as dev dependency: `npm install eslint --save-dev `
3. Initialize eslint: `eslint --init` and follow steps:

   - How would you like to use ESLint? To check syntax and find problems
   - How would you like to use ESLint? None of these
   - How would you like to use ESLint? None of these
   - Does your project use TypeScript? › No
   - Where does your code run? Browser

4. Go to `.eslintrc.json` file and make add your necessary adjustments
   Example

   ```json

   following codes will activate the recommended rules which can be changed inside the rules object.
     {
      "extends": "eslint:recommended"
     }

    <!-- first value is error level, it can have 3 values: off/0, warn/1, error/2 -->
    Example of ESLint rules
    "rules": {
        "quotes": ["error", "double"]
    }

    More Examples of ESLint rules
   "rules": {
       "no-var": "error",
       "eqeqeq": "error",
       "no-unused-vars": "error",
       "default-case": "error",
       "no-console": "error",
       "camelcase": "error",
       "consistent-return": "error",
       "func-style": "error",
       "max-depth": ["error", 2],
       "max-lines": ["error", 25],
       "prefer-arrow-callback": "error",
       "prefer-const": "error",
       "no-useless-return": "error",
       "no-plusplus": "error",
       "quotes": ["error", "single"]
     }

   ```

5. add some codes in a js file for testing the eslint. I have created a file called app.js and added the following codes for testing purpose

   ```javascript
   var username = "anisul Islam";
   var password = "12345";
   var occupation = "full stack web developer";
   const user_presentaddress = "lala";

   var a = 6;
   a++;

   console.log(occupation);

   const validateUser = (pwd) => {
     if (password == pwd) {
       return true;
     }
   };

   console.log(validateUser(12345));

   switch (foo) {
     case 1:
       console.log(foo);
       break;

     case 2:
       console.log(foo);
       break;
   }

   const foo = true;
   if (foo) {
     if (foo) {
       if (foo) {
         console.log("hi");
       }
       console.log("hi");
     }
     console.log("hi");
   }

   setTimeout(function () {}, 1000);
   ```

6. make some changes in setting.json

   format on save and fix errors: add the following codes in settings.json

   ```
    "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
    },
    "eslint.validate": ["javascript"]
   ```

7. Run the eslint: `eslint fileName.js` and check the erros
8. Fix automatically fixable errors: `eslint fileName.js --fix`

---

### Thanks for reading this ESLint documentation.

---

<!-- Links section starts here -->

[website]: http://www.studywithanis.com/
[youtube]: https://www.youtube.com/c/anisulislamrubel
[facebook]: https://www.facebook.com/studywithanis/
[linkedin]: https://www.linkedin.com/in/anisul2020/
[github]: https://github.com/anisul-Islam
