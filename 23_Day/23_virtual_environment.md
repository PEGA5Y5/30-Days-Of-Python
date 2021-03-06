<div align="center">
  <h1> 30 Days Of Python: Day 23 - Virtual Environment </h1>
  <a class="header-badge" target="_blank" href="https://www.linkedin.com/in/asabeneh/">
  <img src="https://img.shields.io/badge/style--5eba00.svg?label=LinkedIn&logo=linkedin&style=social">
  </a>
  <a class="header-badge" target="_blank" href="https://twitter.com/Asabeneh">
  <img alt="Twitter Follow" src="https://img.shields.io/twitter/follow/asabeneh?style=social">
  </a>

  <sub>Author:
  <a href="https://www.linkedin.com/in/asabeneh/" target="_blank">Asabeneh Yetayeh</a><br>
  <small> First Edition: Nov 22 - Dec 22, 2019</small>
  </sub>
</div>
</div>

[<< Day 22](../22_Day/22_web_scraping.md) | [Day 24 >>](../24_Day/24_statistics.md)

![30DaysOfPython](../images/30DaysOfPython_banner3@2x.png)
- [📘 Day 23](#%f0%9f%93%98-day-23)
  - [Setting up Virtual Environments](#setting-up-virtual-environments)
  - [💻 Exercises: Day 23](#%f0%9f%92%bb-exercises-day-23)
# 📘 Day 23

## Setting up Virtual Environments

To start with project, it would be better to have a virtual environment. Virtual environment can help us to create an isolated or separate environment. This will help us to avoid conflicts in dependencies across projects. If you write pip freeze on your terminal you will see all the installed packages on your computer. If we use virtualenv, we will access only packages which are specific for that project. Open your terminal and install virtualenv

```sh
asabeneh@Asabeneh:~/Desktop/30DaysOfPython/flask_project$ pip install virtualenv
```

After installing the virtualenv package go to your project folder and create a virtual env by writing:
``sh
asabeneh@Asabeneh:~/Desktop/30DaysOfPython/flask_project\$ virtualenv venv

````
The venv name could another name too but I prefer to call it venv. Let's check if the the venv is create by using ls command.
```sh
asabeneh@Asabeneh:~/Desktop/30DaysOfPython/flask_project$ ls
venv/
````

Let's activate the virtual environment by writing the following command at our project folder.

```sh
asabeneh@Asabeneh:~/Desktop/30DaysOfPython/flask_project$ source venv/bin/activate

```

After you write the activation command, your project directory will start with venv. See the example below.

```sh
(venv) asabeneh@Asabeneh:~/Desktop/30DaysOfPython/flask_project$
```

Now, lets check the available package in this project by writing pip freeze. You will not see any package.

We are going to do a small flask project so let's install flask to this project.

```sh
(venv) asabeneh@Asabeneh:~/Desktop/30DaysOfPython/flask_project$ pip install Flask
```

Now, let's write pip freeze to see the install packages in the project

```sh
(venv) asabeneh@Asabeneh:~/Desktop/30DaysOfPython/flask_project$ pip freeze
Click==7.0
Flask==1.1.1
itsdangerous==1.1.0
Jinja2==2.10.3
MarkupSafe==1.1.1
Werkzeug==0.16.0
```

When you finish you should dactivate active project using _deactivate_.

```sh
(venv) asabeneh@Asabeneh:~/Desktop/30DaysOfPython$ deactivate
```

The necessary modules to work on flask are installed. Now, you project directory is ready for flask project. You should include the venv to your .gitignore file not to push it to github.

## 💻 Exercises: Day 23
1. Create a project directory with a virtual environment based on the example give above.


🎉 CONGRATULATIONS ! 🎉
[<< Day 22](../22_Day/22_web_scraping.md) | [Day 24 >>](../24_Day/24_statistics.md)
