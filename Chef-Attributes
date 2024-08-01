# Chef Attribute

Attribute is a key-value pair which represents a specific detail about a node.

```ruby
file '/home/ec2-user/Desktop/attributes-by-chef' do
  content "These attributes are generated through
  chef configuration management tool
  HOSTNAME: #{node['hostname']}
  IPADDRESS: #{node['ipaddress']}
  CPU: #{node['cpu']['0']['mhz']}
  MEMORY: #{node['memory']['total']}"
  owner 'root'
  group 'root'
  action :create
end

Output:

These attributes are generated through chef configuration management tool:

HOSTNAME: ip-172-31-60-218
IPADDRESS: 172.31.60.218
CPU:
MEMORY: 972320kB
