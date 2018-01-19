namebench 2.0
=============
namebench provides personalized DNS server recommendations based on your
browsing history.

WARNING: This tool is in the midst of a major rewrite. The "master" branch is currently in experimental
form and currently lacks a user interface, nor does it support any command-line options.

BUILDING:
=========
Building requires Go 1.2 to be installed: http://golang.org/

* Create a workspace directory, and cd into it.
* Prepare your workspace directory:

```
    go get -u github.com/forrest321/namebench
```

* Build it.

```
    cd src/github.com/forrest321/namebench
    go build namebench.go
```

You should have an executable named 'namebench' in the current directory.


RUNNING:
========
* End-user: run ./namebench, which should open up a UI window.
* Developer, run ./namebench_dev_server.sh for an auto-reloading webserver at http://localhost:9080/

NOTES:
========
* made a copy of a copy of publicsuffix due to name mangling from code.google.com shennanigans
* updated code to handle expected 3 params, discarding the new third. 
* probably need to check that third param and reduce code elsewhere -fo

