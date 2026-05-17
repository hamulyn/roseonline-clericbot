# 🛡️ Cleric Support Tool

Um script de automação avançado desenvolvido em AutoHotkey v2 para facilitar a vida de quem joga com um Cleric como personagem de suporte (Dual-Box) no Rose Online. 

O grande diferencial desta ferramenta é a execução em **segundo plano**. Você não precisa focar na janela do seu Cleric para que ele te cure ou te buffe; o programa envia os comandos silenciosamente enquanto você controla seu personagem principal!

---

## 📋 Índice
1. [Pré-requisitos](#-pré-requisitos)
2. [Instalação](#-instalação)
3. [Guia de Uso (Manual do Usuário)](#-guia-de-uso)
   - [Conectando o Jogo](#1-primeiros-passos-conectando-o-jogo-)
   - [Cleric Hotkeys (O que o boneco aperta)](#2-cleric-hotkeys-as-teclas-do-jogo-)
   - [Macro Hotkeys (O que VOCÊ aperta)](#3-macro-hotkeys-os-seus-controles-)
   - [O Menu Principal](#4-o-menu-principal-seu-painel-de-controle-)
   - [Overlay Config](#5-overlay-config-painel-visual-flutuante-)
   - [Presets](#6-presets-salvando-suas-configurações-)

---

## ⚙️ Pré-requisitos

* **Sistema Operacional**: Windows 10 ou superior.
* **Permissões**: Executar o programa como Administrador (clique com o botão direito > *Executar como Administrador*) para garantir que os comandos em segundo plano funcionem corretamente dentro do jogo.
* **Arquitetura**: Compatível com sistemas de 64 bits.

---

## 🚀 Instalação e Execução

Por ser um arquivo executável compilado (`.exe`), o processo é extremamente simples e não requer a instalação prévia de nenhuma outra ferramenta:

1. Baixe a versão mais recente do arquivo `Cleric_Companium.exe` na aba de **Releases** do repositório.
2. Mova o executável para uma pasta de sua preferência (o script criará automaticamente as subpastas `\Presets` e `\Logs` no mesmo diretório).
3. Dê um duplo clique no arquivo `Cleric_Companium.exe` para iniciar.
4. Um ícone aparecerá na sua bandeja do sistema (perto do relógio do Windows) e o menu principal será aberto automaticamente.

---

## 📖 Guia de Uso

### 1. Primeiros Passos: Conectando o Jogo 🪟
Antes de qualquer coisa, o programa precisa saber *qual* é a janela do seu Cleric para enviar os comandos corretamente.

* **Opções de Janela (`🪟 Opções Janela`):** Aqui você define o nome padrão da janela do jogo (o padrão é "Destiny"). Você também pode configurar o **Delay entre comandos**, que é uma pequena pausa (padrão de 50ms) enviada entre cada tecla para evitar que o jogo trave ou ignore seus comandos.
* **Selecionar Janela (`🎯 Selecionar`):** No menu principal, clique neste botão. Ele abrirá uma lista com todas as janelas abertas com o nome do jogo. Selecione a janela do seu Cleric e confirme.
* **Status de Conexão:** O menu mostrará `✅ [Nome da Janela]` se estiver conectado, ou `❌ Não conectado` caso contrário.

### 2. Cleric Hotkeys: As Teclas do Jogo ⚙️
Neste menu, você informa ao script **onde as skills estão na barra de atalhos do jogo**.

* **Game Key (Tecla no Jogo):** A tecla exata que o Cleric usaria. (Ex: se *Cure* está no "4", coloque "4") .
* **Delay (ms):** O tempo de espera *após* o uso da skill, essencial para respeitar a animação do personagem.
  > **Recomendações padrão:**
  > * Buffs normais: `1600ms`.
  > * Healing: `6000ms`.
  > * Bonfire: `14000ms`.
* **Ativo:** Marque a caixa para incluir o buff na sua sequência automática.
* **Pressões por Buff:** Define quantas vezes o botão será "apertado" virtualmente (evita falhas por lag).
* **Modo Bonfire / Healing:** Permite escolher entre o uso único ou o modo **Spam** (repetição automática off-CD respeitando o delay).

### 3. Macro Hotkeys: Os Seus Controles 🎮
Estes são os **botões que VOCÊ vai apertar no seu teclado** enquanto joga no seu personagem principal.

* **🔮 Buff Hotkey:** Executa todos os buffs marcados como ativos em sequência.
* **💚 Party Heal:** Ativa a cura. Liga/desliga o modo Spam se estiver configurado.
* **💊 Cure / ✨ Resurrection:** Restaura HP de um alvo ou revive um jogador.
* **🔥 Bonfire:** Invoca a fogueira. Liga/desliga o modo Spam se configurado.
* **🏃 Follow / Unfollow:** Faz o Cleric seguir o nick configurado. 
  * *Nota: Preencha o campo "Nick para Follow" com o nome exato do personagem principal.*

**Hotkeys de Sistema Padrão:**
* `Delete`: Abre o menu principal.
* `F12`: Pausa o script temporariamente (Suspend).
* `Home`: Mostra/esconde o Overlay.

### 4. O Menu Principal: Seu Painel de Controle 📊
Use a hotkey de Menu para acessar o resumo em tempo real do seu Cleric.

* **Status:** Visualize rapidamente se suas macros estão `▶️ ATIVOS` ou `⏸️ SUSPENSO`.
* **Indicadores de Spam:** Confirme visualmente se o auto-heal ou a fogueira estão ligados.
* **Debug Mode:** Ative a caixinha `Debug` para ver ToolTips com mensagens detalhadas sobre as ações do script em tempo real.

### 5. Overlay Config: Painel Visual Flutuante 🖥️
Uma interface clicável e transparente que fica sobre o seu jogo para ativação de skills via mouse.

* **Personalização:** Defina posição `X/Y`, tamanho (largura/altura) e escolha entre layout Vertical ou Horizontal.
* **Estilo:** Ajuste a opacidade (0-255) e altere a cor de fundo usando a paleta de cores integrada.

### 6. Presets: Salvando Suas Configurações 📦
Evite configurar tudo do zero se jogar em contas diferentes.

* Salve suas configurações atuais com um nome personalizado.
* Carregue ou exclua perfis facilmente pelo menu.

---

> **Aviso:** O uso de macros pode violar os Termos de Serviço de alguns servidores. Utilize por sua própria conta e risco.
