ANIMATION TOGGLE

<p align="center"> <a href="https://animation-toggle.vercel.app"> <img src="https://img.shields.io/badge/Deploy-Vercel-black?style=for-the-badge&logo=vercel" alt="Vercel Deploy" /> </a> <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" /> <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" /> <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" /> </p> <p align="center"> Um toggle animado de tema claro/escuro com animação suave entre <b>sol e lua</b>.<br/> Feito em <b>HTML, CSS e JavaScript puro</b>, sem frameworks. </p> <p align="center"> <a href="https://animation-toggle.vercel.app"><b>🔗 Acesse o Deploy ao vivo → animation-toggle.vercel.app</b></a> </p>

🌓 Preview
<p align="center"> <img src="https://raw.githubusercontent.com/Jairocpdev/animation-toggle/main/preview.gif" alt="Animation Toggle Preview" width="600" onerror="this.style.display='none'" /> </p>
Se ainda não tem um GIF, grave a tela do toggle (pode usar o próprio Vercel) e salve como preview.gif na raiz do repo. O README já está preparado para exibir automaticamente.

O componente alterna entre:

☀️ Light mode - transição clara com animação do sol
🌙 Dark mode - transição escura com animação da lua
Com animação fluida, transição de cores e foco em UX.

🚀 Tecnologias
HTML5 - Estrutura semântica
CSS3 - Animações, @keyframes, variáveis CSS e transition
JavaScript - Lógica de toggle com classList.toggle
Vercel - Hospedagem e deploy contínuo
📁 Estrutura
bash
animation-toggle/
├── index.html   # Markup do toggle (☀️ / 🌙)
├── styles.css   # Animações, temas e transições
├── scripts.js   # Lógica de alternância e localStorage
└── preview.gif  # (opcional) GIF de demonstração
⚙️ Como funciona
js
// scripts.js
const toggle = document.querySelector('.toggle');
const body = document.body;

toggle.addEventListener('click', () => {
  body.classList.toggle('dark');
  localStorage.setItem('theme', body.classList.contains('dark') ? 'dark' : 'light');
});
💻 Instalação e uso local
bash
# 1. Clone o repositório
git clone https://github.com/Jairocpdev/animation-toggle.git

# 2. Entre na pasta
cd animation-toggle

# 3. Abra o projeto
# Opção A: Clique duplo no index.html
# Opção B: Com VS Code + Live Server
# Opção C: Com servidor simples
npx serve .
Não precisa instalar dependências.

🎨 Customização rápida
No topo do seu styles.css:

css
:root {
  --bg-light: #ffffff;
  --bg-dark: #101010;
  --toggle-size: 60px;
  --transition-duration: 0.5s;
  --transition-timing: cubic-bezier(0.68, -0.55, 0.265, 1.55);
}
Altere --transition-duration para deixar a animação mais rápida/lenta.

📦 Deploy
Este projeto já está no ar na Vercel. Para fazer o seu:

[Deploy with Vercel](https://vercel.com/new/clone?repository-url=https://github.com/Jairocpdev/animation-toggle)

Ou manualmente:

Fork este repositório
Importe no Vercel > New Project
Deploy automático, sem necessidade de build  

📝 Licença
MIT - Livre para usar, modificar e compartilhar.

<p align="center"> Feito com 🖤 por <a href="https://github.com/Jairocpdev">Jairo Andrade</a> • <a href="https://animation-toggle.vercel.app">Ver Deploy</a> </p>
