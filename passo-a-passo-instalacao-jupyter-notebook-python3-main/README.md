# Passo a passo de instalação do Jupyter Notebook (Python 3)

### Requisitos mínimos para instalação:

> Sistema operacional Linux (esse passo a passo foi feito no Ubuntu 20.04.2 LTS)  <br/>Memória RAM de 4GB ou mais

## **1º Passo** - Instalação do Python3

- Atualize o ambiente antes de iniciar o processo com os seguintes comandos:

````
sudo apt update
sudo apt upgrade -y
````

- Verifique se o Python3 está instalado e qual é sua versão executando o seguinte comando:

````
python3 -V
````

![Versão Python 3](https://drive.google.com/uc?export=view&id=1zq6YUCBXtRmzShJApmjxTIObJZLW3dI4)

- Caso o Python3 não esteja instalado é só usar o seguinte comando:

````
sudo apt install python3.8 -y
````

## **2º Passo** - Criação de um ambiente virtual para o Jupyter Notebook 

- Instalando a biblioteca VENV

````
sudo apt install python3.8-venv -y  
````

![Instalação VENV](https://drive.google.com/uc?export=view&id=1zrfv_pn2z9H47WgDkvSOdp-F2GDrPAo9)

- Criando o ambiente virtual chamado **‘env’**

````
python3 -m venv env
````

- Ativando o ambiente virtual

````
source env/bin/activate
````

![Ativação ENV](https://drive.google.com/uc?export=view&id=1zrtv0BC3J3tN58eHHx2WMsZYY53M1oCk)

## **3º Passo** - Instalação do gerenciador de pacotes do Python - PIP 

- Instalando o PIP

````
sudo apt install python3-pip -y
````

![Instalação PIP](https://drive.google.com/uc?export=view&id=1zvElZcae23cnbK2qDk5wsw3cyAg5UOR3)

- Atualizando o PIP (Caso ele já estivesse instalado)

````
pip install --upgrade pip 
````

- Listando pacotes/bibliotecas instalados

````
pip list 
````

![PIP List](https://drive.google.com/uc?export=view&id=1zvR_yps2Kgqw2uCvcjRRfOhiTww9aDqL)

- Instalando pacotes (Teste do PIP...)

````
pip install pandas 
````

![Teste PIP...](https://drive.google.com/uc?export=view&id=1zxNNx2fou7DyTlR49Ksw-Bcxfv-tO0w2)

## **4º Passo** - Instalação do Jupyter Notebook

- Instalando o Jupyter no Linux

````
pip install jupyter 
````

![Instalação Jupyter](https://drive.google.com/uc?export=view&id=1zxQK6FcwsKmVwvtfSvZ6rLYqewIq92p5)

- Executando o Jupyter Notebook

````
jupyter notebook
````

![Execução Jupyter Notebook](https://drive.google.com/uc?export=view&id=1zxX2X8rWP91At4ede5JTbkUYczTPPpsa)

>> **Observação:** Após a execução do comando ````jupyter notebook```` vai abrir a IDE pelo navegador que estiver definido com padrão no seu computador, caso ele não abra acesse pela url: [localhost:8888/tree](http://localhost:8888/tree). Lembre-se de sempre ativar o ambiente virtual do Python que você vai executar o Jupyter.  

> **Referências:**  <br/><font size="1">Python.org, **Beginner's Guide to Python.** Disponível em: <https://wiki.python.org/moin/BeginnersGuide>. Acesso em: 12 nov. 2021.  <br/>Python.org, **venv - Criação de ambientes virtuais.** Disponível em: <https://docs.python.org/pt-br/3/library/venv.html>. Acesso em: 12 nov. 2021.  <br/>Python.org, **Instalando Módulos Python.** Disponível em: <https://docs.python.org/pt-br/3/installing/index.html#install-pip-in-versions-of-python-prior-to-python-3-4>. Acesso em: 12 nov. 2021.  <br/>Jupyter, **Installing the classic Jupyter Notebook interface.** Disponível em: <https://jupyter.readthedocs.io/en/latest/install/notebook-classic.html>. Acesso em: 12 nov. 2021.  <br/></font>