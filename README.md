# Instalando_Git_Windows

Instalação e configuração inicial do Git no ambiente Windows.

A instalação é bem simples.

Para as configurações iniciais, precisa de atenção para que todo o seu repositório futuro não tenha problema com a definição da branch principal que é a primeira que o Git cria, no futuro você pode criadas outras branches.

Claro que a qualquer momento se pode alterar nome do branch padrão, seu endereço de e-mail e usuário.

Agora vamos partir para as configurações iniciais:

Primeira coisa a fazer é criar uma pasta em seu diretório principal do Win disco local, que pode ser o C, D, F..., verifique no seu "Gerenciamento de discos" do Windows.

Criado, clique com o botão direito do mouse e abra o "Open Git Bash HERE", vai abrir seu ambiente de trabalho, terminal Git.

Com o Git Bash Here aberto, as primeiras informações que ele traz são, (em verde) nome de usuário, (em rosa) nome do computador e (laranja) nome do diretório criado que se encontra.

Alterar o tema do terminal, mudando as cores das letras e fundo do terminal:

    - clique com o botão direito em "Options..."
    - em Looks -> Colours -> Theme, estará como "*None*", só escolher.
    
![Sem título](https://github.com/angelicakadja/Instalando_Git_Windows/assets/156589643/58340822-443a-410d-8681-354211110d2f)

Informações sobre a ferramenta instalada para que analise e defina variáveis de configurações, comando:
$ git config

Os 3 principais exibidos na configuração inicial:
--global -> referente ao usuário
-- sistem -> referente a sistema como um todo onde abriga todos os usuários e o sistema Win
--local -> referente ao repositório específico, onde armazena o projeto no ambiente local

Sempre que desejar limpar o terminal pressione ctrl + L.

Como deseja que todos as informações commitadas tenha o mesmo *nome e endereço de e-mail* armazene no *--global*.
Claro que futuramente você pode alterar o nome de usuário e e-mail, mas, os commits antigos não terão essas novas variáveis, só os commits após as trocas.

Definir nome do usuário, comando:
$ git config --global user.name "*seu nome*" --> sem as aspas
Exemplo, usei meu nome de usuário do GitHub para unificar tudo e ter mesma informação.

Definir endereço do e-mail do usuário :
$ git config --global user.email "*seu endereço de e-mail*" --> sem as aspas

Confirmar a variável de configuração sobre o *nome do usuário*, se salvou certinho:
$ git config user.name

Confirmar a variável de configuração sobre o *endereço de e-mail*, se salvou certinho:
$ git config user.email

Alterar nome da Branch padrão em *--global*, normalmente se usa *main*, no passado era *master*:
$ git config --global init.defaultBranch "*nome que deseja*" --> sem as aspas

Confirmar a variável de configuração sobre o *nome da Branch padrão*, se salvou certinho:
$ git config init.defaultBranch

Para mais configurações acesse:

https://git-scm.com/doc
