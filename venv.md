# Virtual env em Python

Em Python, um Virtual Environment (venv) permite instalar pacotes Python em um local isolado do resto do sistema, em vez de instalá-los em todo o sistema. Vejamos como usar o venv:

> *O módulo venv oferece suporte à criação de “ambientes virtuais” leves, cada um com seu próprio conjunto independente de pacotes Python instalados em seus diretórios site. Um ambiente virtual é criado sobre uma instalação existente do Python, conhecido como o Python “base” do ambiente virtual, e pode, opcionalmente, ser isolado dos pacotes no ambiente base, de modo que apenas aqueles explicitamente instalados no ambiente virtual estejam disponíveis.*

> *Quando usadas em um ambiente virtual, ferramentas de instalação comuns, como pip, instalarão pacotes Python em um ambiente virtual sem precisar ser instruído a fazê-lo explicitamente.*


### Criar novo virtual environment (venv), com nome projeto1-venv

```shell
python -m venv projeto1-venv
```
### Ativar o venv criado
```shell
source projeto1-venv/bin/activate
````
### Verificar a versão do pip no venv criado
```shell
pip --version
````
### A título de testes, realizar a atualização do pip no venv criado
```shell
upgrade pip
/<path to venv folder>/projeto1-venv/bin/python -m pip install --upgrade pip
````
### Conferir a versão do pip no venv após atualização
```shell
pip --version
````
### Desativar o venv
```shell
deactivate
```
### Criar novo venv, com nome projeto2-venv
```shell
python -m venv projeto2-venv
````
### Ativar o novo venv
```shell
source projeto2-venv/bin/activate
````
### Verificar a versão do pip no venv projeto2-venv criado 
##### *É esperado que a versão seja diferente da versão do pip no venv projeto1-venv, que foi atualizado, indicando que a atualização do pip realizada no venv projeto1-venv não afetou o pip do venv projeto2-venv*
```shell
pip --version
```

### Referências:
https://docs.python.org/pt-br/3/library/venv.html?highlight=venv

https://python.land/virtual-environments/virtualenv

https://www.slideshare.net/AlphaReaction/python-virtual-environmentpptx
