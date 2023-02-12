# FIAP-1SCJRBB-Cloud_Development
English School

#Trabalho para a disciplina de CLOUD DEVELOPMENT.

"Disponibilizar em uma gravação vídeo disponibilizado ao professor uma apresentação com diagrama de arquitetura de solução Azure contendo no mínimo 3 serviços que se comuniquem e explicar o projeto mostrando a solução rodando em seu ambiente Azure com evidências como dados no banco de dados, log da aplicação ou ainda mensagens no broker de mensagem. Além do vídeo disponibilizar um repositório público onde seja possível ter acesso ao código fonte das aplicações que compõem a solução."

Nesse exemplo vamos ver de forma simples os mais conhecidos como máquinas virtuais, banco de dados, storage, redes etc. 

Após as configfurações os acessos à nossa aplicação se dará de duas formas diferentes: uma via cURL e outra diretamente pelo browser com umas das rotas da aplicação, observando as respostas dos dados em tela de forma responsiva na internet da nossa aplicação pelo web server (nossa Máquina Virtual criada).


Vídeo da Apresentação no Youtube: https://youtu.be/_aWXbJjCwqE


Visão geral - AZURE:

![image](https://user-images.githubusercontent.com/101299093/218313168-5e906346-7e11-43d7-ad74-024103a98c45.png)


Principais recursos:

Máquina Virtual utilizada como servidor web:

![image](https://user-images.githubusercontent.com/101299093/218313512-16a5358a-f44a-4831-8308-9cc98f0a4238.png)


IP Público:

![image](https://user-images.githubusercontent.com/101299093/218313581-94a5f5da-7d5c-4a53-ad5c-227bb551d5e0.png)


Disco de 30 GB:

![image](https://user-images.githubusercontent.com/101299093/218313622-9e255817-41fd-4907-948d-394bd37aef10.png)


Servidor flexível do Banco de Dados do Azure para MySQL:

![image](https://user-images.githubusercontent.com/101299093/218313670-e7948714-655d-46b7-8ec7-3511577d4ddb.png)


Diagrama da arquitetura Azure:

![image](https://user-images.githubusercontent.com/101299093/218313851-7d3d543c-7953-4b6c-8f04-7687c143edd5.png)


Acessando a VM:
ssh -i fiap_cloud.pem fiap_cloud_user@4.228.84.4

Chave de acesso (fiap_cloud.pem)

![image](https://user-images.githubusercontent.com/101299093/218313964-f46fe409-a921-4307-befd-4ff3e4080beb.png)


Acessando o Banco de Dados, databases e tabelas:

hostname=fiap-cloud-db.mysql.database.azure.com 

username=fiapdb

password=MySqlCloud1234@

database: school_db

Comando para acessar:
mysql -h fiap-cloud-db.mysql.database.azure.com -u fiapdb -p

![image](https://user-images.githubusercontent.com/101299093/218314087-ca080279-dd57-474c-b35c-173b7d181651.png)


Ver conteúdo de algumas tabelas:

![image](https://user-images.githubusercontent.com/101299093/218314192-afd84ca3-4e7a-4786-b668-b312556d4bb3.png)


LOG de atividade das últimas 24 horas:

![image](https://user-images.githubusercontent.com/101299093/218314342-565af722-311f-417a-95d2-5e14edb38ae2.png)


Integração da api:

Start na api:
Comando: DEBUG=cloud-development-vm:* npm start

![image](https://user-images.githubusercontent.com/101299093/218314475-a98a4e2d-6ffe-4ee2-8c96-1a340b212faf.png)


Consulta da tabela turmas pelo terminal (fora da vm):

![image](https://user-images.githubusercontent.com/101299093/218314525-d5dae2e3-ec38-4631-a78f-09730f6297b4.png)


Consultando a tabela pessoas pelo navegador de internet:

![image](https://user-images.githubusercontent.com/101299093/218314650-edb5bbec-760f-4299-ab22-49f00c0b00eb.png)

Obrigado!
