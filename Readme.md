# Projetos do Santander Bootcamp

*Exposição de comandos para facilitar a utilização do Git e exposição de projetos em geral.*



#### Comandos para uso do Terminal Windows e Git Bash

|                            Ações                             | **Comandos para Terminal Windows** |         Comandos Git Bash          |
| :----------------------------------------------------------: | :--------------------------------: | :--------------------------------: |
|         Apresenta diretórios contidos na pasta atual         |             ***dir***              |             ***ls*** ¹             |
|  Navega entre as páginas (Use ".." para retornar um nível)   |       ***cd*** / ***cd ..***       |       ***cd*** / ***cd ..***       |
|        Limpa o terminal para facilitar visualizações         |             ***cls***              |   ***Clear*** ou ***Ctrl + L***    |
|                  Auto completar informações                  |             ***Tab***              |             ***Tab***              |
|                         Criar pastas                         |            ***mkdir***             |            ***mkdir***             |
| Criar arquivos (Deve estar acompanhado do "> + Nome do arquivo") |       ***echo > Test.txt***        |              ***-***               |
|             Apagar arquivos dentro de uma pasta              |       ***del Nomedapasta***        |              ***-***               |
|          Apagar pasta por completo e seus arquivos           |      ***rmdir Nomedapasta***       |              ***-***               |
|            Ler o conteúdo de um arquivo de texto             |              ***-***               |             ***cat***              |
|              Mostra o caminho até a pasta atual              |              ***-***               |             ***pwd***              |
|                       Mover um arquivo                       |              ***-***               | ***mv nomedoarquivo ./novolocal*** |

¹ No comando ls, ao acrescentar o parâmetro "-a" o mesmo ira listar as pastas ocultas.



#### Comandos de criação de Chave SSH

|                   Ações                   |                       Comandos                        |
| :---------------------------------------: | :---------------------------------------------------: |
| Criação das chaves publica e privada SSH² | ***ssh-keygen -t ed25519 -C emailquedesejavincular*** |
| Processo que ficara gerenciando as chaves |              ***eval $(ssh-agent -s)***               |
|     Designação de chave para o Agent      |          ***ssh-add arquivodachaveprivada***          |

² Os comandos executados devem ser no git bash global.



#### Inicialização e gerenciamento do Git em um projeto

|                        Ações                         |                      Comandos                       |
| :--------------------------------------------------: | :-------------------------------------------------: |
|      Iniciar o Git dentro de uma pasta/projeto       |                   ***Git Init***                    |
|  Salvar e-mail do Autor para assinatura dos Commits  | ***git config --global user.email "emaildoautor"*** |
|   Salvar nome do Autor para assinatura dos Commits   |  ***git config --global user.name "nomedoautor"***  |
|           Mostrar as configurações do git            |               ***git config --list***               |
|       Apagar credencial e-mail de usuário git        |    ***git config --global --unset user.email***     |
|       Apagar credencial Nome de usuário do git       |     ***git config --global --unset user.name***     |
|         Mostra as pendências do seu projeto          |                  ***git status***                   |
|   Transferir pastas/arquivos para setor de Staged    |         ***git add nomedoarquivo/pasta*** ³         |
|                   Criar um Commit                    |        ***git commit -m "Nomedaalteração"***        |
|        Orientar o Github o repositório local         | ***git remote add origin linkdorepositorioremoto*** |
| Verificar o repositório que o projeto está vinculado |                 ***git remote -v***                 |
|     Enviar atualização para o repositório remoto     |             ***git push origin main***              |
|  Baixar a versão mais recente do repositório remoto  |             ***git pull origin main***              |
|    Clonar um repositório para minha máquina local    |          ***git clone linkdorepositorio***          |

³ Para realizar todas as mudanças de uma unica vez, é possível usar á variavel "*" ou "."
	Ex¹: Git add *
	Ex²: Git add .
