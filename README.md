# 🏃‍♂️ Associação Atlética de Manaus (AAM) — Plataforma Oficial de Corridas

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

Plataforma web institucional e interativa desenvolvida para a **Associação Atlética de Manaus (AAM)**, projetada para centralizar a divulgação do calendário anual de corridas de rua na capital amazonense, detalhamento técnico de percursos, captação de patrocinadores, programa de voluntariado e inscrição de atletas.

---

## 🌐 Demonstração ao Vivo (Deploy)

👉 **[Acessar Plataforma no Vercel](https://site-corridas-aam.vercel.app/)**

---

## 🏆 Calendário Oficial de Provas — Temporada 2026

A plataforma apresenta quatro modalidades que percorrem os principais cartões-postais e patrimônios naturais de Manaus:

| Prova | Distância | Data | Local de Largada | Perfil do Percurso |
| :--- | :---: | :---: | :--- | :--- |
| **Maratona da Floresta** | **42K** | 15 de Agosto de 2026 | Anfiteatro da Ponta Negra | Prova rainha às margens do Rio Negro com suporte completo |
| **Meia Maratona do Encontro** | **21K** | 12 de Setembro de 2026 | Centro Histórico (Teatro Amazonas) | Circuito histórico-cultural celebrando a Belle Époque e o porto |
| **Corrida do Rio** | **10K** | 03 de Outubro de 2026 | Orla do Rio Negro | Pista plana e veloz ideal para quebra de recordes pessoais |
| **Corridinha da Comunidade** | **5K** | 20 de Novembro de 2026 | Parque Ponte dos Bilhares | Percurso arborizado voltado para iniciantes, famílias e comunidade |

---

## ✨ Principais Funcionalidades e Destaques Técnicos

- **⏱️ Cronômetro Regressivo Dinâmico (Real-Time Countdown):**
  - Desenvolvido em JavaScript puro (`Vanilla JS`), calcula em tempo real os dias, horas, minutos e segundos restantes até a próxima prova oficial (**Corridinha da Comunidade — 5K**, em 20 de novembro de 2026), com tratamento automático de encerramento quando o evento é iniciado.
- **🗺️ Páginas Individuais de Percurso com Geolocalização:**
  - Cada corrida conta com página dedicada contendo ficha técnica resumida (distância, largada, hidratação, perfil), fotografia proporcional responsiva (`object-fit: cover`) e mapa interativo integrado via **Google Maps Embed**.
- **📱 Design Responsivo e Tipografia Fluida:**
  - Layout construído com **CSS Grid** e **Flexbox**, tipografia escalável com `clamp()`, navegação adaptativa com menu mobile expansível (`aria-expanded`) e dropdown interativo para acesso rápido às modalidades.
- **🎨 Identidade Visual Amazônica & Favicon SVG:**
  - Sistema de cores baseado em variáveis CSS (`--accent-1: #0b6b58` Verde Amazônico, `--accent-2: #00a6b5` Azul Rio e `--accent-3: #f2c94c` Amarelo Solar), efeitos de *glassmorphism* (`backdrop-filter: blur`) e ícone vetorial exclusivo (`img/favicon.svg`).
- **🤝 Ecossistema Completo (Inscrições, Voluntariado e Parceiros):**
  - **Inscrições (`inscricoes.html`):** Formulário estruturado para escolha de modalidade e tamanho de camiseta técnica.
  - **Voluntariado (`volutarios/voluntarios.html`):** Apresentação das áreas de atuação (percurso, linha de chegada e entrega de kits), benefícios ao voluntário e formulário de cadastro dedicado.
  - **Parceiros (`Parceiros/parceiros.html`):** Vitrine organizada em cotas de patrocínio institucional e apoio comunitário regional.

---

## 📂 Estrutura do Projeto

```text
associacao-atletica-de-manaus/
├── index.html                  # Página inicial (Hero, Countdown, Cards das Corridas, Parceiros e Footer)
├── Corrida 1.html              # Detalhes e mapa: Maratona da Floresta (42K)
├── Corrida 2.html              # Detalhes e mapa: Meia Maratona do Encontro (21K)
├── Corrida 3.html              # Detalhes e mapa: Corrida do Rio (10K)
├── Corrida 4.html              # Detalhes e mapa: Corridinha da Comunidade (5K)
├── inscricoes.html             # Formulário de inscrição de atletas
├── styles.css                  # Folha de estilos global e responsividade
├── Parceiros/
│   ├── parceiros.html          # Página de patrocinadores oficiais e parceiros comunitários
│   └── styles.css              # Estilos específicos da seção de parceiros
├── volutarios/
│   ├── voluntarios.html        # Página do programa de voluntariado e formulário de staff
│   └── styles.css              # Estilos específicos da página de voluntariado
├── img/                        # Ativos visuais, fotografias de Manaus e favicon.svg
└── README.md                   # Documentação técnica do projeto
```

---

## 🛠️ Tecnologias Utilizadas

- **HTML5 Semântico:** Uso adequado de tags estruturais (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`) e atributos de acessibilidade (`aria-label`, `aria-live`, `aria-expanded`).
- **CSS3 Moderno:** Custom Properties (variáveis CSS), CSS Grid Layout, Flexbox, Media Queries para múltiplos breakpoints (`900px` e `650px`) e transições suaves.
- **JavaScript (ES6+):** Manipulação do DOM, controle de estado de menus dropdown e mobile, atualização dinâmica de ano no rodapé e temporizador `setInterval` para o cronômetro regressivo.
- **Google Fonts:** Tipografia moderna com a família de fontes **Inter** (`300`, `400`, `600`, `700`).

---

## 🚀 Como Executar Localmente

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/italoholanda-dev/associacao-atletica-de-manaus.git
   ```
2. **Acesse o diretório do projeto:**
   ```bash
   cd associacao-atletica-de-manaus
   ```
3. **Inicie o projeto:**
   Abra o arquivo `index.html` diretamente no navegador ou utilize a extensão **Live Server** no VS Code para recarregamento automático.

> **ℹ️ Nota Técnica sobre o Formulário:**
> Originalmente concebido com integração a um backend Node.js/SQL para persistência de inscrições, o projeto opera em produção na Vercel como uma aplicação Front-end estática interativa, exibindo confirmações diretas no cliente para facilitar testes e demonstração de portfólio.

---

## 👨‍💻 Autor

Desenvolvido por **Ítalo Holanda** — [GitHub](https://github.com/italoholanda-dev)
