## Track de seguidores no twitter

## Instalação
Para instalar -
* Clone o projeto (`git clone https://github.com/WesleyDettmer/twitter-new-followers-tracker.git`)
* Instale os pacotes requisitados pelo arquivo de texto - (`'pip3 install -r requisitos.txt'`)

## Configuração
A configuração base do projeto se dá com três arquivos principais:
* `.env`
    * Contém as informações da API do Twitter. Após criada a conta de desenvolvedor, criada as chaves de acesso, de API e o token, essas informações devem ser copiadas corretamente em acordo com as variáveis `API_KEY`, `API_SECRET`, `ACCESS_TOKEN`, `ACCESS_SECRET` e `BEARER_TOKEN`.
    * Caso o projeto seja versionado e compartilhado é importante descomentar a linha que exclui o `.env` do `.gitignore`.
* `users.csv`
    * Controla a lista de usuários a serem observados pelo bot, sendo a primeira linha o cabeçalho, onde a a coluna de 'Usuários' sendos usuários a lista a ser dada, podendo outras colunas serem adicionadas para controle se necessário.
* `formatoMensagem.txt`
    * Controla o formato do tweet caso um dos usuários da lista siga alguém. Esse formato deve conter dois `{}` que serão respectivamente o usuário da lista e aquele que foi seguido (ex: "@{} acabou de seguir @{}!" (formato padrão) se tornaria "@wes acabou de seguir @perfildeTI")

## Uso
Após instalado e configurado, o projeto pode ser rodado com `python3 bot.py` ou, no Linux, `./bot.py`.
