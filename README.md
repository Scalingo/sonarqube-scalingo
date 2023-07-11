# SonarQube on Scalingo

SonarQube is SonarQube is a tool for continuously inspecting the Code Quality
and Security of your codebases, and guiding development teams during Code
Reviews.

## One-Click Installation

[![Deploy to Scalingo](https://cdn.scalingo.com/deploy/button.svg)](https://dashboard.scalingo.com/create/app?source=https://github.com/Scalingo/scalingo-sonarqube)

> :warning: SonarQube requires quite a lot of RAM to run properly. **We
strongly recommend to use at least one 2XL container for your SonarQube
setup.**

> :information_source: The default credentials to log on SonarQube are:
> - Username: `admin`
> - Password: `admin`

## Installing a SonarQube Plugin

To install a SonarQube plugin, please:
1. Fork this repository
2. Copy the plugin JAR archive into the `plugins` folder of your forked
   repository
3. Commit the content of your repo
4. Push your updated repo to Scalingo
5. The new deployment triggered by the push will take the plugin into account.

## Updating SonarQube

To update an existing SonarQube setup, you only need to redeploy it. The new
deployment will retrieve the latest version available in
[our Sonarqube buildpack](https://github.com/Scalingo/sonarqube-buildpack/).

From the Command Line Interface:

```bash
scalingo --app my-app deploy https://github.com/Scalingo/scalingo-sonarqube/archive/refs/heads/master.tar.gz`
```
