# Atividade API em Node JS

## Descrição do Projeto:
O projeto consiste em um servidor feito puramente com Node JS para testar a nossa compreensão sobre APIs e métodos de requisição. O servidor em questão simula uma API de organização de tarefas, onde é possível utilizar os métodos GET para listar as tarefas, POST para criar tarefas, PUT para alterar tarefas já criadas e DELETE para deletar tarefas, esses dois últimos feitos com base no ID de cada tarefa, representando assim as 4 operações fundamentais do CRUD.

## Tecnologias Utilizadas:
- Node JS com APIs.

## Como Configurar o Ambiente:
- Certifique-se de ter o Node.js instalado. Verifique com:

```node -v```

- A versão deve ser 14 ou superior.
- Clone ou baixe este repositório.
- Não há dependências externas — nenhum npm install é necessário.

## Como executar o projeto:
- Basta abrir o terminal e executar o seguinte comando:

```node app.js```

## Solução do Problema:
Para garantir que todas as tarefas fossem salvas, foi utilizado o File System (fs) do Node JS para salvar cada tarefa dentro do arquivo "tasks.js". Para buscar por tarefas pelo ID, foi necessário navegar por cada tarefa criada no arquivo de tarefas até que fosse encontrada a tarefa com o ID desejado usando o método .find(). O campo "completed" foi implementado sem muitas dificuldades no arquivo de modelo das tasks, a lógica para alterar esse campo segue a mesma lógica para alterar o nome das tarefas, é necessário escolher o ID da tarefa a ser alterada e por fim definir que queremos alterar o campo "completed" da tarefa, inserindo em seguida seu novo valor.
