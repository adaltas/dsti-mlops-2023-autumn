
# Lab

Continuous testing

## Objectives

- Learn how to write and run unit tests for your functions
- Use test-driven development (TDD)

## Before starting

1. Create and activate virtual environment: `env_mlops`
2. In this virtual environment install `pytest`: `pip install pytest`
3. Set PYTHONPATH otherwise the modules will not be found [instructions](https://bic-berkeley.github.io/psych-214-fall-2016/using_pythonpath.html). This is a temporary setting and you need to do it each time you open the terminal.

```
$ export PYTHONPATH="$PWD/src"
$ echo $PYTHONPATH
```

## Lab context

Imagine you are developing an application, where users need to register. They need to fill in their get username, email and password.

Your job is to write the functions that will accept those parameters from the user input (in command line) and test if they follow the criteria:

- user name:
  - not empty
  - no spaces
- password:
  - at least 8 characters
  - at least one number
  - at least one letter
  - at least one special character
- email:
  - contains `@` and `.`

Run tests by running `pytest` in the terminal from the directory you defined as PWD before. If it doesn't work, try running `python -m pytest` instead.

Help yourself with the [pytest documentation](https://docs.pytest.org/en/7.0.x/getting-started.html).

If you finished, you can check out [what else you can do with pytest](https://towardsdatascience.com/pytest-with-marking-mocking-and-fixtures-in-10-minutes-678d7ccd2f70).

## Test-driven development (TDD)

Develop a function that will test if the input si a prime number. Use TDD to do that. Follow [this tutorial](https://stackabuse.com/test-driven-development-with-pytest/) if you need help.

## Troubleshooting

If you have problems running your tests:

1. Check that you read the tutorial correctly and that you reall followed the instruction.
2. Copy your error to browser (or describe it properly) and Google it. Since pytest is much used by the Python community, you have a big chance that somebody else already resolved the same issue.
3. When you open a link with a potential solution, don't just scroll through the page, but read. (Even if you don't understand it. You have to start somewhere.)
4. Try out the proposed solution.    
