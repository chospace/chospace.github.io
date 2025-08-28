---
title: "Exploring Filesystem in Golang"
date: 2019-03-06T21:37:39+07:00
# weight: 1
# aliases: ["/first"]
tags: ["golang"]
author: "Cho"
summary: "test note"
# author: ["Me", "You"] # multiple authors
showToc: false
TocOpen: false
draft: false
hidemeta: false
comments: false
#description: "Desc Text."
canonicalURL: "https://canonical.url/to/page"
disableHLJS: false # to disable highlightjs set true
disableShare: false
hideSummary: false
searchHidden: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: true
cover:
  image: "<image path/url>" # image path/url
  alt: "<alt text>" # alt text
  caption: "<text>" # display caption under cover
  relative: false # when using page bundles set this to true
  hidden: true # only hide on current single page
editPost:
  URL: "https://github.com/chospace/chospace.github.io/content"
  Text: "Suggest Changes" # edit text
  appendFilePath: true # to append file path to Edit link
---

I am currently dabbling in [GoLang](https://golang.org/) and trying to get familiar with its syntax and style of programming. I also want to get familiar with the built-in packages for basic tasks without having to google for basic features.

In this post I will be working my way up to building a simple program that can list the files of a given path to it as a command line argument.

---

## 1. Print to console

Let’s start with a simple program that can print a statement to the console using the `"fmt"` package and the `"Println()"` function.

```go
package main

import (
	"fmt"
)

func main() {
    fmt.Println("Welcome to Go!")
}

#=> Welcome to Go!
```
## 2. Read arguments from command line

Now, let’s learn to read the command line arguments to the program using the `"os"` package and the Args variable that stores them as an array of strings starting with the program name as the first element.

```go
package main

import (
	"fmt"
	"os"
)

func main() {
	if len(os.Args) > 1 {
		fmt.Println("Arguments:", os.Args[1])
	} else {
		fmt.Println("No Arguments provided")
	}
}
#=> Apurvas-MacBook-Pro:OSManipulation apurva$ go run CommandLineArgs.go Hello
Arguments: Hello

#=> Apurvas-MacBook-Pro:OSManipulation apurva$ go run CommandLineArgs.go
No Arguments provided
```

## 3. Traversing the listings of a path

Finally, we need to be able to discover all the file/directory listings for a given path passed as a command line argument.

This can be conveniently achieved using the ReadDir() function of the "io/ioutil" package.

```go
package main

import (
	"fmt"
	"io/ioutil"
	"os"
)

func main() {
	var files []os.FileInfo
	var err error
	if len(os.Args) > 1 {
		files, err = ioutil.ReadDir(os.Args[1])
	} else {
		files, err = ioutil.ReadDir(".")
	}

	if err != nil {
		fmt.Println("Err ", err)
	}
	for _, file := range files {
		fmt.Print(file.Mode())
		fmt.Print(" ", file.Size())
		fmt.Print(" ", file.Name())
		fmt.Println()
	}
}
```
🤓 Exploring further into `"fmt"`, `"os"`, `"io/ioutil"` to recreate an implementation of the `"ls"` unix utility is left as an exercise for the reader.
