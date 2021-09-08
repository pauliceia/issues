Especificação de Requisitos do Usuário

1. Propósito do documento

Este documento contém as especificações de requisitos do usuário para a interface de usuário (UI) da plataforma Pauliceia 2.0.

2. Escopo da plataforma

Plataforma computacional para pesquisa histórica colaborativa, que permite ao usuário criar, organizar, armazenar, integrar, processar e publicar conjuntos de dados espaço-temporais de história urbana.

3. Características do usuário

  a. Usuário visitante

  Qualquer pessoa com interesse em consultar e visualizar dados de história urbana através da plataforma.

  b. Usuário colaborador

  Qualquer pessoa interessada em participar do processo colaborativo de criação e publicação de dados através da plataforma.

4. Requisitos da interface de usuário (UI)

  4.1 Home

  O propósito dessa tela é funcionar como página inicial da plataforma. Ela deverá conter os seguintes elementos:

    4.1.1 Barra superior

       a. Logo compacta do projeto Pauliceia 2.0
       b. Menu com links para as páginas principais da plataforma:
          i. Home
          ii. Mapa
          iii. Tutorial
          iv. Sobre
          v. Publicações
          vi. Contato
       c. Botão “Criar conta” com link para a página de criação de conta para novo usuário. 
       d. Botão “Entrar” com link para a página de login para usuário já cadastrado.
       e. Botão com ícone do globo com link para a versão traduzida da plataforma:
          i. Caso o usuário esteja acessando a versão em Português da plataforma, o botão deverá exibir o ícone do globo mais as iniciais “ENG” para English.
          ii. Caso o usuário esteja acessando a versão em Inglês da plataforma, o botão deverá exibir o ícone do globo mais as iniciais “PT” para Português.

    4.1.2 Corpo 
    
      Banner central contendo os seguintes elementos:
          i. Imagem como background na resolução 1440 x 679 pixels.
          ii. Banner em posição centralizada na cor branca com tamanho 738 x 475 pixels.
          iii. Logo completa do projeto Pauliceia 2.0.
          iv. Breve texto sobre os objetivos da plataforma e seu funcionamento.
          v. Botão “Saiba mais” com link para a página “Sobre”.

    4.1.2 Rodapé
    
      a. Três colunas contendo as logos das instituições envolvidas com o projeto com links para suas respectivas páginas de website: 
          i. Realização
          ii. Apoio
          iii. Financiamento
          
      b. Texto de rodapé contendo as seguintes informações:
          i. O tipo de licença livre adotada pela plataforma
          ii. O link para a página do Github do projeto.

  4.2 Mapa 

  O propósito dessa tela é permitir ao usuário pesquisar endereços e visualizá-los através dos mapas, assim como também visualizar, criar e editar camadas. Ela deverá conter os seguintes elementos:

    4.2.1 Barra superior

      Conforme item 4.1.1

    4.2.2 Corpo

      a. Background com mapa padrão com resolução padrão de 1440 x 910 pixels.
      b. Banner em posição centralizada com tamanho 898 x 518 pixels.
      c. Logo completa do projeto Pauliceia 2.0
      d. Texto de boas-vindas explicando que a plataforma está em fase de testes, que podem surgir erros e como o usuário pode reportá-los.
      e. Botão “Fechar” que deverá permitir ao usuário fechar o banner de boas-vindas. 
      f. Barra de ferramentas lateral expansível (collapsible sidebar) contendo os seguintes elementos:
        i. Botão “Pesquisar” que deverá permitir ao usuário realizar buscas inserindo o(s) endereço(s) a ser(em) pesquisado(s). Ao clicar neste botão, a UI deverá permitir ao usuário: 
          1. Visualizar um campo de texto e inserir um endereço a ser pesquisado.
          2. Visualizar um botão para realizar o envio (upload) de arquivos em formato CSV (Comma-separated values) contendo os endereços a serem pesquisados. Após o envio do arquivo, a UI deverá permitir ao usuário:
            a. Visualizar os dados do resultado da busca por endereços dentro da própria plataforma.
            b. Realizar o download dos dados do resultado da busca por endereços.
        ii. Botão “Visualizar camadas” que deverá permitir ao usuário acessar todas as camadas disponíveis na plataforma. 




