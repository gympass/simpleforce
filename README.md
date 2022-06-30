# simpleforce

Forked from [github.com/simpleforce/simpleforce](https://github.com/simpleforce/simpleforce)

## Changes

- Now the Create function returns the error
	```golang
	cs, err := client.SObject("Case").                       	// Create an empty object of type "Case"
			Set("Subject", "Case created by simpleforce").     	// Set the "Subject" field.
			Set("Comments", "Case commented by simpleforce").  	// Set the "Comments" field.
			Create() 											// Create the record on Salesforce server.
	```