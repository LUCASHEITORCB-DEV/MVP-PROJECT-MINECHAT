MINECHAT - Documentação do Projeto
📌 Visão Geral
O MINECHAT é um jogo interativo transmitido ao vivo no YouTube em formato vertical, onde jogadores controlam criaturas inspiradas em Minecraft usando comandos do chat. O público-alvo são crianças e adolescentes fãs de streaming, Pokémon e RPG.

Este MVP servirá como base para um futuro RPG completo com monetização, progressão e multiplataforma.

🎮 Funcionalidades Principais
⚡ Sistema de Batalha
Comandos do Chat:

!Join – Entra na fila para batalha.

!Ready – Confirma prontidão.

!atack (1-4) – Executa um ataque específico.

!item (1-4) – Usa um item (cura, buff, etc.).

!bet – Aposta tudo (50% de chance de vitória ou derrota instantânea).

Criaturas com habilidades únicas (4 ataques cada, incluindo críticos e efeito Appart – hit kill 0,5%).

Sistema de defesa (reduz dano em 25% a 75%).

Bots automáticos entram após 4:40 min sem interação.

📊 Progressão e Ranking
Ranking e histórico salvos em JSON.

Tela de transmissão com HUD (barra de vida, nomes, comandos visíveis).

💰 Monetização (Futuro)
Loja virtual com skins, itens e lootboxes.

Moedas compráveis via PIX/gateways.

LivePix para doações diretas.

🎨 Interface na Live
Formato vertical (1080x1920).

Jogador 1 (esquerda) vs. Jogador 2 (direita).

Barras de vida animadas.

Ranking exibido na parte inferior.

🛠️ Stack Tecnológica
Área	Tecnologias
Backend	Python (lógica do jogo)
Renderização	Pygame (tela vertical)
Chat	YouTube Data API v3
Transmissão	OBS Studio
Banco de Dados	SQLite (MVP) → Firebase/PostgreSQL (futuro)
Frontend Web	HTML/CSS/JS, Flask/React/Next.js
📂 Armazenamento
MVP: Dados salvos em JSON (histórico, ranking).

Futuro: Migração para banco de dados (Firebase/PostgreSQL) com backups.

🚀 Visão Futura
Jogo RPG completo com:

Mundo aberto.

Criaturas evolutivas.

Progressão persistente.

Multiplataforma (web, desktop, mobile).
