# SonarQube on Scalingo

SonarQube is a tool to help you improve the ode quality and security. Deploy a SonarQube instance on the [Scalingo](https://scalingo.com) PaaS.

## One-Click Installation

[![Deploy to Scalingo](https://cdn.scalingo.com/deploy/button.svg)](https://my.scalingo.com/deploy)

## Install a SonarQube Plugin

You may want to install a SonarQube plugin. In such situation, fork this repository. Then copy the plugin JAR archive into the `plugins` folder. Commit the content of this repository, and push it to Scalingo. Your SonarQube instance will have the plugin installed.

# Update

To upgrade to the latest version you only need to redeploy it, this will retrieve the latest version avaible on [our Sonarqube buildpack](https://github.com/Scalingo/sonarqube-buildpack/).

`scalingo -a  my-app deploy https://github.com/Scalingo/sonarqube-scalingo/archive/refs/heads/master.tar.gz`
