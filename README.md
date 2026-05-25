# 🎮 Portal de Jogos Acadêmicos - Atividade Prática

Bem-vindos ao repositório oficial do nosso portal de jogos! Este repositório (hospedado em `https://github.com/PalmutiUnis/PalmutiUnis.github.io`) será a nossa vitrine oficial para o evento de exibição de jogos marcado para o dia **22 de Junho**.

O objetivo desta atividade é atualizar o portal com os dados reais dos projetos de cada equipe, estabelecer a página de venda (Store Page) em formato web e garantir que a documentação principal do seu jogo (GDD) esteja acessível e bem estruturada.

**⚠️ ATENÇÃO: O prazo de entrega desta atividade (abertura do Pull Request) é HOJE, ao final da aula.**

**💻 REQUISITO TÉCNICO: Todo o desenvolvimento desta etapa deve ser realizado utilizando os notebooks disponibilizados pela instituição.**

## 📋 Missões da Equipe (Passo a Passo)

Para concluir a atividade de hoje, sua equipe deve seguir as etapas abaixo:

### 1. Atualização do Card da Equipe (`index.html`)

Localize o card provisório da sua equipe na página principal e atualize-o com dados reais:

* **Nome da Equipe e Integrantes:** Insira o nome oficial do estúdio/equipe e o nome de todos os membros.
* **Título do Jogo:** O nome oficial do projeto de vocês.
* **Plataforma e Modalidade:** Atualize as *badges* e descrições (Mobile, Desktop, Console, Web/Browser).
* **Tags de Busca:** Atualize os atributos `data-tags` da sua `<div class="team-card">` para que o sistema de busca encontre o jogo de vocês facilmente.

### 2. Criação da Store Page Dinâmica (HTML)

O conceito de "Store Page" em PDF evoluiu. Agora, vocês terão uma página web real para o jogo.

* Substitua o conteúdo da página HTML dedicada da sua equipe criando uma Store Page real e chamativa (podem usar o template do portal como base).
* **Link de Acesso ao Jogo:** Esta página *obrigatoriamente* deve conter um botão/link jogável ou de download do projeto. Pode ser o link para jogar no browser, a URL da loja (Google Play/App Store) ou um link do Google Drive para baixar o executável do jogo.
* O botão secundário no card da página inicial (`index.html`) deve redirecionar para essa nova Store Page HTML.

### 3. Anexo do Game Design Document (GDD)

O botão principal que antes baixava a Store Page em PDF deverá, a partir de agora, apontar para o **Game Design Document (GDD)** do jogo de vocês em formato PDF.

**O que é o GDD e como fazê-lo?**

Um bom GDD serve como material de referência fundamental para a equipe durante o desenvolvimento, funcionando como uma "planta baixa para construção de um edifício". Ele existe para dois propósitos vitais: memória e comunicação.

* **Se a equipe já possui um GDD:** Exporte para PDF, coloque na pasta correspondente no repositório e vincule-o ao botão do card.
* **Se a equipe AINDA NÃO possui um GDD:** Vocês deverão redigi-lo **durante a aula de hoje**. Recomendo utilizarem o formato **One-Sheet** (uma página contendo uma visão geral com título, plataformas, público-alvo, modos de jogo e pontos principais de venda)  ou um formato **Ten-Pager** simplificado, caso precisem detalhar controles, história e o fluxo principal do jogo.

* *Lembrete de Design:* O GDD deve conter informações relacionadas ao desenvolvimento do jogo e ao que será apresentado ao jogador. Evitem detalhar no documento sistemas não testados ou elementos de história profunda (*backstory*) que o jogador nunca verá na tela.

### 4. Submissão via GitHub (Pull Request)

Todo o ecossistema do nosso portal roda via GitHub Pages. Para entregar a atividade:

1. Faça um clone do repositório: `https://github.com/PalmutiUnis/PalmutiUnis.github.io`
2. Crie uma nova **Branch** com o nome da sua equipe (ex: `feature/equipe-alpha`).
3. Faça os *commits* das suas alterações (`index.html`, página HTML da Store Page e o PDF do GDD).
4. Faça o *Push* para o GitHub e abra um **Pull Request (PR)** para a branch `main`.
5. **IMPORTANTE:** Adicione o Professor como **Revisor (Reviewer)** do seu Pull Request.

---

## 🏆 Critérios de Conclusão

A atividade será considerada "Concluída" quando o Pull Request estiver aberto contendo:

* [ ] Card da página inicial totalmente atualizado.
* [ ] Store Page em HTML criada e linkada corretamente, contendo o acesso ao jogo (Drive/Web/Lojas).
* [ ] GDD (Game Design Document) em PDF linkado no botão principal do card.
* [ ] PR submetido dentro do prazo da aula e com o professor marcado como revisor.

🕹️ Mãos à obra e excelente desenvolvimento! Nos vemos no playtest.
