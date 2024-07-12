# exemplos_python

Esse repositório conterá alguns códigos pythons de exemplos simples.

## Configuração inicial do projeto

### Criar venv
- No powershell dentro do vscode dar um upgrade no pip:

```cmd
python -m pip install --upgrade pip
pip install --upgrade cryptography
```

- Criar um venv para o projeto
```cmd
python -m venv venv_exemplos_python
```

- Normalmente o Vscode já pergunta se quer vincular essa nova venv ao projeto. Diga sim. Espere 1 minuto para atualizar o projeto. 
- Caso ele não pergunte, executar o novo venv para no terminal

### Usar o PIP Tools para gerenciar os pacotes

- Feche o powershell atual e abra de novo. Quando abrir de novo ele já vai entrar com a nova venv. Caso não procurar rodar o novo venv.

- Adicionar um arquivo `requirements.in` com os pacotes para instalar e instalar o pip-tools

``` cmd
pip install pip-tools
```

- Caso tenha algum problema no comando acima, rodar

``` cmd
python -m pip install pip-tools
```


- Depois, na pasta onde estivar o arquivo requirements.in, rodar 

``` cmd
pip-compile
```

- Ele vai gerar um arquivo 'requirements.txt'que é usado para instalar os pacotes.

- Instalar o pacote através do comando

``` cmd
pip install -r requirements.txt
```

### GIT

- adicionar o arquivo `.gitignore` e configurar para não versionar o diretório `venv`

