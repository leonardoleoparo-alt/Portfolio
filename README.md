# 🚀 Meu Portfólio Pessoal

Bem-vindos ao repositório do meu portfólio pessoal! Este projeto foi desenvolvido para apresentar minha trajetória profissional, minhas habilidades e (futuramente) os projetos de programação que irei construir. 

O foco deste projeto foi construir uma página estática moderna, performática e responsiva, utilizando puramente as tecnologias base da web (sem o uso de frameworks pesados).

---

## 🛠️ Tecnologias Utilizadas

A stack escolhida foi focada em **Vanilla Web Technologies**, garantindo carregamento instantâneo e total controle sobre o DOM:
- **HTML5:** Semântico e estruturado.
- **CSS3:** Variáveis nativas (Custom Properties), Flexbox, CSS Grid, Glassmorphism e animações com `@keyframes`.
- **JavaScript (Vanilla):** Manipulação do DOM para interatividades complexas (suporte bilíngue, animações de scroll e menu mobile).

---

## ✨ Principais Funcionalidades

Implementei diversas features para tornar a experiência do usuário (UX) e a interface (UI) mais atrativas:

1. **Tema "Dark Mode" Moderno:**
   - Paleta de cores escura (`#0a0a0f`) com acentos luminosos em tons de roxo (`#7C3AED` e `#A855F7`).
   - Efeito de **Glassmorphism** (fundo desfocado) no header de navegação (`backdrop-filter`).
   
2. **Suporte Bilíngue (PT / EN):**
   - Sistema de tradução *on-the-fly* (em tempo real) construído em JavaScript.
   - Através de atributos de dados (`data-pt` e `data-en`) injetados no HTML, a página troca todo o conteúdo, inclusive links de navegação e *placeholders* do formulário, sem precisar recarregar o navegador.

3. **Efeito "Typing" (Máquina de Escrever):**
   - Um script dedicado que itera sobre arrays de strings ("Estudante de Programação", "Apaixonado por Tecnologia") gerando um efeito de digitação e apagamento contínuo na seção Hero.

4. **Animações de "Scroll Reveal":**
   - Os elementos não aparecem todos de uma vez. Utilizei a API de escuta de scroll (`window.addEventListener('scroll')`) para calcular a posição dos elementos na tela e adicionar a classe `.active` no momento certo, criando uma animação de *fade-in-up* suave ao rolar a página.

5. **Responsividade Total (Mobile-First):**
   - O layout se adapta perfeitamente a dispositivos móveis.
   - Implementação de um menu **Hamburger** customizado que bloqueia o scroll do corpo da página (`body.no-scroll`) quando aberto, oferecendo uma navegação fluida no celular.

---

## 📂 Arquitetura do Projeto

A estrutura de arquivos foi mantida simples, porém altamente organizada:

```text
/
├── index.html       # Estrutura principal da página e lógica JavaScript incorporada
├── style.css        # Folha de estilos contendo o "Design System" do projeto
├── curriculo.pdf    # Currículo em PDF para download direto
├── main.jpg         # Imagem de avatar para a seção Hero
└── README.md        # Esta documentação!
```

### Notas sobre o `style.css`
O CSS foi estruturado utilizando **Design Tokens** na raiz (`:root`). Isso permite que, se a equipe quiser alterar o tom de roxo do projeto para verde, por exemplo, basta alterar a variável `--accent` e a mudança refletirá globalmente em botões, bordas, textos e sombras de neon.

### Notas sobre o `index.html`
Para evitar múltiplas requisições de arquivos menores e garantir velocidade máxima, a lógica JavaScript foi incorporada ao final da tag `<body>`. Ela está documentada e dividida em blocos (Typing Effect, Scroll Reveal, Header Background, Mobile Menu, Language Toggle e Smooth Scroll).

---

## ⚙️ Como executar localmente

Sendo um projeto Vanilla, não há necessidade de gerenciadores de pacote (`npm` ou `yarn`):
1. Clone este repositório.
2. Abra o arquivo `index.html` em qualquer navegador moderno.
3. *Opcional:* Se você utiliza o VS Code, recomendo usar a extensão **Live Server** para obter recarregamento automático durante o desenvolvimento.

---

> **Desenvolvido com muita dedicação por Leonardo Costa.** Vamos nos conectar! Sinta-se à vontade para enviar PRs ou dicas de melhorias. 💜
