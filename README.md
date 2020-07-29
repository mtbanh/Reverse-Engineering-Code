# Reverse-Engineering-Code

## About

This application is empowered, by using a middleware 'passport' npm package, with the ability to create a new user with the specific email and password. This instance of the user is saved in the database, and can be accessed when the user log-in with the same credentials. If any of the credentials does not match, the user is unable to log-in.

The tutorial below is to explain how the features seen in the deployed application was created and implemented. It is meant to be a high-level overview; for more specifics, please open the source files and there will be line-by-line comment explaining how and why the code works.

---

## Live Site

![Deployed Application](assets\deployed-site.gif)

---


## Getting started
Below are the prerequisite understanding and programs that were utilized :
* Visual Studio Code-click [here](https://code.visualstudio.com/) to a tutorial to install
* Github repository-click [here](https://help.github.com/en/github/)
* node.js and its file system [here](https://nodejs.org/en/)
* bcrypt.js [here](https://www.npmjs.com/package/bycrypt)
* express and express-session [here](https://www.npmjs.com/package/express)
* mysql2 [here](https://www.npmjs.com/package/mysql2)
* passport and passport-local [here](https://www.npmjs.com/package/passport)
* sequelize [here](https://www.npmjs.com/package/sequelize)

---

## Code spotlight

The code snippet below demonstrate how to create a synchronous call of function that will also generate role-specific questions by evaluating what the provided 'role' is. This function will also continue to perform this set of work as long as the user want to continue to add employees.
```js
{

    async function generateProfile(){
    try {
        let wantsToCont = true;
        while (wantsToCont){
            const employeeProfile = await promptQs();
            const {name, id, email, role} = employeeProfile;
            console.log(employeeProfile);

            switch(role){
}

```
---



## Deployed link

[Live site](https://mtbanh.github.io/Template-Engine)


---

## Author

**Mai Banh**
- [Link to Github](https://github.com/mtbanh)
- [Link to LinkedIn](https://www.linkedin.com/in/mai-banh-311ba6164/)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## Acknowledgments
Thank you to my tutor, Matthew Chen.