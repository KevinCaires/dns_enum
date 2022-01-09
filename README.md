# DNS ENUM

## Instalação

É necessário ter o python3 instalado.

Depois de clonar o repositório basta entrar na pasta e instalar com o setup.

    python3 setup.py install

    ou
    
    ./setup.py install

## Comandos

 Argumento | Alias | Descrição 
-----------|-------|------------
 domain    | | Argumento posicional obrigatório contendo o nome do dominio. Ex: `google.com`.
 --word_list | -wl | Argumento opcional, correspondente com o caminho + nome de uma lista de protocolos de rede. Ex: `www, ftp, ns1, ...`.
 --threads_nuber | -tn | Quantidade de threads que devem ser executadas na busca.
 --processes_number | -pn | Quantidade de processos que devem ser executados na busca. Essa opção usa multiprocessing, recomendo que se usar essa opção seja passado no argumento, no máximo, a mesma quantidade de núcleos do seu processador, visando não travar seu sistema.

_________________

Exemplo de uso 1:
    
    ./dns_enum google.com

Exemplo de uso 2:

    ./dns_enum google.com --word_list /home/jon/my_word_list.txt

Exemplo de uso 3:

    ./dns_enum google.com -threads_number 500
