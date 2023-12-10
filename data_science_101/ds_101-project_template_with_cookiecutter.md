# Data Science 101 - Project template with cookiecutter

*This tutorial belongs to a set of tutorials intended to help other data professionals and our study group.*

**Why?**

There are a few minor grammar errors in the text. Here is a corrected version:

One of the critical aspects of a successful project is communication. Standardization of folder structure works as communication within a technical team. Just like lean strategies in factories, knowing where your supplies and tools are stored can save a lot of time. Therefore, I summarize the benefits of Cookiecutter as:
> 1. It decreases the time spent in creating the project's structure;
> 2. It increases and reinforces the chosen structure and some configurations of a team.

One library that I use to help build the initial folder structure in projects that I am working on is [Cookiecutter](https://www.cookiecutter.io/). According to its documentation, "Cookiecutter is an open-source library for building coding project templates".

**How to use?**

Firstly, you will need to install Cookiecutter in your environment. As you will probably use this for several projects, I recommend installing it in you global environment.

```bash
pip install cookiecutter
```

Cookiecutter just reproduces a folder's structure from a chosen template. In its [documentation](https://www.cookiecutter.io/templates), you will find a lot of templates. As I work as a data scientist, I would recommend the [Cookiecutter Data Science](https://drivendata.github.io/cookiecutter-data-science/) made by the [Drivendata team](https://www.drivendata.org/).

So, the second step is to create your project using a template.

```bash
cookiecutter <template-of-your-choice>
```

E.g. using [Cookiecutter Data Science](https://drivendata.github.io/cookiecutter-data-science/):

```bash
cookiecutter -c v1 https://github.com/drivendata/cookiecutter-data-science
```

A series of questions will appear to help you customize your initial project.

That's it. =)

---

