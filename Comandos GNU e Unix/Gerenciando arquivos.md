#### Para criarmos arquivos, precisamos da permissão de escrita na pasta

Podemos criar um arquivo usando o 'touch'. Com ele podemos criar diversos arquivos de uma só vez, separando-os com espaço
```
$ touch arquivo_1.txt arquivo_2.log etc
```

Arquivos e pastas ocultas no linux tem como primeiro caractere em seu nome o .
```
$ touch .oculto.txt
```

Para criarmos uma pasta, cada nova pasta separada por um espaço
```
$ mkdir primeiroDiretorio
$ mkdir nome_da_pasta nome_do_outro_diretorio
$ mkdir /home/$USER/nova_pasta
```

Removendo um diretório
```
$ rm nome_da_pasta
$ rm nome_da_pasta -r # apagar recursivamente
$ rm nome_da_pasta -rf # apagar recursivamente e forçar
```

Listando arquivos e outros diretórios
```
$ ls
$ ls -l
$ ls -la
$ ls -lah
```

Com um link simbólico, podemos encurtar o caminho de uma pasta. Podemos excluir diretórios simbólicos da mesma forma que os normais
```
$ ln -s diretorio diretorio_simbolico
```

Para compactar, visualizar ou extrair um diretório ou arquivo, podemos utilizar o 'tar', com os seguintes parâmetros
```
$ tar -czvf BKP_HOME.tar.gz /home # para compactar com tar e comprimir com gzip -> leia-se: C = criar / Z = com gzip / V = no modo verbose / F = o arquivo BKP_HOME.tar.gz a pasta /home
$ tar -tzvf BKP_HOME.tar.gz # para visualizar com tar e gzip -> leia-se: T = visualizar / Z = com gzip / V = no modo verbose / F = o arquivo BKP_HOME.tar.gz
$ tar -xzvf BKP_HOME.tar.gz -C /teste # para extrair os arquivos compactados e comprimidos -> leia-se: X = extrair / Z = com gzip / V = no modo verbose / F = o arquivo BKP_HOME.tar.gz na pasta /teste
```
