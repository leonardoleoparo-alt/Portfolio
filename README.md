# Portfolio — Leonardo Costa

Portfólio pessoal estático de Leonardo Costa, desenvolvido com HTML, CSS e JavaScript nativos, sem framework ou etapa de build.

## Recursos atuais

- Interface responsiva em tema escuro com identidade roxa.
- Português/Inglês com troca de idioma no próprio navegador.
- Menu mobile acessível, com `aria-expanded`, fechamento por `Esc` e bloqueio de scroll quando aberto.
- Animações de entrada usando `IntersectionObserver`, com fallback seguro quando JavaScript estiver desativado.
- Navegação ativa por seção.
- Suporte a `prefers-reduced-motion`.
- Links profissionais e contato direto via WhatsApp.
- Projeto Catálogo WARD com screenshot real, demo e repositório.
- SEO básico, Open Graph, Twitter Card, favicon e Apple Touch Icon.
- Imagens de interface otimizadas em WebP e dimensões explícitas para reduzir CLS e tráfego.

## Estrutura

```text
/
├── index.html
├── style.css
├── Leonardo-Costa-Curriculo.pdf
├── assets/
│   ├── hero-leonardo-purple.webp
│   ├── logo-leonardo-purple.webp
│   ├── signature-leonardo.webp
│   ├── ward-catalog-preview.webp
│   ├── favicon-lc-64.png
│   ├── apple-touch-icon.png
│   └── og-leonardo-costa.png
└── README.md
```

## Executar localmente

O projeto não precisa de instalação de dependências. É possível abrir `index.html` diretamente ou usar um servidor local.

Com Node.js:

```bash
npx serve .
```

Depois, abra o endereço informado no terminal.

## Observações

- O JavaScript fica no final de `index.html` e é usado somente para comportamento do site: revelação progressiva, estado de navegação, menu mobile, idioma e ano do rodapé.
- A rolagem suave é feita em CSS, evitando uma implementação JavaScript redundante.
- Conteúdo essencial permanece visível mesmo se JavaScript estiver desativado.
