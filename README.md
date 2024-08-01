# Chef

Chef is a configuration management tool. Configuration means we have to configure our system by installing OS like Ubuntu, Linux, CentOS, and Windows, and other packages and services like Apache, Nginx, and Tomcat which are web servers. It's written in Ruby and Erlang and was developed by Adam Jacob in 2009. It’s a pull-based tool like Puppet. It’s an operational tool and is open source.

## Infrastructure as Code (IAC)

Infrastructure as Code is a very important term used in DevOps that means we create/build infrastructure through code.

## Chef Architecture

We have a Chef Workstation on which we write our code. After this, we save this code on the Chef Server and then through Knife we run it on our machines where we want to do configuration. Ohai is a very important component that has all the information of that machine which we want to configure.

## How We Work in Chef Tool

After installing Chef, we will create a cookbooks directory through:

```bash
mkdir cookbooks

After creating cookbooks directory through #cd cookbooks we are now in our cookbooks directory

Here we will create a cookbook through cli through command
#chef generate cookbook <cookbook name>

After creating cookbook we will create a recipe 
#chef generate recipe <recipe name>

Recipe will be in ruby language that you don’t worry if you are not familiar with Ruby just understand its syntax and then after you can find different configuration files in chef market just change a little bit according to your need and configure your machine accordingly.

Then you have to come in cookbooks dir where you can write code in Ruby
