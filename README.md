# Boto Guardiao

Um shoot 'em up 2D feito em Godot, onde voce controla um boto que protege o rio contra ondas de poluicao, inimigos aquaticos e chefes cada vez mais perigosos.

Jogue a versao Web:

https://jonnaes.github.io/Boto-Guardiao/

## Sobre o jogo

Em Boto Guardiao, o objetivo e sobreviver as ondas, derrotar inimigos e impedir que a poluicao tome conta do rio. A cada progresso, o jogo ganha novas mecanicas: inimigos com funcoes diferentes, chefes com fases, upgrades permanentes, missoes, combo, placar de lideres e eventos de onda.

## Controles

| Acao | Tecla |
| --- | --- |
| Mover | WASD ou setas |
| Atirar | Espaco ou mouse |
| Dash | Shift |
| Especial | E |
| Pausar | Esc |

## Recursos

- Waves progressivas por capitulos.
- Bosses com barra de vida e padroes por fase.
- Upgrades permanentes estilo roguelike.
- Power-ups temporarios estrategicos.
- Missoes variadas.
- Sistema de combo e score.
- Placar de lideres local.
- Inimigos com papeis claros: rapido, tanque, atirador e perseguidor.
- Perolas de risco/recompensa para ganhar pontos extras.
- HUD customizado com fonte pixelada.
- Musica dinamica em camadas.
- SFX para tiros, impactos, power-ups, boss, poluicao e game over.
- Exportacao Web pronta via GitHub Pages.

## Como jogar localmente pela Web

Depois de exportar o projeto para Web, sirva a pasta `docs` ou `build/web` com um servidor HTTP. Abrir o `index.html` direto no navegador pode nao funcionar.

Exemplo:

```powershell
cd docs
python -m http.server 8000
```

Depois acesse:

```text
http://localhost:8000
```

## Como exportar para Web no Godot

1. Abra o projeto no Godot.
2. Instale os export templates em `Project > Install Export Templates`.
3. Use renderer `Compatibility` para Web.
4. Va em `Project > Export`.
5. Selecione o preset `Web`.
6. Exporte para:

```text
build/web/index.html
```

Para publicar no GitHub Pages, copie os arquivos exportados para `docs/`.

## GitHub Pages

Este repositorio usa a pasta `docs/` como build Web publicado.

Configuracao recomendada:

```text
Settings > Pages
Build and deployment: Deploy from a branch
Branch: main
Folder: /docs
```

## Tecnologias

- Godot 4.6
- GDScript
- Export Web/HTML5

## Estrutura principal

```text
Audio/       SFX e musica
Enemies/     Cenas dos inimigos
Player/      Cena e tiro do player
PowerUps/    Power-ups coletaveis
Sprites/     Artes do jogo
main/        Cena principal
scripts/     Logica do jogo
systems/     Spawner e GameManager
ui/          HUD e menus
docs/        Build Web para GitHub Pages
```

## Status

Projeto em desenvolvimento. A versao Web em `docs/` e a build publicada do jogo.
