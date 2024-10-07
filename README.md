# PACOTES

Um pacote é um programa que faz alguma tarefa para o computador.

Programas são importantes para que o computador tenha funcionalidades.

Programas podem servir para jogar, estudar, programar e etc...

## Dependências

Todo o pacote pode depender de outros pacotes para funcionar. Esses pacotes recebem o nome de dependências.

Vamos supor que você quer instalar o programaA, e durante a instalação, um erro é retornado, pois o programaA depende do programaB para funcionar. Então, você baixa o programaB, e realiza a instalação, só que o programaB depende dos programasC e programaX para funcionar, e assim sucessivamente. 

Os programas B,C,X são as dependências do programaA. Dependendo do gerenciador de pacotes, você terá que instalar cada um dos pacotes na mão ou poderá simplesmente instalar o pacote, e o gerenciador de pacotes fará a instalação do pacote e de suas dependências.

## Gerenciador de pacotes

O gerenciador de pacotes é uma ferramenta responsável por pesquisar, listar, atualizar, instalar, remover, dar manutenção, mostrar informações e entre outros sobre pacotes.

### Debian

No debian existem os gerenciadores apt-get e dpkg

#### dpkg

dpkg é um gerenciador de pacotes não versátil. Isso significa que, se um programa for instalado e ele tiver dependências, o dpkg não vai instalar automaticamente as dependências. Isso significa que você vai ter que baixar e instalar as dependências uma por uma.

Para instalar um pacote usando o dpkg, você vai usar o comando:

```bash
dpkg -i pacote
```

Você também pode fazer da seguinte maneira:

```bash
dpkg --install pacote
```

#### apt-get

O apt-get é um gerenciador de pacotes versátil. Isso significa que ele instala o pacote e suas dependências automaticamente. A versatilidade do apt-get é composta de vários elementos, sendo um deles a lista de repositório debian/ubuntu e seus derivados, que é de onde o apt-get puxa, lista, baixa e atualiza os pacotes.

Para instalar um pacote no apt-get, basta:

```bash
apt-get install pacote
```
