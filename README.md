# Merge CSV
It is a Go implementation for merging csv files

## Install
You can install mergecsv using Go's built-in package manager, go get:
``` 
go get github.com/DanielFillol/mergecsv 
```
## Usage
Here's a simple example of how to use mergecsv:
```go
package main

import (
	"github.com/DanielFillol/mergecsv"
	"log"
)

const (
	filePath      = "YOUR_FILES_FOLDER"
	mergeFileName = "MERGED_FILE_NAME"
)

func main() {
	err := mergecsv.Merge(filePath, mergeFileName)
	if err != nil {
		log.Println(err)
	}
}
```
