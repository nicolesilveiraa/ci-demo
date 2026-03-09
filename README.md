 Pipeline de CI com GitHub Actions

Este projeto foi criado para uma atividade prática sobre Continuous Integration utilizando GitHub Actions. A ideia foi criar um pipeline  que executa automaticamente quando acontece um push no repositório.

O objetivo da atividade foi aprender como funciona a automação de tarefas dentro do GitHub e entender como configurar um pipeline simples.

O arquivo principal é o `.github/workflows/ci.yml`, que é onde está o workflow do pipeline. Também tem o arquivo `README.md`, para explicar o projeto.

No arquivo `ci.yml` foi criado um workflow chamado **CI Example**. Esse workflow é executado sempre que acontece um **push** no repositório. Dentro dele existe um job chamado **first-job**, que roda em um ambiente **ubuntu-latest**. Esse job possui um passo chamado **Print message**, que executa o comando `echo "Pipeline executado com sucesso!"` para mostrar uma mensagem no terminal.

O funcionamento do pipeline acontece da seguinte forma: quando é feito um push no repositório, o GitHub Actions detecta essa mudança e executa automaticamente o pipeline. Depois disso o job roda, executa o comando configurado e mostra a mensagem no terminal.

Assim é possível ver na aba **Actions** do GitHub que o pipeline foi executado e que tudo funcionou corretamente.
