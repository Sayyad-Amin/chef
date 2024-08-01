# How to run multiple recipes from multiple cookbooks

We can run only one recipe from each cookbook by this command

#chef-client -zr “recipe[<cookbook-name>::<recipe-name>],recipe[<second-cookbook-name>::<recipe-name>]

If we have to run multiple recipes from a single cookbook We can do it easily
Simply we have to add/include all recipes to default.rb file
Through vi editor we will go inside default.rb and include all recipes that want to execute

include_recipe "<cookbook-name>::<recipe-name>"
include_recipe "<cookbook-name>::<another-recipe-name>"

Now use case is If we want to run multiple cookbooks and recipes through a single command

#chef-client -zr “recipe[<cookbook-name>::<default.rb>],recipe[<second-cookbook-name>::<default.rb>]

This is because we have already added all the recipes into default.rb file.
