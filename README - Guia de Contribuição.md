# Contribuindo para o Projeto Pauliceia

Toda ajuda é bem-vinda! Todos que quiserem contribuir para o andamento do Pauliceia precisam apenas ler este pequeno guia.

## 1- Realizando o fork no repositório

A primeira coisa que você precisa fazer é forkar o nosso repositório. Ao fazer isso, uma cópia dele será adicionada à sua conta no Github.

![fork_repositorio](https://user-images.githubusercontent.com/55334621/118742818-7d476b80-b827-11eb-880e-343213049953.png)

### 2- Set up local repository

Agora, você precisará de um repositório local do projeto. Para isso será necessário que tenha a chave SSH do seu repositório. Para isso, primeiro clique em Code. 
![image](https://user-images.githubusercontent.com/55334621/118745672-0e6d1100-b82d-11eb-8bf2-d79d79c6a55b.png)

Depois, clique em SSH. 
![image](https://user-images.githubusercontent.com/55334621/118745776-52601600-b82d-11eb-886a-72fb9f9b96e3.png)

Copie a URL gerada e clone o seu repositório localmente com o comando "git clone <SSH>" no terminal do seu computador, como no exemplo abaixo:
``` bash
git clone git@github.com:stackOvercrow/pauliceia.git
```
  
Ao clonar, o repositório remoto no Github será automaticamente configurado como o repositório remoto do seu ambiente.
  
### 4- Baixando as dependências do projeto

Abra um terminal na pasta do seu repositório local e digite o seguinte comando:

``` bash
npm install 
```

Este comando instalará automaticamente as dependências do Pauliceia. Depois, vá para o diretório "config" e crie uma cópia do arquivo "prod.env.js.EXAMPLE" no mesmo local e renomeie-o removendo o ".js.EXAMPLE" de seu nome. O resultado esperado será:

![image](https://user-images.githubusercontent.com/55334621/125361107-3cf5fc80-e343-11eb-8477-68b2de32dacb.png)
  
### 5- Fazendo o servidor funcionar
  
Agora, para fazer o servidor funcionar, digite no terminal:

``` bash
npm run dev 
```

Depois que a aplicação terminar de ser construída, seu terminal deverá parecer com o da foto abaixo. 

![image](https://user-images.githubusercontent.com/55334621/140801701-31b7cfff-2d03-4553-9fbb-a24e9ec781ae.png)

### 6- Enviando suas mudanças para o repositório remoto
 
Quando você terminar de desenvolver a sua funcionalidade, abra um terminal na pasta que funciona como seu repositório local. Use os comandos abaixo para adicionar seus arquivos, crie um commit (o nome dele deverá seguir o [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0-beta.2/):) e envie-o para seu repositório remoto.
  
``` bash
git add .
git commit -m "Nome do Commit"
git push origin master
```

### 7- Abrindo um Pull Request

Para abrir um Pull Request para o repositório do Pauliceia, clique em Contribuir.
![image](https://user-images.githubusercontent.com/55334621/118753891-44fe5800-b83c-11eb-8034-7fcb13653800.png)
  
Então, clique em Open Pull Request.
![image](https://user-images.githubusercontent.com/55334621/118753519-935f2700-b83b-11eb-90e1-76726c946709.png)

Ao criar seu Pull Request, o Github irá pedir um título e uma descrição. É importante enfatizar que: 
  1. Os nomes de seus Pull Requests devem seguir [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0-beta.2/);
  2. Pull Requests precisam ser feitos para a branch "develop", como é mostrado na imagem. 
 
![image](https://user-images.githubusercontent.com/55334621/140802850-4dadfeb0-2139-4181-a070-179a4cadddfb.png)
  
Agora é só esperar que o seu Pull Request seja verificado por um de nosso membros.
