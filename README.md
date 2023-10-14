# to-do-list
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/PedroRSilveira/to-do-list/blob/main/LICENSE)
# Sobre o projeto

to-do-list é um software de lista de tarefas (to-do list) desenvolvido em Java usando o framework Spring Boot e a gestão de dependências com o Maven. Consiste em um sistema para criar, acessar e editar tarefas. O sistema está hospedado no serviço de nuvem Render e pode ser acessado a partir da seguinte URL: https://todolist-5efv.onrender.com

# Demonstração do software

Para usar o sistema é preciso usar uma plataforma de API, nesse caso o Postman.

<br/>

- Cadastrando um usuário:

A primeira coisa a se fazer é cadastrar um usuário. É feito com o método POST, usando a URL no início da documentação com "/users/" no final, passando os campos username, name e password via JSON como mostra a imagem abaixo.

![image](https://github.com/PedroRSilveira/to-do-list/assets/120536516/05e922d5-e88c-4d87-ade7-abca680e9aa1)

Resposta da API:

![image](https://github.com/PedroRSilveira/to-do-list/assets/120536516/fb880cc2-549f-41ae-b559-728b4b31ffe4)

- Cadastrando uma tarefa:

Para cadastrar uma tarefa o usuário precisa estar cadastrado. Usando o método POST com a URL do início da documentação com "/tasks/" no final, passando o usuário e senha em Basic Auth e os campos description, title, priority, startAt e endAt via JSON como mostrado nas imagens abaixo.

Validação do usuário:

![image](https://github.com/PedroRSilveira/to-do-list/assets/120536516/78b190cb-c172-4367-b051-b773d6f5b8b8)

Criação da tarefa:

![image](https://github.com/PedroRSilveira/to-do-list/assets/120536516/262a476e-11bd-44b1-bb60-0242a16e7f53)

Resposta da API:

![image](https://github.com/PedroRSilveira/to-do-list/assets/120536516/678af7a2-c4a2-4250-ae2d-217a030d02dc)

- Lista de tarefas:

Para ver a lista de tarefas do usuário, é preciso usar o método GET com a URL do início da documentação com "/tasks/" no final, passando o usuário e senha em Basic Auth, como mostra a imagem abaixo:

![image](https://github.com/PedroRSilveira/to-do-list/assets/120536516/c9220b09-7533-4818-bb4e-8233df6b27de)

Resposta da API:

![image](https://github.com/PedroRSilveira/to-do-list/assets/120536516/3d43e50b-c738-46df-97ed-adbccf4a1581)

- Editar tarefa:

Para editar um campo específico de uma tarefa é preciso usar o método PUT com a URL do início da documentação com "/tasks/{id}" no final, substituindo {id} pelo id da tarefa que deseja editar. Então passar o usuário e senha em Basic Auth e digitar os campos que deseja alterar via JSON como mostrado na imagens abaixo:

Validação do usuário:

![image](https://github.com/PedroRSilveira/to-do-list/assets/120536516/870fc449-4c91-4975-9422-73fadd842132)

Edição da tarefa:

![image](https://github.com/PedroRSilveira/to-do-list/assets/120536516/9f78680a-de7d-40df-85c3-19d849e65b76)

Resposta da API:

![image](https://github.com/PedroRSilveira/to-do-list/assets/120536516/ed246d10-9b7f-4cef-a446-e68e99e32c4f)
