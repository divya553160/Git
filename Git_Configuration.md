# Git has 3 levels of Configuration files :

     Local level (Project/Repository) :- 
     
              Configurations available for only the current project and stored in .git/config in the project's directory.
     
     Global level (User account) :- 
              
              Configurations available for all the projects for the current user and stored in ~/.gitconfig.
     
     System level (git installation) :- 
      
              Configurations are available for all the users/projects ans stored in usr/etc/gitconfig.
              
# To create a local config,execute below command in the project's directory :

     $ git config user.name "Hardhik Pandya"
     
# To create a global config :

     $ git config --global user.name "Hardhik Pandya"
     
# To create a system config :

     $ git config --system user.name "Hardhik Pandya"
  
