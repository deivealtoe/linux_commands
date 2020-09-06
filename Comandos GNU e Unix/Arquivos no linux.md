Podemos criar um arquivo usando o 'touch'. Com ele podemos criar diversos arquivos de uma só vez, separando-os com espaço ' '
```
$ touch arquivo_1.txt arquivo_2.log etc
```

Arquivos e pastas ocultas no linux tem como primeiro caractere em seu nome o .
```
$ touch .oculto.txt
```


Para listar todas as partições montadas
```
$ mount
```

Uma opção mais clean ao 'mount' é o
```
$ findmnt
```


Listar todas as partições do sistema
```
$ df -h
```

Observando tamanho de arquivo e/ou diretórios
```
$ du
$ du -h
$ du -hs
$ du -hs /home
```
