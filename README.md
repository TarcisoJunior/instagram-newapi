# instagram-newapi
Exemplo de consumo da nova api do instagram


Esse código contém um exemplo de consumo da API do Instagram.

Para consumo da API é necessário gerar um token de acesso, seguindo os passos descritos em 
https://www.instagram.com/developer/authentication/

basicamente consiste em seguir os seguintes passos:

1 - cadastrar o cliente, em https://www.instagram.com/developer/clients/manage/

No cadastro do cliente, vc terá que configurar uma url para receber o token gerado (REDIRECT_URI). Pode ser qualquer url, 
o token será gerado no link gerado como um parâmetro da URL

2 - adicionar o usuario na sandbox, na tela de clientes, selecionando a opção Manage

3 - solicitar a autorização do dono da conta a ser pesquisada, através do link
https://api.instagram.com/oauth/authorize/?client_id=CLIENT-ID&redirect_uri=REDIRECT-URI&response_type=code&scope=public_content

Atenção para o parâmetro scope. Sem ele a consulta pode não funcionar dependendo da aplicação em desenvolvimento.

4 - gerar o token, que será usado na consulta acima e retornado na REDIRECT_URI como um parâmetro da url:
http://your-redirect-uri?code=CODE


Você pode, se preferir, usar a url abaixo pra gerar o token
http://www.tarcisojunior.com.br/instagram/

Um exemplo online pode ser testado em
http://www.tarcisojunior.com.br/instagram-newapi/


