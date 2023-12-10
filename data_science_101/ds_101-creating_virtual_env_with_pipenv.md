# Data Science 101 - Creating a virtual environment with pipenv

*This tutorial belongs to a set of tutorials intended to help other data professionals and our study group.*

**Why?**

As said in our previous tutorial, a virtual environment is one of the pillars of good development, because it helps to avoid the "it works in my machine" problem by listing all dependencies needed to run or develop the application. Later, we built the virtual environment using the python submodule venv. Therefore, this time we will use the pipenv library.

**But why pipenv?**

Pipenv helps us with the following:

- its virtual environment manager can even set the python version;
- it adds each new non-transitive dependency in the pipfile (as it calls your "requirements.txt" file); and
- it adds a Pipfile.lock which ensures the right library will be installed because it generates a hash number for each library.

**How to use?**

As pipenv is a third-party library, we need install it beforehand in our global python installation:

```bash
pip install pipenv
```

Just to remember, if you want to install in your user's installation:

```bash
pip install pipenv --user
```

By default, pipenv creates its virtual environments in his installation folder, but I prefer to create a *.venv* folder within the project folder. For enabling this, you must add a new environment variable called PIPENV_VENV_IN_PROJECT and set it to 1. This addition will depends on your OS.

If you are using Windows, go to "initiate" button and type "environment variables", select and click on "user environment variables". A window like Figure 1 will be showed.

![Enviroment variables for user](https://github.com/cafe-com-analytics/cafe-com-analytics/blob/main/assets/images/text_02_figure_01.png)

Figure 1 - Enviroment variables for user.

Click on "New". Write "PIPENV_VENV_IN_PROJECT" on the variable side and "1" (without parentheses) in the value side.

Now, you are good to go. Your pipenv is installed and set.

Try to build a virtual environment in a new project:

```bash
pipenv install pandas
```

You will se that the folder .venv will appear in the root of your project, besides, two other files will appear: a Pipfile and a Pipfile.lock. They hold the dependecies.

That's it. =)

---

## References:

1. [Pipenv](https://pipenv.pypa.io/en/latest/)
