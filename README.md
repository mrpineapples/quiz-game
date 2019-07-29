# quiz-game
Math quiz written in Go

To use the math quiz:

```bash
go get github.com/mrpineapples/quiz-game
cd $GOPATH/src/github.com/mrpineapples/quiz-game
go run main.go
```

**If you opt not to use `go get` you can just clone the repo anywhere on your machine and just run that last line in that directory**

Feel free to change the problems in the csv or create your own custom file and use it with the `csv` flag shown below

## Options
You can pass in a number (seconds) to the limit flag which will set a timer for the quiz:
```
go run main.go -limit=5
```
**The default time limit is 20 seconds if one isn't passed**

In the same directory, you can create a `.csv` file with your own math problems and use it with the csv flag like so:
```
go run main.go -csv=[csvFilename].csv
```
**The csv flag defaults to problems.csv if one isn't passed**

Both flags can be combined to perform something like this:
```
go run main.go -csv=custom.csv -limit=10
```
