# InteragindoGithubComGit
Criado com o objetivo de mostrar comandos básicos para operar o Git Bash criando e adicionando itens ao repósitório no GitHub. 


## Primeiros passos:
- Instale o Git no site oficial e selecione as configurações que recomendam.
- Crie uma conta no GitHub.
- Abra a pasta do arquivo que deseja realizar o upload.
- Clique com o botão direito dentro da janela da pasta.
- Clique no Git Bash.
- Digite: (Para inicializar o git na pasta.)      

        git init
- Digite: (Para adicionar um arquivo a uma parte de espera para depois ser empurrado ao repositório, porém se for todos os arquivos de dentro da pasta basta usar o . no lugar do "Nome do arquivo". Exemplo: git add . ) 

        git add "Nome do arquivo"
- Digite: (Use esse comando sempre após um comando para evitar uma cascata de erros.)  
        
        git status
- Digite: (Após mandar o arquivo para a espera é necessário fazer um comentário de registro.)  

        git commit -m "Primeiro commit"
- Digite: (Caso queira mudar o nome do seu branch atual, geralmente é utilizado o nome main.)  

        git branch -M main


## Crie um repositório
- Ao abrir o github.com com a conta logada, na aba superior a sua direita há um círculo com sua   imagem de perfil. Clique nele e selecione a opção "Your repositories", clique em "New".


## Configurando novo repositório
- Coloque o título sem espaços.
- Descrição é opcional, serve para descrever o repositório caso seja necessário!
- Selecione a opção de privacidade que preferir para seu repositório, a "Public" tem a função de poder ser vista e pesquisada por qualquer usuário, enquanto que a "Private" permite que seja   apenas visto e pesquisado por você e os colaboradores que adicionar através das configurações pós feito o repositório.
- Ao clicar em "Add a README file", cria um arquivo com extensão markdown dentro do repositório no qual permite mostrar textos, imagens e etc, como este texto que você está lendo agora.
- O "Add .gitignore" faz com que o git ignore os tipos de arquivos que você selecionou como desnecessários para atualizações no repositório do GitHub. (Opcional, pois se não quiser é só   deixar do jeito que está!) 
- "Choose a license" pode a inserir a licença que mais lhe agrada. (Opcional, pois se não quiser é só deixar do jeito que está!)


## Enviar arquivos em espera no Git ao repositório recém criado no GitHub
- Digite:  

      git remote add origin https://github.com/NomeDoUsuário/NomeDoRepositório.git
- Digite:  

      git branch -M main
- Digite (Depois de usar esse comando pela primeira vez, só é necessário utilizar o comando "git push"):

      git push -u origin main
      
       
## Adicionando o repositório já existente a sua máquina local e modificando seus itens
- Abra seu Git Bash, deixe-o no diretório que desejar.
- Coloque o comando:   

      git clone https://github.com/NomeDeUsuário/NomeDoRepositório.git
- É só acessá-lo no diretório escolhido.
- Digite:  (Após fazer as suas modificações e sempre use o git status para saber se há algum problema que têm que resolver!)

      git add .
- Digite:  

      git commit -m "Seu comentário"
- Para enviar para o github.com digite o comando:   

      git push -u origin main
- Já está lá, para ver é só acessar a aba de seus repositórios no github.com.


## Possível problema de conflito
Um colega ou você adicionou uma nova versão, enquanto que você estava modificando a versão antiga no seu computador local, na hora de você empurrar a sua versão para o repositório, aparece um erro que não permite este ato. Solução: 

- Digite o comando (Após digitar esse comando pela primeira vez, só é necessário utilizar o comando "git pull"):  

      git pull origin main
- Edite novamente o arquivo se aparecer um conflito na fusão.
- Digite o comando:  

      git add .
- Digite o comando:   

      git commit -m "Seu comentário"
- Digite o comando:   

      git push origin main
- Pronto!


## Comandos essenciais
- cd = Abre um diretório.
- cd -- = Volta ao diretório selecionado anteriormente.
- CTRL+L = Limpa o terminal do Git Bash.
- TAB = Autocompletar termo digitado.
- git clone https://github.com/NomeDeUsuário/NomeDoRepositório.git = Faz uma cópia do repositório no github.com para o seu computador local.
- git add . = Usado para adicionar arquivos novos e modificados do diretório atual.
- git commit -m "" = Permite adicionar um comentário entre as aspas, sobre a modificação realizada.
- git status = Mostra quais alterações não foram ou foram preparadas e quais arquivos não estão sendo monitorados pelo Git.
- git pull -u origin main = Atualiza a sua versão local do repositório para a mais nova existente. 
- git push -u origin main = Empurra a sua versão local do repositório para se tornar a versão mais nova existente. 
