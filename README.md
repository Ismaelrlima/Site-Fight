# Fight House FSA

Site estático completo da Fight House FSA. Imagens, estilos, scripts e ícones Lucide estão incluídos no pacote.

## Arquivos

- `dist/`: site pronto para servir, incluindo HTML, CSS, JavaScript, ícones e imagens.
- `Dockerfile`: imagem Nginx com os arquivos do site.
- `nginx.conf`: configuração do servidor web.
- `docker-compose.yml`: serviço e mapeamento de porta.
- `LUCIDE-LICENSE`: licença da biblioteca de ícones incluída.

## Rodar com Docker

No diretório do projeto, execute:

```bash
docker compose up -d --build
```

Abra `http://IP_DO_SERVIDOR:8080`. A porta externa padrão é `8080`.

Para usar outra porta:

```bash
PORT=3000 docker compose up -d --build
```

Para atualizar o site depois de copiar os novos arquivos ao servidor, execute novamente `docker compose up -d --build`. O site não precisa de Node.js, banco de dados nem variáveis de ambiente.
