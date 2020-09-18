# Configurando virtualenv com Python3
![procedimento](/procedimento.gif)

## Instalação

Inicialmente deve-se instalar o pacote python3-venv que fornece o módulo venv.
```
sudo apt install python3-venv
```

## Utilização

Alterne para o diretório onde deseja armazenar seus ambientes virtuais Python 3. No diretório, execute o seguinte comando para criar seu novo ambiente virtual:
```
python3 -m venv my-project-env
```
O comando acima cria um diretório chamado my-project-env, que contém uma cópia do binário Python, o gerenciador de pacotes Pip, a biblioteca Python padrão e outros arquivos de suporte.

Para começar a usar este ambiente virtual, você precisa ativá-lo executando o script **activate**:

```
source my-project-env/bin/activate
```

Uma vez ativado, o diretório bin do ambiente virtual será adicionado no início da variável $PATH. Além disso, o prompt do seu shell mudará e mostrará o nome do ambiente virtual que você está usando no momento. No nosso caso, isso é my-project-env:
```
Output

$ source my-project-env/bin/activate
(my-project-env) $
```

Agora que o ambiente virtual está ativado, podemos começar a instalar, atualizar e remover pacotes usando pip.

Para instalar varios modulos, deve-se criar um arquivo **requirements.txt** contendo a lista de modulos por exemplo:
```
requirements.txt

numpy
pandas
```
Em seguida executar o comando:
```
(my-project-env) $ pip install -r requirements.txt
```

Tudo pronto para rodas os scrips na sua venv python3!!

Assim que terminar seu trabalho para desativar o ambiente, simplesmente digite **deactivate** e você retornará ao seu shell normal.

```
(my-project-env) $ deactivate
```

```
$
```

