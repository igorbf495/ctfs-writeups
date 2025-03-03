alvo: 10.129.104.15

como sempre, iniciaremos com um scan na rede com o nmap

![image](https://github.com/user-attachments/assets/1b6423c8-b587-4778-b688-d8024b2e345c)

encontramos somente uma porta em uso, porta 80 rodando um nginx

tentei acesso pela web e não consegui:

![image](https://github.com/user-attachments/assets/051518fd-4ddc-4716-80e2-a9bab2c647a3)

no analisando a request no burp, ele me mostra o status code 302, ou seja, redirect

![image](https://github.com/user-attachments/assets/c591ec8e-1d20-4787-8bc9-cf8c6082a944)

![image](https://github.com/user-attachments/assets/8547c7b7-2750-46b1-8971-6dea7ac512ca)
