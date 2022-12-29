CI/CD is a popular solution in the application development industry. Today, we will discuss some points around this powerful tool. To be more clear, we will assume a project which is coded using Python.

Initially, the common steps in a CI setup are linting, testing, and building. When using Python, there are some specific tools for dealing with those steps accordingly.

For *linting*, we have **Pylint**, who keeps the coding standard as close to PEP8 as possible, and **Flake8**, who is also enforcing PEP8 style on codes but it works with PyFlakes, pycodestyle and McCabe.

For *testing*, we have many tools, but I personally recommend **Testify**. This tool was made to replace unittest and nose since it has more advanced features over unittest. Testify is also easy to learn and has quite a fame by being created with a Java-styled solution.

For *building*, there is the infamous **PyInstaller**.By using PyInstaller,the user do not need to install any Python interpreter or modules. The app can run normally because PyInstaller bundles it and all its dependencies into a single package. 

Additionally, we will talk about how to setup the CI. Two of the popular options for this step is GitHub Actions and Jenkins. I would like to introduce another useful service. It goes by the name GitLab CI/CD. This service helps user with cleaning the codes of bugs, making the early stage of the development cycle more stable.

Personally, I think GitLab CI/CD is better for a cloud-based environment. It is a cloud service, a tool of GitLab repository. It follow commits of the source code and act accordingly. As mentioned in https://docs.gitlab.com/ee/ci/cloud_services/index.html, GitLab CI/CD support OpenID Connect (OIDC) that allows your build and deployment job access to cloud credentials and services.
