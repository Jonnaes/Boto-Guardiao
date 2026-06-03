# Boto Guardião

Um shoot 'em up 2D desenvolvido na Godot, onde você controla um boto que protege o rio contra ondas de poluição, inimigos aquáticos e chefes cada vez mais perigosos.

[Jogue a versão Web AQUI](https://joaolorena0.github.io/Boto-Guardiao/)


## Sobre o Jogo

Em Boto Guardião, o objetivo é sobreviver às ondas, derrotar inimigos e impedir que a poluição tome conta do rio. A cada progresso, o jogo ganha novas mecânicas: inimigos com funções diferentes, chefes com fases, upgrades permanentes, missões, sistema de combo, placar de líderes e eventos de onda.

## Controles

Ação       | Tecla
---------- | ------------------
Mover      | WASD ou setas
Atirar     | Espaço ou mouse
Dash       | Shift
Especial   | E
Pausar     | Esc

## Recursos

- Ondas (waves) progressivas por capítulos.
- Chefes (bosses) com barra de vida e padrões por fase.
- Upgrades permanentes estilo roguelike.
- Power-ups temporários estratégicos.
- Missões variadas.
- Sistema de combo e score.
- Placar de líderes local.
- Inimigos com papéis claros: rápido, tanque, atirador e perseguidor.
- Pérolas de risco/recompensa para ganhar pontos extras.
- HUD customizado com fonte pixelada.
- Música dinâmica em camadas.
- SFX para tiros, impactos, power-ups, boss, poluição e game over.
- Exportação Web pronta via GitHub Pages.

## Como Jogar Localmente pela Web

Depois de exportar o projeto para Web, sirva a pasta `docs` ou `build/web` com um servidor HTTP. Abrir o `index.html` direto no navegador pode não funcionar.

Exemplo:
cd docs
python -m http.server 8000

Depois acesse:
http://localhost:8000

## Tecnologias

- Godot 4.x
- GDScript
- Export Web/HTML5

## Estrutura Principal

Audio/       SFX e música
Enemies/     Cenas dos inimigos
Player/      Cena e tiro do player
PowerUps/    Power-ups coletáveis
Sprites/     Artes do jogo
main/        Cena principal
scripts/     Lógica do jogo
systems/     Spawner e GameManager
ui/          HUD e menus
docs/        Build Web para GitHub Pages
