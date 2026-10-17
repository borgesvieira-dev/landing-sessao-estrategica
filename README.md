# Landing Page — Sessão Estratégica

Landing page de captação para uma sessão estratégica gratuita, desenvolvida como teste prático (2ª etapa) usando **apenas HTML e CSS puro**.

🔗 **Deploy:** https://sessao-estrategica.vieiradev.com.br/

## Tecnologias

- HTML5 semântico
- CSS3 puro (custom properties, Flexbox, Grid, `clamp()`)
- Fonte Montserrat (Google Fonts)

## Estrutura

```
.
├── index.html          # Marcação da página
├── css/style.css       # Estilos (mobile-first)
└── assets/img/         # Foto do especialista e favicon
```

## Decisões

- **Mobile-first**, com breakpoints em `768px` (tablet) e `1024px` (desktop). Tipografia e espaçamentos fluidos com `clamp()`.
- **Hierarquia**: um único `h1` no hero; cada seção com seu `h2` (ligado via `aria-labelledby`) e `h3` nos cards.
- **Visual** baseado na referência (tema escuro azul com brilhos neon e CTAs laranja).
- **Ícones em SVG inline** (com um pequeno sprite `<symbol>` para os reutilizados), evitando bibliotecas e requisições extras.
- Efeitos de brilho e anéis atrás das fotos feitos só com `radial-gradient`, `repeating-radial-gradient` e `mask-image`.
- Todos os CTAs levam à seção do formulário (`#aplicar`) com rolagem suave.
- Acessibilidade: `lang="pt-BR"`, `alt` nas imagens, `label` em todos os campos, foco visível e respeito a `prefers-reduced-motion`.

## Como rodar localmente

Abra o `index.html` no navegador ou sirva a pasta:

```bash
python3 -m http.server 8000
# http://localhost:8000
```

## Observações / limitações

- **Formulário sem backend**: o teste pede somente HTML e CSS, então o formulário tem validação nativa (`required`, `type="email"`), mas não envia dados para nenhum serviço.
- **Especialista fictício**: "Lucas Andrade" é um personagem criado para o teste. A foto é de banco de imagens gratuito.

## Créditos

- Foto: [Dellon Thomas — Pexels](https://www.pexels.com/photo/man-wearing-suit-2216607/) (Licença Pexels, uso gratuito).
