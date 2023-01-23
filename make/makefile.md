# `Makefile`

A `Makefile` is a way of automating software building procedure and complex tasks with dependencies. It consists mainly of **rules**. 

Dependency rule form: 
```
target: dependencies
    commands
```

Sample code:
```
clean:
    rm -rf *o
```
