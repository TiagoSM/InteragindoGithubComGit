# InteragindoGithubComGit
Criado com o objetivo de mostrar comandos básicos para operar o Git Bash criando e adicionando itens ao repósitório no Github. 



## Primeiro crie um repositório
- Ao abrir o github.com com a conta logada, na aba superior a sua direita há um círculo com sua   imagem de perfil. Clique nele e selecione a opção "Your repositories", clique em "New".


## Configurando novo repositório
- Coloque o título sem espaços.
- Descrição é opcional, serve para descrever o repositório caso seja necessário!
- Selecione a opção de privacidade que preferir para seu repositório, a "Public" tem a função de poder ser vista e pesquisada por qualquer usuário, enquanto que a "Private" permite que seja   apenas visto e pesquisado por você e os colaboradores que adicionar através das configurações pós feito o repositório.
- Ao clicar em "Add a README file", cria um arquivo com extensão markdown dentro do repositório no qual permite mostrar textos, imagens e etc, como este texto que você está lendo agora.
- O "Add .gitignore" faz com que o git ignore os tipos de arquivos que você selecionou como desnecessários para atualizações no repositório do Github. (Opcional, pois se não quiser é só   deixar do jeito que está!) 
- "Choose a license" pode a inserir a licença que mais lhe agrada. (Opcional, pois se não quiser é só deixar do jeito que está!)


## Adicionando o repositório a sua máquina local e modificando seus itens
- Abra seu Git Bash, deixe-o no diretório que desejar.
- Coloque o comando "git clone https://github.com/NomeDeUsuário/NomeDoRepositório.git".
- É só acessa-lo no diretório escolhido.
- Quando terminar de modificar use o comando "git add *" para atualizar o versionamento local.
- Logo em seguida "git commit -m "Seu comentário" " para comentar o que foi modificado.
- Para enviar para o github.com digite o comando "git push origin main". (o termo "main" é na verdade o nome do ramo principal, que geralmente é main ou master, mas é personalizável!)
- Já está lá, para ver é só acessar a aba de seus repositórios no github.com.


## Possível problema de conflito
Um colega ou você adicionou uma nova versão, enquanto que você estava modificando a versão antiga no seu computador local, na hora de você empurrar a sua versão para o repositório, aparece um erro que não permite este ato. Solução: 

- Digite o comando "git pull origin main".
- Edite novamente o arquivo se aparecer um conflito na fusão.
- Digite o comando "git add *".
- Digite o comando "git commit -m "Seu comentário" ".
- Digite o comando "git push origin main".
- Pronto!


## Comandos essenciais
- cd = Abre um diretório.
- cd -- = Volta ao diretório selecionado anteriormente.
- CTRL+L = Limpa o terminal do Git Bash.
- TAB = Autocompletar termo digitado.
- git clone https://github.com/NomeDeUsuário/NomeDoRepositório.git = Faz uma cópia do repositório no github.com para o seu computador local.
- git add * = Usado para adicionar arquivos novos e modificados do diretório atual.
- git commit -m "" = Permite adicionar um comentário entre as aspas, sobre a modificação realizada.
- git status = Mostra quais alterações não foram ou foram preparadas e quais arquivos não estão sendo monitorados pelo Git.
- git pull origin main = Atualiza a sua versão local do repositório para a mais nova existente. 
- git push origin main = Empurra a sua versão local do repositório para se tornar a versão mais nova existente. 
