alvo: 10.129.229.220

esse write-up documenta a exploracao de um servico mysql em um host especifico. O objetivo eh obter acesso ao banco de dados e capturar a flag armazenada.

iniciei com um scan utilizando o nmap para identificar portas abertas e servicos ativos.


![image](https://github.com/user-attachments/assets/9a6fbd6f-35f3-4d59-a26f-a2af206222a4)

encontramos a porta 3306 aberta rodando o servico mysql.

usando o netcat consegui identificar a versao do mysql

![image](https://github.com/user-attachments/assets/a1df1032-1d6d-40ac-ab26-883bcb9577fb)

usando o mysql para tentar conectar ao banco com user padrao retornou o seguint erro:

![image](https://github.com/user-attachments/assets/5370b23c-1a0a-4e26-8698-d557b4063509)

fui pesquisar sobre e para contornar passei o seguinte parametro

![image](https://github.com/user-attachments/assets/cbd6a753-ece2-47fe-b2dc-4b725b4127d1)

conectado com sucesso usando user root sem senha.

![image](https://github.com/user-attachments/assets/9434e4ea-6ae0-480f-8aa4-252f5d16725f)

vamos ver as tabelas que temos nesse banco

![image](https://github.com/user-attachments/assets/2ec8153b-ddb9-4efc-92ba-c0f3960943a9)

ao explorar mais o banco, conseguimos a flag

![image](https://github.com/user-attachments/assets/b5bf9418-f795-4165-bc7d-ac934e2bedb6)
