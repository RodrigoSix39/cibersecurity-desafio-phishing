# Phishing para captura de senhas do Facebook

### Ferramentas

- Kali Linux
- setoolkit

### Configurando o Phishing no Kali Linux

- Acesso root: ``` sudo su ```![2-sudo_su_command](https://github.com/user-attachments/assets/c66fe208-ea6b-4270-af4a-d6108fc4fb22)

- Iniciando o setoolkit: ``` setoolkit ```![setoolkit_command](https://github.com/user-attachments/assets/2e0c372e-05c7-4a6b-a701-da07f9cd1866)

- Tipo de ataque: ``` Social-Engineering Attacks ```![setoolkit_1st_menu_option_1](https://github.com/user-attachments/assets/e0242515-2d06-4f1d-bfce-a94edb200bfe)

- Vetor de ataque: ``` Web Site Attack Vectors ```![setoolkit_2nd_menu_option_2](https://github.com/user-attachments/assets/c2723284-ae82-4ade-ad32-53a46568f4df)

- Método de ataque: ```Credential Harvester Attack Method ```![setoolkit_3rd_menu_option_3](https://github.com/user-attachments/assets/aaa0481a-d622-441d-9dfd-d5487eb4440f)

- Método de ataque: ``` Site Cloner ```![setoolkit_4th_menu_option_2](https://github.com/user-attachments/assets/8387b3c3-4060-41ca-8ed5-b941fd28537d)

- Obtendo o endereço da máquina: ``` ifconfig ```![setoolkit_ip_address_input](https://github.com/user-attachments/assets/107d6773-e3e9-40f5-bf02-a57940a3a5bf)

- URL para clone: http://www.facebook.com
![setoolkit_site_to_be_cloned_input](https://github.com/user-attachments/assets/84a28da6-00b9-40df-9e1f-4de16dc6d281)

### Resutados

![setoolkit_result](https://github.com/user-attachments/assets/d4a7c7b3-0b31-41fa-8595-51c8b1dcfe78)

### Alternativa
Aparentemente este metodo não funciona mais para o facebook. Como alternativa criei um servidor node js usando express e nodemailler e fiz pequnas alterações em um clone existente do facebook para receber no servidor o email e senha digitados e redirecionar o usuário para a pagina real do facebook. O servidor então envia através do nodemailler o que foi digitado nos campos de email e password para meu email.

-Rodando o servidor local
![server_running_localhost](https://github.com/user-attachments/assets/9da6ce63-a277-4d86-9148-e0f49ea4d532)

-Criando o servidor remoto com ngrok na porta 3000
![ngrok_serving](https://github.com/user-attachments/assets/6c5e8f6a-43f5-469a-ba6d-c44339b39ba6)

-Copiando o endereço fornecido pelo ngrok
![ngrok_forwarding](https://github.com/user-attachments/assets/698d3aaa-0b9d-4da4-85ab-857a90a4db92)

-Acessando a pagina clonada e inserindo email e senha
![accessing_coned_facebook](https://github.com/user-attachments/assets/0d0fd698-e193-4927-8d17-213e454955a7)

-Sendo redirecionado para o facebook real
![redirected_to_real_facebook](https://github.com/user-attachments/assets/bc780ac3-656a-4a24-9bbb-874591e4f0a1)

-Recebendo dados digitados no back end
![email_password_on_server_log](https://github.com/user-attachments/assets/80c4eb2a-415a-4b6c-b0be-44b2e3ca4b47)

-Recebendo dados digitados no email
![result_on_gmail](https://github.com/user-attachments/assets/50721cd1-fbb7-419f-a552-4e58bbdfabbb)





