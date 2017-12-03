# Usando a biblioteca Folium

Um projeto simples sobre algumas análises de utilizando a biblioteca [Folium]().

## Instalação

### Docker 🐳

Instale o [docker](https://docs.docker.com/engine/installation/) e o [docker-compose](https://docs.docker.com/compose/install/). Depois disso é só rodar:

_Pode ser que esse comando demore um pouco na primeira vez_
```console
$ docker-compose up
```

### Sem docker

#### Preparando o ambiente

Aqui eu uso [virtualenv](). Caso não queira seguir com um ambiente virtual pule para a seção "Instalando" logo abaixo.

```console
$ pip3 install virtualenv
$ virtualenv .env --python=python3
$ source .env/bin/activate
```
_O comando de ativação pode variar de acordo com o sistema operacional. O comando acima é para OS X ;)_

#### Instalando
```console
(.env) $ cd intro-folium/
(.env) $ pip install -r requirements.txt
(.env) $ pip install jupyter
```

## Dados

No notebook vou usar os dados de geolocalização de empresas no Brasil. O arquivo original,  gerado pelo Serenata, pode ser baixado pelo `serenata-toolbox` e instruções sobre como fazer isso podem ser encontradas [aqui](https://github.com/datasciencebr/serenata-toolbox/blob/master/README.rst#usage).

## Arquivos

- `prepacao-de-dados.ipynb`: Apenas um registro de como o dataset foi feito
- `folium.ipynb`: Análise usando a biblioteca folium
- `mapas/`: Diretório com os mapas resultantes da análise
- `empresas.xz`: Arquivo `.csv` comprimido com dados de empresas
