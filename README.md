# ⚖️ Ética e Inteligência Artificial | Futuro Responsável

Projeto front-end de uma página web imersiva focado no debate contemporâneo sobre a regulamentação, governança e impactos éticos da Inteligência Artificial. 

Este trabalho foi desenvolvido como projeto de conclusão da disciplina de **Direito Aplicado à Informática** na 1ª fase do curso de **Análise e Desenvolvimento de Sistemas (ADS)**, combinando pesquisa jurídico-tecnológica com práticas de UI/UX Design (Estilo Cyberpunk/Sci-Fi) e manipulação gráfica avançada com JavaScript Vanilla.

Este foi um projeto onde assumi o papel de Arquiteto e Engenheiro de Prompt. Como eu queria entregar uma experiência visualmente impressionante para o meu conteúdo da disciplina de Direito Digital, utilizei ferramentas de IA assistida (como o Cursor) como parceiras de desenvolvimento. Fui responsável por definir a arquitetura semântica, direcionar a lógica do Canvas, as regras de CSS e validar todo o comportamento de UI/UX, revisando e integrando o código final para garantir que fosse performático e otimizado.

---

## 🎯 Objetivo do Projeto

Transformar um tema analítico e crítico — os desafios regulatórios e éticos da IA — em uma experiência digital interativa e engajante. 

O site atua como um manifesto interativo, estruturando de forma imparcial e visual os dois lados do debate contemporâneo (pró-regulamentação vs. livre inovação), além de abordar privacidade de dados, viés algorítmico, governança global (UNESCO) e os princípios de *Ética by Design*.

---

## 🚀 Funcionalidades e Diferenciais da Interface

- **Animação Procedural em Canvas 2D (`<canvas>`):** Renderização dinâmica em tempo real de uma malha tridimensional perspectivada (3D Grid) combinada com um sistema constelado de partículas interligadas (`Particle Network`), executada em 60 FPS via `requestAnimationFrame`.
- **Efeito Visual "Sci-Fi / Cyberpunk" (CRT Scanline):** Aplicação de uma camada de sobreposição (`.scan-overlay`) simulando monitores analógicos CRT e efeitos de brilho *Neon* com `text-shadow` e `box-shadow` multicamadas.
- **Scroll Spy & Navegação Ativa:** Monitoramento da barra de rolagem através da **Intersection Observer API** para realçar dinamicamente o link da seção em foco na barra de navegação.
- **Animações Condicionadas ao Scroll:** Elementos visuais (Cards, Alertas de Risco, Blocos de Citação) aparecem de forma fluida (`fadeInUp`) apenas quando entram na área de visualização do usuário, otimizando o processamento gráfico.
- **Apresentação Crítica e Multidisciplinar:** Síntese equilibrada cobrindo viés de algoritmos em concessão de crédito, dilemas da autonomia humana e o custo ambiental de carbono no treinamento de Grandes Modelos de Linguagem (LLMs).

---

## 🛠️ Tecnologias e Conceitos de Engenharia Aplicados

O projeto não utiliza frameworks externos, evidenciando forte domínio do núcleo web padrão:

*   **HTML5 Semântico e Acessível:**
    * Uso consistente de atributos de acessibilidade (`aria-label`, `aria-labelledby`, `aria-hidden="true"`, `role="navigation"`).
    * Estrutura visual tipográfica usando Google Fonts (`Orbitron` para cabeçalhos sci-fi e `Exo 2` para leitura estendida).
*   **CSS3 Moderno & Arquitetura de UI:**
    * **Glassmorphism:** Interface de cartões translúcidos construídos com `backdrop-filter: blur(12px)` e bordas com luminosidade sutil.
    * **Variáveis Globais (`:root`):** Padronização de paleta de cores (Cyan, Blue e Orange Dim) para facilitar a manutenção e manter a harmonia dos tons *neon*.
    * **CSS Grid & Flexbox:** Criação de layouts responsivos complexos sem recorrer ao Bootstrap ou Tailwind CSS.
    * **Keyframe Animations:** Animações CSS nativas para flutuação de imagens (`@keyframes float-slow`) e pulsações contínuas de luz (`@keyframes glow-pulse`).
*   **JavaScript Vanilla (ES6+):**
    * **API de Canvas (HTML5 Canvas 2D Context):** Lógica matemática de projeção e renderização vetorial para gerar a rede de conexões que reage perfeitamente ao redimensionamento da janela (`window.addEventListener('resize')`).
    * **IntersectionObserver API:** Substituição moderna e performática aos eventos pesados de `onscroll` para gerenciar animações de entrada e realce de links do menu.

---

## 💻 Como Executar e Visualizar o Projeto

Por ser estruturado de forma estática e autônoma, você pode rodá-lo localmente em segundos sem precisar instalar pacotes node.

### 1. Visualização Online (Recomendado)
Acesse a página em produção através do GitHub Pages:
👉 **[Acessar a SPA](https://henriquesssantos.github.io/Etica-e-Inteligencia-Artificial/)**

### 2. Acesso Rápido Local
1. Clone este repositório no seu terminal:
   ```bash
   git clone [https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git](https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git)
