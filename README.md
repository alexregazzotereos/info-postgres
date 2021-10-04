# Instalação do Postgres sem acesso admin

Fonte: `https://www.geeksforgeeks.org/postgresql-installing-postgresql-without-admin-rights-on-windows/`

## Configurações únicas
1. [Acesse o site](https://www.enterprisedb.com/download-postgresql-binaries) e faça o download do binaries do postgres da versão 13.4 para windows
   
2. Extraia a pasta e coloque-a em um luga para ficar fixa, por exemplo: C:\Users\SEUUSUARIO\
3. Execute no terminal o comando:   `"C:\Users\SEUUSUARIO\pgsql\bin\initdb" -D "C:\Users\SEUUSUARIO\pgsql\data" -U postgres -E utf8`

## Inicialização do banco (toda vez que for usar depois de fechar terminal/reiniciar computador)
1. Execute no terminal o comando: `"C:\Users\SEUUSUARIO\pgsql\bin\pg_ctl" -D "C:\Users\SEUUSUARIO\pgsql\data" start`
2. Manter o terminal aberto enquanto utiliza o banco

### Conexão com banco (dbeaver)
    host: localhost
    port: 5432
    database: postgres
    user: postgres
    senha: 

# Abrir terminal
1. Aperte `WIN+R`
2. Digite `cmd`
3. Pressione `enter`
