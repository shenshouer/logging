# logging

## Usage:

for base package

	package base

	import (
		"github.com/shenshouer/logging"
	)


	func NewLogger() logging.Logger {
		return logging.NewSimpleLogger()
	}

for other package you want to use:

	var logger *logging.Logger = base.NewLogger()


the method for logger to use like fmt.Print、fmt.Println、fmt.Printf

for example :

	logger.Info("")
	
	logger.Infoln("")

	logger.Infof("%s", "test")

the same to the Error、Warn