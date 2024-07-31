# Chef Recipe for Apache server

This repository contains a Chef recipe to install and configure the `httpd` service along with creating specific files.

## Chef Recipe Content

The following Chef recipe performs the following tasks:
1. Creates a file `/home/ec2-user/Desktop/alnafi-2.0`.
2. Installs the `httpd` package.
3. Creates an index file at `/var/www/html/index.html`.
4. Enables and starts the `httpd` service.

```ruby
file '/home/ec2-user/Desktop/alnafi-2.0' do
  content 'Welcome to chef-devops Lets automate our machines through chef'
  action :create
end

package 'httpd' do
  action :install
end

file '/var/www/html/index.html' do
  content 'Welcome to apache server'
  action :create
end

service 'httpd' do
  action [:enable, :start]
end
