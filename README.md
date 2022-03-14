# Docker-Nginx-Site
Exemplo de criação de imagem Docker com Nginx

# Dependências

- Docker

# Desenvolvimento

Feito o clone somente executar na raíz do projeto o seguinte:

- Executando o comando abaixo será gerada a imagem chamada webapi

    ```
    docker build -t web-site-static .
    ```

- O próximo passo será executar o container com o comando:

    ```
    docker run -d -p 8080:80 web-site-static
    ```

    O docker subirá a aplicação na porta 80 interna do container e deixará exposta na porta 8080 do host. Comando -d é passado para não deixar o terminal travado com a execução.

- Agora é só verificar o endpoint para observar a aplicação executando, pode ser utilizado alguma aplicação como Postman ou mesmo via navegador.

    ```
    http://localhost:8080/index.html
    ```

