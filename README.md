# 🎲 Random Number Generato

Este é um pequeno projeto em Python que solicita ao usuário um valor **mínimo** e um valor **máximo**, e então gera um número aleatório dentro desse intervalo.  
O objetivo deste repositório é demonstrar como executar um script **interativo** dentro de um container Docker.

---

## 📥 1. Clonar o repositório

```bash
git clone https://github.com/rafaelalmeidab/docker-core-building.git
cd docker-core-building

🐳 2. Requisitos

Antes de rodar o projeto, você precisa ter instalado:

Docker

Docker Compose

Verifique:

docker -v
docker compose version

🛠️ 3. Build do projeto
🔧 Build usando Docker Compose
docker compose build

🔧 Build manual (opcional)
docker build -t rng .

▶️ 4. Executando o script

Como o script é interativo (usa input()), ele não funciona com docker compose up.
Use uma das opções abaixo:

🟩 Opção recomendada: Docker Compose
docker compose run --rm app


Você verá:

Please, enter the min number:


Digite os valores e o programa exibirá o número gerado.

🟦 Opção alternativa: Docker manual
docker run -it rng

📁 5. Estrutura do projeto
/
├── rng.py                # Script principal que gera números aleatórios
├── Dockerfile            # Configuração para criar a imagem Python
├── docker-compose.yml    # Facilita execução interativa
└── README.md             # Documentação do projeto

🧠 6. Como o script funciona

O arquivo rng.py faz:

Solicita um número mínimo

Solicita um número máximo

Verifica se o máximo é menor que o mínimo

Se estiver tudo ok, gera um número aleatório usando randint()

Exibe o resultado no terminal

Se o valor máximo for menor que o mínimo, o script exibe:

Invalid input - shutting down...

📜 7. Licença

Este projeto é apenas um exemplo simples para aprendizado.
Sinta-se à vontade para usar, modificar e compartilhar. 🚀
```
