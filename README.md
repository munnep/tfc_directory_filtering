# tfc_directory_filtering
TFC directory filtering

# Example: null provider and directory filtering with TFC

Directory filtering enables you to define on which directory in your repository terraform will execute [See documentation](https://www.terraform.io/cloud-docs/workspaces/settings#terraform-working-directory) 


# How to

- Clone/Fork this repository to your own VCS
- Within TFC make a new workspace that points to this repository  
![](media/2022-03-10-16-32-40.png)  
![](media/2022-03-10-16-33-00.png)  
![](media/2022-03-10-16-33-19.png)  
![](media/2022-03-10-16-33-36.png)  
- When running a new plan you will get no output. No configuration.   
![](media/2022-03-10-16-35-21.png)  
- change the directory where it should execute from. Go to settings --> General --> Terraform Working Directory
![](media/2022-03-10-16-35-49.png)  
- Change the value to dev/
![](media/2022-03-10-16-36-58.png)  
- save settings
- Create a new run and you should see a null_resource.dev wanting to be created
![](media/2022-03-10-16-44-21.png)  