# How to create user and group

user 'zayyan' do
  action :create
end

group 'devops' do
  action :create
  members 'zayyan'
  append true
end
