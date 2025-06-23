# MVP-PROJECT-MINECHAT

1. Visão Geral do Projeto
MINECHAT é um projeto de jogo online interativo que ocorre ao vivo no YouTube em formato vertical. Utilizando comandos do chat, os jogadores podem participar de batalhas 1x1 controlando criaturas em tempo real. O público-alvo é formado por crianças e adolescentes que consomem conteúdo de streaming e jogos como Pokémon ou RPG. O jogo foi criado como MVP para futura expansão em um jogo estilo RPG completo com monetização e progressão.

3. Funcionalidades do Sistema
- Entrada via comando `!Join` sorteando jogadores automaticamente.
- Comandos para controlar a batalha (`!Ready`, `!atack`, `!item`, `!escape`, `!bet`).
- Cada criatura possui 4 ataques únicos com possibilidade de crítico e efeito 'Appart' (hit kill 0.5%).
- Itens ilimitados: buffs, cura e suporte.
- Sistema de defesa das criaturas reduz dano de 25% a 75%.
- Bots entram automaticamente após 4:40 min sem interação no chat.
- Ranking e histórico salvos em arquivos JSON periodicamente.
- Tela responsiva com HUD dividida e nomes acima das criaturas.
- Site com login, loja, inventário, ranking e histórico de partidas.

3. Interface Visual na Live
A interface principal exibida na live é dividida verticalmente (1080x1920):
- Jogador 1 à esquerda, Jogador 2 à direita.
- Nome dos jogadores exibido acima das criaturas.
- Barra de vida animada.
- Comandos visíveis no topo da tela.
- Ranking visível em uma das extremidades inferiores.
- 
4. Lógica e Regras de Batalha
- Cada batalha dura no máximo 2 minutos ou até um dos jogadores perder todo o HP.
- Se o jogador não digitar `!Ready` em 20 segundos, é substituído.
- Comando `!bet` tem 50% de chance de matar ou morrer instantaneamente.
- Cada criatura possui 4 ataques únicos com variações de dano, crítico e habilidades.
- O ataque 1 possui chance de crítico e chance de hit kill chamada 'Appart'.
- Sistema de defesa aplicado à criatura reduz dano com base no tipo.
- 
5. Criaturas Iniciais
    • Zumbi
    • Esqueleto
    • Pé grande
    • Olho mágico flutuante
    • Homem quadrado estilo Minecraft
  
6. Comandos Disponíveis
    • `!Join` – entra na fila e sorteio
    • `!Ready` – confirma prontidão para batalha
    • `!atack` – ataque padrão
    • `!atack (1-4)` – ataque específico
    • `!ataque aleatorio` – sorteia ataque da criatura
    • `!item (1-4)` – usa item
    • `!escape` – desiste da batalha
    • `!bet` – aposta tudo (50% de chance de matar ou morrer)

7. Monetização
- Jogadores compram moedas no site oficial via PIX ou gateways de pagamento.
- Com as moedas, compram skins (cosméticas e com habilidades), itens e ataques especiais.
- Skins são obtidas via lootboxes e influenciam no visual e nas habilidades da criatura.
- Planeja-se LivePix como forma de apoiar diretamente durante as transmissões.
- 
8. Funcionalidades do Site
- Sistema de login e cadastro.
- Escolha de criatura e ataques.
- Loja virtual para comprar moedas, itens e skins.
- Inventário do jogador com itens e personalizações.
- Visualização de ranking e histórico de partidas.
- 
9. Stack Tecnológica
    • Python para backend e lógica do jogo
    • Pygame para renderização vertical (1080x1920)
    • API YouTube Data v3 para leitura do chat
    • OBS Studio para transmissão da live
    • Banco de dados: SQLite, PostgreSQL ou Firebase
    • Frontend web: HTML/CSS/JS, Flask, React ou Next.js
  
10. Armazenamento e Backup
O histórico de batalhas, dados de jogadores, skins e ranking serão armazenados em arquivos JSON durante o MVP. Posteriormente, será migrado para um banco de dados mais robusto com backups automáticos.

12. Equipe e Estrutura Organizacional
Lucas Heitor é o fundador, líder técnico, designer, gerente e coordenador de equipe. Atualmente, o projeto conta com 3 membros, com previsão de expansão conforme o MVP avance e traga resultados.

14. Visão Futura: Jogo RPG Completo
O MINECHAT servirá como base para um jogo completo RPG com mundo aberto, criaturas evolutivas, inventário persistente, sistema de progressão, loja integrada e campanhas. O jogo será multiplataforma, podendo rodar na web, desktop ou até dispositivos móveis.
