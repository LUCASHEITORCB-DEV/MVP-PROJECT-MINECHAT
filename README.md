# MINECHAT - Jogo Interativo via Chat do YouTube

![Banner MINECHAT](caminho/para/banner.png) <!-- Adicione um banner se disponível -->

**MINECHAT** é um jogo interativo transmitido ao vivo no YouTube em formato vertical, onde jogadores controlam criaturas estilo Minecraft através de comandos no chat. Desenvolvido como um MVP, o projeto visa evoluir para um RPG completo com monetização e progressão.

## 🚀 Visão Geral

Um jogo de batalha 1v1 em tempo real, onde:
- **Jogadores** usam comandos como `!join`, `!attack`, e `!item` para participar.
- **Criaturas** têm habilidades únicas, sistemas de defesa e ataques especiais.
- **Interface** é exibida diretamente na live (1080x1920) com HUD dinâmico.

## ✨ Funcionalidades

### 🎮 Sistema de Batalha
- Comandos: `!join`, `!ready`, `!attack (1-4)`, `!item`, `!bet` (50% de chance de vitória/derrota).
- **Criaturas Iniciais**: Zumbi, Esqueleto, Pé Grande, Olho Mágico, Homem Quadrado (Minecraft).
- **Mecânicas**:
  - Ataques com crítico e efeito "Appart" (0.5% de hit kill).
  - Defesa reduz dano em 25%-75%.
  - Bots entram após 4:40 sem interação.

### 📊 Progressão
- Ranking e histórico salvos em JSON.
- **Site Integrado** (Futuro): Login, loja, inventário e histórico de partidas.

### 💰 Monetização (MVP Futuro)
- Skins cosméticas e funcionais via lootboxes.
- Moedas compráveis via PIX/gateways.
- Integração com LivePix para doações.

## 🛠️ Tecnologias

```plaintext
Backend: Python (Pygame para renderização)
API: YouTube Data v3 (leitura do chat)
Transmissão: OBS Studio
Banco de Dados: SQLite (MVP) → Firebase/PostgreSQL (Futuro)
Frontend Web: HTML/CSS/JS + Flask/React
