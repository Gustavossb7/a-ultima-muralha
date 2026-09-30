# 🧙 A Última Muralha

Um jogo de sobrevivência contra hordas de inimigos, com temática medieval, inspirado em jogos do estilo *survivor-like* (na linha de *Vampire Survivors* / *Seraph's the Last...*). Você controla um arquimago que precisa resistir ao maior número possível de rodadas contra hordas de esqueletos, morcegos, cavaleiros, arqueiros, ogros e chefes poderosos.

Jogo feito em **HTML5 + Canvas + JavaScript puro**, sem dependências externas, rodando inteiramente no navegador.

## 🎮 Como jogar

Abra o arquivo `ultima-muralha.html` em qualquer navegador moderno (desktop ou mobile).

### Controles (Desktop)
| Ação | Tecla |
|---|---|
| Mover | `W A S D` ou setas |
| Mirar | Mouse |
| Atirar | Clique esquerdo |
| Nova Arcana (explosão em área) | `Espaço` ou clique direito |
| Passo Sombrio (dash com invulnerabilidade) | `Shift` |
| Disparo automático | `F` |
| Pausar | `P` ou `Esc` |
| Mudo | `M` |

### Controles (Mobile)
Jogue na horizontal. Arraste no lado esquerdo da tela para mover (joystick virtual). A mira e o disparo contra o inimigo mais próximo são automáticos. Botões na tela para Nova Arcana e Dash.

## 🧟 Mecânicas principais

- **Ondas de inimigos:** esqueletos, morcegos, cavaleiros, arqueiros e ogros, cada um com comportamento e sprite próprios, desenhados via Canvas 2D.
- **Progressão por rodadas:** ao fim de cada rodada, o jogador escolhe 1 entre 3 poderes (dano, cadência, projéteis extras, perfuração, explosão em área, crítico, vida, regeneração, cura, velocidade, etc.), com upgrades acumulativos e níveis.
- **Chefes a cada 5 rodadas:** Rei Esqueleto, Cavaleiro Negro, Lich Sombrio e Dragão Ancião, cada um com padrões de ataque próprios (investida, pancada em área, leque de projéteis, anel de projéteis, invocação de aliados, teletransporte) com avisos visuais (telegraphing).
- **Poderes lendários:** dropados exclusivamente por chefes — Chuva de Meteoros, Aura Gélida, Relâmpago em Cadeia, Pena da Fênix (ressurreição), Orbes Arcanos, Pacto Arcano e Barreira Rúnica.
- **Recorde persistente:** pontuação e melhor rodada salvas via `localStorage`.
- **Áudio procedural:** todos os efeitos sonoros são gerados via Web Audio API (osciladores), sem arquivos de áudio externos.

## 🛠️ Tecnologia

- Um único arquivo HTML autocontido (`ultima-muralha.html`)
- Canvas 2D para renderização (sprites desenhados via código, sem imagens externas)
- Web Audio API para efeitos sonoros
- `localStorage` para salvar recorde
- Suporte a mouse, teclado e touch (mobile)
- Sem frameworks, sem build step, sem dependências — basta abrir no navegador

## 📂 Estrutura

```
.
├── ultima-muralha.html   # jogo completo (HTML + CSS + JS em um único arquivo)
└── README.md
```

## 🚀 Rodando localmente

Não é necessário servidor nem instalação. Basta baixar o arquivo e abrir direto no navegador:

```bash
git clone <url-do-repositorio>
cd <repositorio>
# abra ultima-muralha.html no navegador
```

Ou, se preferir servir localmente:

```bash
python3 -m http.server 8000
# acesse http://localhost:8000/ultima-muralha.html
```

## 📌 Possíveis melhorias futuras

- Novos tipos de inimigos e chefes
- Ajustes de curva de dificuldade
- Novas skins/visuais para o mago
- Modo cooperativo local

## 📄 Licença

Defina a licença do projeto aqui (ex.: MIT).
