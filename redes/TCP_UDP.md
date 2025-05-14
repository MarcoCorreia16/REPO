# Resumo: TCP vs UDP

## TCP – Transmission Control Protocol

- **Orientado à ligação (connection-oriented)**: é estabelecida uma ligação antes de transmitir dados.
- **Fiável**: garante que os dados chegam ao destino e na ordem correta.
- **Controlo de erros e reenvio**: deteta perdas e reenvia pacotes.
- **Mais lento**, devido ao controlo adicional.
- Usado quando a **fiabilidade é essencial**, como em:
  - Web (HTTP/HTTPS)
  - Email (SMTP, IMAP)
  - Transferência de ficheiros (FTP)

### Vantagens:
- Garante entrega completa e ordenada
- Gestão automática de congestionamento

### Desvantagens:
- Overhead maior  (custos adicionais que não fazem parte dos dados úteis que queremos transmitir ou processar)
- Mais lento que UDP

---

## UDP – User Datagram Protocol

- **Sem ligação (connectionless)**: envia os dados sem negociar ligação.
- **Não fiável**: não há garantias de entrega ou ordem correta.
- **Sem controlo de erros nem reenvio automático**.
- **Mais rápido**, ideal para situações em que a velocidade é mais importante que a fiabilidade.
- Usado em:
  - Streaming de vídeo/áudio
  - Jogos online
  - DNS
  - VoIP

### Vantagens:
- Muito rápido
- Ideal para tempo real

### Desvantagens:
- Pode perder dados
- Não garante ordem nem entrega

---

## 🧠 Resumo final

| Característica | TCP                        | UDP                     |
|----------------|-----------------------------|--------------------------|
| Ligação        | Sim                         | Não                     |
| Fiabilidade    | Elevada                     | Baixa                   |
| Velocidade     | Mais lento                  | Mais rápido             |
| Uso típico     | Web, email, ficheiros       | Streaming, jogos, DNS   |
