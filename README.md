# camel-twitter-examproject (c) examproject

## What's this?
This project shows how to work with  
  Apache Camel Twitter  
  Spring MVC  
and how to configure.

## How to configure your twitter account?
First, you should read here. [Apache Camel Twitter](http://camel.apache.org/twitter.html)  
You will need a create an application for the Twitter. [Twitter Create an application](https://dev.twitter.com/apps/new)  

The configuration is required of your Twitter account.

    > cd { path to this README.md directory. }
    > cd src/main/webapp/WEB-INF/spring
    > notepad.exe camel-config.xml
    (*linux # vi camel-config.xml )
  
Please change to your account of the [change-this] of this descriptions.
    <to uri="twitter://timeline/user?consumerKey=change-this&amp;consumerSecret=change-this&amp;accessToken=change-this&amp;accessTokenSecret=change-this"/>

## How to build at the local?

You will need to get [Apache Maven](http://maven.apache.org/).

You will need to compile this project.
    > cd { path to this README.md directory. }
    > mvn compile
    > mvn install

## How to run at the local?

You will need to make the data directory.
    > cd { path to this README.md directory. }
    > mkdir data
    > cd data
    > mkdir inbox

To run the .war application by jetty plugin.
    > cd { path to this README.md directory. }
    > mvn jetty:run

A server be run on http://localhost:8081/

You can access to http://localhost:8081/ on your web browser.  
But, web browser access is not necessary in this case.

To stop the server hit ctrl + c  
The server must keep running!

## How to do to post for the Twitter?

You will need to make a text file, and write a message to Tweet on the text files.  
In the folder that appears below, and put a text file in, will be posted automatically.

    ${project-dir}/data/inbox

Put the text file in this folder.

## This project is hosted on GitHub.
https://github.com/hiroxpepe/camel-twitter-examproject

## Author
[hiroxpepe](hiroxpepe@gmail.com)

