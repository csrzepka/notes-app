# Notes-App

Notes-App is a Node.js terminal application to read and write notes.

This is a terminal based application, developed through the [The Complete Node.js Developer Course (3rd Edition)](https://www.udemy.com/course/the-complete-nodejs-developer-course-2/), as the first of three Node applications. At the current state of the application, I have not made any significant changes, and this is just my written copy of the app made in the course.

The [The Complete Node.js Developer Course (3rd Edition)](https://www.udemy.com/course/the-complete-nodejs-developer-course-2/) is taught by [Andrew Mead](https://twitter.com/andrew_j_mead) and [Rob Percival](https://twitter.com/techedrob) and deserve credit for creating the course and application from where this comes from.

## Installation

To set up this project, download or clone the repository. Once that is finished, open the containing folder in the command line or terminal and run
```
npm i
``` 
to install the required node modules for the project.

## Commands

```
node app.js add --title="some string title" --body="some string body"
```

To create a new note, you can use the `add` command. This requires two arguments to run, **Title** and **Body**.

**Title**: The title to save the note under. This has to be unique and cannot be the same as any other note already saved.

**Body**: The body of the note, where all of the contents will be stored.

```
node app.js remove --title="some string title"
```

The `remove` command will delete any note with the specified **Title**.

**Title**: Title of the note to be deleted.


```
node app.js list
```

The `list` command will list out the title of all notes created with this application. 

```
node app.js read --title="some string title"
```

The `read` command will let you read the body of a saved note by entering the **Title** of the note.

**Title**: Title of the note to be read.

## Storage

The notes created by this application are stored in a JSON file created by the application, called `notes.json`. 

