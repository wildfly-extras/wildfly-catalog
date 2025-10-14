Contributing to the WildFly Catalog
==================================

Welcome to the WildFly Catalogproject! We welcome contributions from the community. 
This guide will walk you through the steps for getting started on our project.

- [Forking the Project](#forking-the-project)
- [Issues](#issues)
- [Setting up your Developer Environment](#setting-up-your-developer-environment)
- [Contributing Guidelines](#contributing-guidelines)


## Forking the Project 
To contribute, you will first need to fork the [wildfly-catalog](https://github.com/wildfly-extras/wildfly-catalog) repository. 

This can be done by looking in the top-right corner of the repository page and clicking "Fork".

The next step is to clone your newly forked repository onto your local workspace. 
This can be done by going to your newly forked repository, which should be at `https://github.com/USERNAME/wildfly-catalog`. 

Then, there will be a green button that says "Code". Click on that and copy the URL.

Then, in your terminal, paste the following command:
```bash
git clone [URL]
```
Be sure to replace [URL] with the URL that you copied.

Now you have the repository on your computer!

## Issues
This project uses Github Issues to manage issues. All issues can be found [here](https://github.com/wildfly-extras/wildfly-catalog/issues). 

## Setting up your Developer Environment
You will need:

* JDK 17
* Git
* Maven 3.3.9 or later
* An [IDE](https://en.wikipedia.org/wiki/Comparison_of_integrated_development_environments#Java)
(e.g., [IntelliJ IDEA](https://www.jetbrains.com/idea/download/), [Eclipse](https://www.eclipse.org/downloads/), etc.)

First `cd` to the directory where you cloned the project (eg: `cd wildfly-catalog`)

Add a remote ref to upstream, for pulling future updates.
For example:

```
git remote add upstream https://github.com/wildfly-extras/wildfly-catalog
```
To build `wildfly-catalog` run:
```bash
cd catalog-generator
mvn clean install
```

## Contributing Guidelines

When submitting a PR, please keep the following guidelines in mind:

1. In general, it's good practice to squash all of your commits into a single commit. For larger changes, it's ok to have multiple meaningful commits. If you need help with squashing your commits, feel free to ask us how to do this on your pull request. We're more than happy to help!

2. Please include the GitHub issue you worked on in the title of your pull request and in your commit message. 

3. Please include the link to the GitHub issue you worked on in the description of the pull request.
