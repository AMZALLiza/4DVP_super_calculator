# Simple calculator

This is a simple calculator made in go !

It supports :

- division
- multiplication
- addition
- subtraction

## Implementation of DevOps in Super Calculator

To implement DevOps philosophy in this project, you need to : 

- create Docker Hub account
- create github account 

To run Workflows, you need : 
- create .github/workflows folder in your project.

To create Docker images and build your project with docker you need :
- create a repository in your Docker Hub.
- generate an access token to authenticate you to the Docker Hub.
- add the access token that docker generated to you in your github project ( settings - secrets and variables - actions)
- create workflows and push it to the github repository and see the result in actions. 

Github Repository : ```
https://github.com/AMZALLiza/4DVP_super_calculator.git ```


## Usage example

```text
This is a simple calculator application.
It supports Addition, Subtraction, Division, Multiplication.
Specify the numbers to use with --x or --y.
Default values for x and y are 0.

Usage:
  calculator [command]

Available Commands:
  add         Addition of x and y
  completion  Generate the autocompletion script for the specified shell
  div         Division of x and y
  help        Help about any command
  mul         Multiplication of x and y
  sub         Subtraction of x and y

Flags:
  -h, --help     help for calculator
  -t, --toggle   Help message for toggle

Use "calculator [command] --help" for more information about a command.
```

## Example usage

### Addition

```bash
./calculator add --x 5 4
4.000000 + 5.000000 = 9.000000
```

### Subtraction

```bash
./calculator sub --x 5 4
4.000000 - 5.000000 = -1.000000
```

### Multiplication

```bash
./calculator mul --x 5 4
4.000000 * 5.000000 = 20.000000
```

### Division

```bash
./calculator div --x 5 4
4.000000 / 5.000000 = 0.800000
```

## Test execution

This application uses the default go test integration.

```text
> go test ./...
?       calculator                  [no test files]
?       calculator/cmd              [no test files]
ok      calculator/internals/math   0.002s
```