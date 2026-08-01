# 🚀 Discord Landing Page - 2026 Edition

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-brightgreen?style=for-the-badge)

> Recriação moderna e responsiva da **Landing Page do Discord (Edição 2026)**, com correções de bugs de seletores CSS, suporte total a tema Claro/Escuro (Modo Noturno com `:has()`), mockups interativos de chat/voz/cargos e novo layout adaptado para padrões atuais.

---

## 🛠️ Principais Correções e Melhorias Realizadas

### 1. 🐛 Correção do Bug do Alternador de Tema Escuro
- **Problema anterior:** O seletor `.theme-toggle-checkbox:checked ~ body` no CSS não funcionava porque a tag `body` é o elemento pai (não irmão) do `input`, fazendo com que as variáveis CSS do fundo da página e de textos não mudassem no escopo global.
- **Solução:** Implementação moderna com o pseudo-seletor `:has()` (`:root:has(#theme-toggle:checked)`) e seletores de elementos irmãos de fallback (`:checked ~ .hero`, `:checked ~ main`, `:checked ~ .footer`), garantindo alternância de tema impecável em 100% dos navegadores sem JavaScript.

### 2. 🎨 Identidade Visual Atualizada para Padrões Discord 2026
- **Cores Oficiais:** Substituição do verde escuro genérico da Hero pelo clássico **Discord Blurple** (`#5865F2`), mantendo acentos em **Green Online** (`#23A55A`), **Fuchsia Nitro** (`#EB459E`) e **Midnight Blue** (`#1E1F22`).
- **Tipografia:** Integração dinâmica com **Inter** para leitura limpa e **Luckiest Guy** para os títulos emblemáticos do Discord.

### 3. 📱 Header Completo e Menu Mobile Drawer
- Adição da barra de navegação desktop completa (Recursos, Nitro, Tecnologia, Descobrir, Suporte, Carreiras, Botão de Login).
- **Menu Mobile Drawer:** Menu hambúrguer funcional em CSS puro com animação lateral de gaveta.

### 4. 💻 Mockups Interativos e Ricos de UI
- **Hero Banner:** Ilustração com badges flutuantes animadas (`10.450 Online`, `Lounge de Voz`, `Impulso Nível 3`).
- **Canal de Texto:** Interface de chat com sidebar de canais, avatares de membros, cargos coloridos (`Mod`, `VIP`), badges e reações com emojis (`🔥`, `🎮`, `❤️`).
- **Canal de Voz:** Grid de membros em chamada com indicador pulsante de fala (`speaking-ring`), botões de atalho de microfone/áudio e transmissão ao vivo.
- **Moderação:** Painel de gerenciamento de cargos (`Admin`, `Mod`, `Nitro`, `Membro`) e banner AutoMod.
- **Nova Seção Discord Nitro:** Destaque para benefícios do Nitro com card em gradiente imersivo.
- **Transmissão HD 4K:** Preview de grid de vídeo com contador de FPS e latência ultra-baixa (`12ms`).

### 5. 🌐 Rodapé Completo
- Estrutura multi-colunas oficial do Discord (Produto, Empresa, Recursos, Políticas).
- Selecionador de idioma (`Português - Brasil`), ícones de redes sociais e copyright atualizado.

---

## 📐 Estrutura de Arquivos

```text
discord-landing-page_2026/
├── index.html          # Estrutura HTML5 semântica e acessível
├── app.html            # Web App demo (mockup da interface 2026)
├── css/
│   ├── style.css       # Design System, Variáveis CSS, Reset e Responsividade
│   └── app.css         # Estilos do Web App (app.html)
├── images/
│   ├── hero_bg.jpg     # Ilustração da Hero com comunidade Discord (otimizada)
│   ├── avatar_gamer.jpg# Avatar perfil gamer (otimizado)
│   ├── avatar_artist.jpg# Avatar perfil artist (otimizado)
│   └── discord-2026.jpg# Mockup da interface do Web App
└── README.md           # Documentação técnica atualizada
```

---

## 💻 Como Executar

Por ser uma aplicação web nativa (Pure HTML/CSS), não exige nenhuma instalação de pacotes Node.js:

1. **Abrir diretamente:** Basta dar um duplo clique no arquivo `index.html` em qualquer navegador moderno.
2. **Servidor Local (opcional):**
   ```bash
   python -m http.server 8080
   ```
   Em seguida, acesse `http://localhost:8080` no navegador.

---

## 👨‍💻 Autor

Desenvolvido e aprimorado por **Pedro Zeferino da Silva**.
- **Licença:** MIT
