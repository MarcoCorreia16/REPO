# Protocolo HTTP (HyperText Transfer Protocol)

O HTTP é o protocolo de comunicação utilizado para transferir páginas web e outros conteúdos entre clientes (ex: navegadores) e servidores web.

---

## 🧱 Características principais

- **Protocolo de texto**: as mensagens são legíveis por humanos.
- **Sem estado (stateless)**: cada pedido é independente, sem memória de pedidos anteriores.
- **Usa o protocolo TCP**, geralmente na porta **80** (ou 443 no caso de HTTPS).
- Utiliza métodos para definir o tipo de ação a realizar.

---

## 📥 Métodos HTTP mais comuns

| Método  | Função                                  |
|---------|------------------------------------------|
| `GET`   | Solicita dados (ex: uma página HTML)     |
| `POST`  | Envia dados ao servidor (ex: formulários)|
| `PUT`   | Atualiza ou cria um recurso              |
| `DELETE`| Remove um recurso                        |
| `HEAD`  | Igual ao GET, mas sem o corpo da resposta|

---

## 🔐 HTTP vs HTTPS

| Característica     | HTTP             | HTTPS                      |
|--------------------|------------------|-----------------------------|
| Porta padrão       | 80               | 443                         |
| Segurança          | ❌ Nenhuma       | ✅ Encriptação com TLS/SSL  |
| Certificado digital| ❌ Não usa       | ✅ Requer certificado válido|

O HTTPS é essencial para proteger dados sensíveis (ex: passwords, cartões de crédito).

---

## 🧪 Exemplo de pedido HTTP

```http
GET /index.html HTTP/1.1
Host: www.exemplo.com
User-Agent: Mozilla/5.0
