# NAT e PAT

## 🌐 O que é NAT?

**NAT (Network Address Translation)** é um mecanismo que permite que dispositivos com **endereços IP privados** comuniquem com a internet, que usa **endereços IP públicos**.

- Traduz endereços IP **privados → públicos**
- Muito usado em routers domésticos e empresariais
- Ajuda a **poupar endereços IPv4** e a **ocultar redes internas**

### 🧠 Exemplo:

> Um computador com IP `192.168.1.10` envia um pedido para a internet.  
> O router substitui esse IP por `81.84.23.5` (IP público) usando NAT.

---

## 🔄 Tipos de NAT

| Tipo de NAT         | Explicação breve                                  |
|---------------------|---------------------------------------------------|
| **Static NAT**       | 1 IP privado → 1 IP público (ligação fixa)        |
| **Dynamic NAT**      | IP privado → IP público de um grupo disponível    |
| **PAT (Port Address Translation)** | Traduz **vários IPs privados** para **um único IP público**, diferenciando pelas **portas** |

---

## 🔁 O que é PAT?

**PAT** é uma forma de NAT também conhecida como **NAT Overload**.

- Permite que **múltiplos dispositivos privados usem o mesmo IP público**
- Usa diferentes **números de porta** para manter as ligações distintas

### 🧠 Exemplo:

| Dispositivo | IP Privado      | IP Público + Porta Traduzida         |
|-------------|------------------|--------------------------------------|
| PC 1        | 192.168.0.2:1025 | 81.84.23.5:30001                     |
| PC 2        | 192.168.0.3:1026 | 81.84.23.5:30002                     |

---

## ✅ Vantagens do NAT/PAT

- **Reduz o consumo de endereços IPv4 públicos**
- **Aumenta a segurança** ao ocultar a rede interna
- Facilita a partilha da ligação à internet

---

## ⚠️ Limitações

- Pode dificultar **ligações de entrada** (ex: hosting de servidores locais)
- Pode interferir com protocolos que não suportam NAT (ex: alguns jogos ou VoIP)

---

## 🔚 Em resumo

- **NAT** traduz IPs privados para públicos
- **PAT** traduz múltiplos IPs privados usando **um só IP público**, diferenciando pelas **portas**
