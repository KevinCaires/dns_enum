# DNS ENUM

## Comandos

 Argumento | Alias | Descrição 
-----------|-------|------------
 domain    |   X   | Argumento posicional obrigatório contendo o nome do dominio. Ex: `google.com`.
 --word_list | -wl | Argumento opcional, correspondente com o caminho + nome de uma lista de protocolos de rede. Ex: `www, ftp, ns1, ...`.

_________________

Exemplo de uso 1:
    
    ./dns_enum google.com

Exemplo de uso 2:

    ./dns_enum google.com --word_list /home/jon/my_word_list.txt