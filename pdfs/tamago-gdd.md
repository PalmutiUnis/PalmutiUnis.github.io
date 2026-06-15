# Game Design Document — TamaGO

> **TamaGO** — Um Tamagotchi RPG clássico com mecânicas modernas, rodando direto no terminal.

| Campo | Valor |
|---|---|
| **Título** | TamaGO |
| **Versão do documento** | v1.25 |
| **Equipe** | TamaGO |
| **Plataforma** | PC / Terminal (TUI) |
| **Engine / Stack** | Go + Bubble Tea + Lipgloss |
| **Gêneros** | RPG, Simulação, Casual, TUI, Sandbox |
| **Modo** | Single-player, Offline-First |
| **Classificação** | Livre |
| **Preço** | Gratuito / Open Source |
| **Repositório** | https://github.com/DeMart1n/Tamagotchi |

---

## 1. Visão Geral (High Concept)

**TamaGO** une a nostalgia dos clássicos pets virtuais (Tamagotchi) com mecânicas
de RPG tático moderno, tudo dentro de uma interface de terminal (TUI). O jogador
precisa manter seu pet alimentado, hidratado e feliz enquanto explora masmorras
perigosas. Cada ação direta impacta a complexa árvore de evolução biológica do
personagem.

Derrote inimigos, colete artefatos e gerencie recursos vitais em um ecossistema
CLI dinâmico de estratégia em tempo real.

### Pilares de Design

1. **Nostalgia + Profundidade** — a simplicidade do pet virtual combinada com a
   estratégia de um RPG por turnos.
2. **Tempo real importa** — o descuido com os recursos vitais tem consequências
   (Game Over).
3. **Progressão significativa** — evolução biológica, níveis e equipamentos que
   recompensam o investimento do jogador.
4. **Terminal-first** — experiência completa e elegante via texto, cores ANSI e
   Unicode.

---

## 2. Público-Alvo

- Jogadores nostálgicos dos pets virtuais clássicos.
- Fãs de RPGs táticos por turnos e roguelikes.
- Usuários de terminal / desenvolvedores que apreciam ferramentas TUI.
- Classificação **Livre**: sem conteúdo violento explícito, linguagem apropriada
  para todas as idades.

---

## 3. Mecânicas Core

### 3.1. Pet Virtual e Sobrevivência

Controle em tempo real dos recursos vitais do pet:

- **Fome**
- **Sede**
- **Energia**
- **Felicidade**
- **Calma**

O descaso com qualquer um desses recursos pode levar ao **Game Over**. O jogador
deve equilibrar o cuidado com o pet e a exploração das masmorras.

### 3.2. Evoluções e Níveis

- **5 Estágios de vida**: do estágio *Baby* até o status de *Ancião*.
- **25 níveis** de progressão escalável por árvore de XP.
- Cada ação impacta a árvore de evolução biológica do personagem.

### 3.3. Dungeon RPG Tática

- Masmorra de **5 andares**, liberada ao alcançar o **Nível 3**.
- **9 tipos de inimigos** diferentes.
- Combate **tático por turnos**.

### 3.4. Biomas Dinâmicos

4 zonas distintas, cada uma com modificadores ambientais e loots exclusivos:

| Bioma | Tema |
|---|---|
| Florestal | Zona inicial / equilibrada |
| Gélida | Frio e modificadores de energia |
| Vulcânica | Calor e perigo elevado |
| Abissal | Profundezas / maior dificuldade |

---

## 4. Sistemas e Conteúdo

| Sistema | Conteúdo |
|---|---|
| **Armamento e Itens** | 12 equipamentos únicos em 3 slots (até raridade Lendário) |
| **Conquistas** | 15 achievements integrados ao core do jogo |
| **Salvamento** | Persistência local e automática (Save/Load) via TUI |
| **Interface** | Construída em Go usando Bubble Tea e Lipgloss |

---

## 5. Loop de Jogo (Gameplay Loop)

1. **Cuidar do pet** — gerenciar Fome, Sede, Energia, Felicidade e Calma.
2. **Ganhar XP e evoluir** — subir de nível e avançar pelos estágios de vida.
3. **Explorar masmorras** (a partir do Lvl 3) — enfrentar inimigos em combate por
   turnos nos 4 biomas.
4. **Coletar loot** — equipamentos e artefatos exclusivos por bioma.
5. **Progredir** — desbloquear conquistas e fortalecer o pet, mantendo sempre os
   recursos vitais equilibrados.

O ciclo se repete com dificuldade e recompensas crescentes conforme o pet evolui.

---

## 6. Interface (UI/UX)

- Interface 100% baseada em **texto e comandos táticos** (TUI).
- Visualização de status e comandos diretamente pelo terminal.
- Estética retrô de terminal (fósforo verde / cores ANSI).
- Construída com **Bubble Tea** (arquitetura Elm-like) e **Lipgloss** (estilização).

---

## 7. Requisitos de Sistema

### Mínimos

| Item | Especificação |
|---|---|
| SO | Windows 10+ / macOS 10.14+ / Linux |
| CPU | Dual-Core 2.0 GHz (Intel i3 ou equiv.) |
| RAM | 512 MB |
| Espaço | 50 MB |
| Console | Suporte a Unicode e cores ANSI |

### Recomendados

| Item | Especificação |
|---|---|
| SO | Windows 11 / macOS 12+ / Linux atual |
| CPU | Quad-Core (Intel i5+ / Ryzen 5+) |
| RAM | 2 GB |
| Espaço | 100 MB SSD |
| Rede | Offline (features futuras opcionais) |

---

## 8. Especificações Técnicas

- **Linguagem:** Go
- **Framework de UI:** Bubble Tea (TUI)
- **Estilização:** Lipgloss
- **Distribuição:** Single-player, Offline-First, executável de terminal (PC)
- **Persistência:** Save/Load local automático

---

## 9. Equipe de Desenvolvimento

- Cauã De Martin
- Luiz Felipe Arcanjo Rangel
- Jean da Silva Lopes
- Luis Filipe Alves

---

## 10. Classificação Indicativa

**LIVRE** — Sem conteúdo violento explícito. Linguagem totalmente apropriada para
todas as idades.

---

*Documento gerado para a Mostra de Games Acadêmica — UNIS.*
