# 🎲 Random Number Generator

Este é um pequeno projeto em Python que solicita ao usuário um valor **mínimo** e um valor **máximo**, e então gera um número aleatório dentro desse intervalo.  
O objetivo deste repositório é demonstrar como executar um script **interativo** dentro de um container Docker.

---

## 📥 1. Clonar o repositório

```bash
git clone https://github.com/rafaelalmeidab/docker-core-building.git
```

```bash
cd docker-core-building
```

🐳 2. Requisitos

Antes de rodar o projeto, você precisa ter instalado:

- Docker
- Docker Compose

Verifique:

docker -v
docker compose version

🛠️ 3. Build do projeto
🔧 Build usando Docker Compose

```bash
docker compose build
```

```bash
docker build -t rng .
```

▶️ 4. Executando o script

Como o script é interativo (usa input()), ele não funciona com docker compose up.
Use uma das opções abaixo:

🟩 Opção recomendada: Docker Compose

```bash
docker compose run --rm app
```

📜 5. Licença

Este projeto é apenas um exemplo simples para aprendizado.
Sinta-se à vontade para usar, modificar e compartilhar. 🚀
