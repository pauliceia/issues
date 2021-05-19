# Contributing to the Pauliceia Project

Any help is welcome! Those who are thinking of contributing to the project needs only to read this guide.

## 1- Fork the repository

The first thing you need to do is fork our repository. When you Fork a repository, a copy of it will be added to your Github account.

![fork_repositorio](https://user-images.githubusercontent.com/55334621/118742818-7d476b80-b827-11eb-880e-343213049953.png)

### 2- Set up local repository

You will now need a local fork of the project. First, you will need to get your SSH key.
![image](https://user-images.githubusercontent.com/55334621/118745672-0e6d1100-b82d-11eb-8bf2-d79d79c6a55b.png)

After that, click on SSH. 
![image](https://user-images.githubusercontent.com/55334621/118745776-52601600-b82d-11eb-886a-72fb9f9b96e3.png)

Copy the generated URL and clone the repository locally with the command "git clone <SSH>" in your terminal, as in the example below:
``` bash
git clone git@github.com:stackOvercrow/pauliceia.git
```
  
When cloning, the remote repository on Github will automatically be configured as remote on your environment. Now you can develop your feature.

### 3- Pushing to the remote repository

As soon as you finish developing your feature, open the terminal in the folder of your local repository. Use the commands below to add your files, create a commit and send it to the remote repository:
  
``` bash
git add .
git commit -m "Nome do Commit aqui"
git push origin master
```

### 4- Openign a Pull Request

To open a Pull Request to the Pauliceia repository, click on Contribute.
![image](https://user-images.githubusercontent.com/55334621/118753891-44fe5800-b83c-11eb-8034-7fcb13653800.png)
  
Then, click in Open Pull Request.
![image](https://user-images.githubusercontent.com/55334621/118753519-935f2700-b83b-11eb-90e1-76726c946709.png)

  
When creating the Pull Request, Github will ask for a title and description. It is important that you fill these fields in a way that explains the feature that you have developed.

 
![image](https://user-images.githubusercontent.com/55334621/118753590-aeca3200-b83b-11eb-8d2a-557a6c2ab64c.png)
  
Your Pull Request Inglês will be verified by one of our members.
