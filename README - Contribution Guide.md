# Contributing to the Pauliceia Project

Any help is welcome! Those who are thinking of contributing to the project needs only to read this guide.

## 1- Fork the repository

The first thing you need to do is to fork our repository. When you fork a repository, a copy of it will be added to your Github account.

![fork_repositorio](https://user-images.githubusercontent.com/55334621/118742818-7d476b80-b827-11eb-880e-343213049953.png)

### 2- Set up local repository

You will now need a local repository of the project. First, you will need to get your SSH key.
![image](https://user-images.githubusercontent.com/55334621/118745672-0e6d1100-b82d-11eb-8bf2-d79d79c6a55b.png)

After that, click on SSH. 
![image](https://user-images.githubusercontent.com/55334621/118745776-52601600-b82d-11eb-886a-72fb9f9b96e3.png)

Copy the generated URL and clone the repository locally with the command "git clone <SSH>" in your terminal, as in the example below:
``` bash
git clone git@github.com:stackOvercrow/pauliceia.git
```
  
When cloning, the remote repository on Github will automatically be configured as remote on your environment.
  
### 4- Downloading dependencies of the project

Open the terminal in the folder of your local repository and run the following command:

``` bash
npm install 
```

This command will install the dependencies of Pauliceia. After running it, go to the config directory and create a copy of the "prod.env.js.EXAMPLE" file  in the same directory. After that, rename the copy by removing the ".js.EXAMPLE" from the filename. The result will be:

![image](https://user-images.githubusercontent.com/55334621/125361107-3cf5fc80-e343-11eb-8477-68b2de32dacb.png)
  
### 5- Running the server
  
Now, to run the server, run the following command in the terminal:

``` bash
npm run dev 
```

After the application is fully built, your terminal should look like the one in the photo below. 

![image](https://user-images.githubusercontent.com/55334621/140801701-31b7cfff-2d03-4553-9fbb-a24e9ec781ae.png)

### 6- Pushing to the remote repository
 
As soon as you finish developing your feature, open the terminal in the folder of your local repository. Use the commands below to add your files, create a commit and send it to the remote repository, but your commit name must follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0-beta.2/):
  
``` bash
git add .
git commit -m "Commit name"
git push origin master
```

### 7- Opening a Pull Request

To open a Pull Request to the Pauliceia repository, click on Contribute.
![image](https://user-images.githubusercontent.com/55334621/118753891-44fe5800-b83c-11eb-8034-7fcb13653800.png)
  
Then, click in Open Pull Request.
![image](https://user-images.githubusercontent.com/55334621/118753519-935f2700-b83b-11eb-90e1-76726c946709.png)

When creating the Pull Request, Github will ask for a title and description. It is important to emphasize two points: 
  1. Your Pull Requests names must follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0-beta.2/);
  2. Pull Requests must be made to the develop branch, as shown in the image. 
 
![image](https://user-images.githubusercontent.com/55334621/140802850-4dadfeb0-2139-4181-a070-179a4cadddfb.png)
  
Now just wait for one of our members to verify your Pull Request.
