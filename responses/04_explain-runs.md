## Runs

As you have learned `runs:` defines the command necessary to execute your Action.

In our current case `runs:` takes 2 arguments

- `using:`
- `main:`

These are specific to JavaScript Actions.  It is our way of telling the runner to run the `main.js` file using `node12`

This is no different than running a local JavaScript file using Node like you see below:
![node example](https://media.giphy.com/media/W1kCFFsaoYlsmpVtxv/giphy.gif)

Which means that the value of `main:` would be different if your file was not named `main.js`.  
![different filename example](https://media.giphy.com/media/H7CCHqH06pVbQeWmlb/giphy.gif)
In this scenario our metadata block would look like this:
```yaml
runs:
  using: 'node12'
  main: 'bread.js'
```

---

Keep this in mind because later we will be referencing a file that is not in the same directory of the `action.yml`