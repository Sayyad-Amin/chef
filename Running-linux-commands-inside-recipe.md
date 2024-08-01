# How to run linux commands inside a recipe
file '/myfile' do
  content 'Welcome to sp21-bcs-015'
  action :create
end

execute "run a script" do
command <<-EOH
mkdir /alnafidir
touch /alnafifile
EOH
end
