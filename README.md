### What I've learned
- learned how to use __go module__ with __go get__ as a package manager
- learned how to release __go module__ and best practice for versioning

### Commands
Initialize module. (In this case I use github as a module registry)
```
go mod init github.com/<username>/<repository>
```


Install module
```
go get github.com/<username>/<repository>
```


Install module with specific version
```
go get github.com/<username>/<repository>@vx.x.x
```


Like this...
```
go get github.com/kaisukez/go-module-practice/v2@v2.1.0
```


List all existing dependent modules
```
go list -m all
```


[Install all modules in go.mod file](https://stackoverflow.com/questions/52266332/manually-fetch-dependencies-from-go-mod)
```
go mod download
```


Clear all unused dependent modules
```
go mod tidy
```


### Quote
`
Sometimes, maintaining backwards compatibility can lead to awkward APIs. That's OK. An imperfect API is better than breaking users' existing code.
`

### References
- https://blog.golang.org/using-go-modules
- https://blog.golang.org/publishing-go-modules
- https://blog.golang.org/v2-go-modules
