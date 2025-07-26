## node-review

# What Happened When Running `npm start`

When I ran the command `npm start` in my terminal, Node.js looked for a script called `"start"` in My`package.json` file. This script tells Node.js what to do when I used `npm start`.

In My `package.json`, I have this section:

```json
"scripts": {
  "start": "node app.js"
}
```

This means that when I ran `npm start`, Node.js will try to run a file called `app.js` in My
project folder.

**If you got an error:**  
It probably means there is no file named `app.js` in your project directory. To fix this, you can either:

1. Create a file called `app.js` in your project folder, or
2. Change the `"start"` script in your `package.json` to point to the correct file you want to run.

**Summary:**  
- `npm start` looks for the `"start"` script in `package.json`.
- My script tries to run `app.js`.
- If `app.js` doesn’t exist, you’ll get an error.
- Make sure the file exists or update the script to match your main