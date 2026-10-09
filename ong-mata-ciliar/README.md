# Instituto Mata Ciliar - site institucional (exemplo)

Site de uma ONG fictícia que protege nascentes e restaura matas ciliares.
Projeto da disciplina de Desenvolvimento Web, feito apenas com HTML5 e um CSS básico (sem JavaScript).

## Páginas

| Arquivo | Conteúdo |
|---|---|
| `index.html` | Sobre a organização: missão, visão, valores, história, equipe, transparência e contato |
| `projetos.html` | Projetos sociais, voluntariado e como doar |
| `cadastro.html` | Formulário de cadastro com validação nativa do HTML5 |

## Estrutura de pastas

```
.
├── index.html
├── projetos.html
├── cadastro.html
├── css/
│   └── estilo.css
├── img/
│   ├── *.jpg   (formato de reserva)
│   ├── *.webp  (formato otimizado, usado pelos navegadores que suportam)
│   └── logo.svg
└── README.md
```

## O que foi aplicado

- HTML5 semântico: `header`, `nav`, `main`, `section`, `article`, `aside`, `figure`, `address`, `footer`.
- Hierarquia de títulos: um `h1` por página, seguido de `h2` e `h3` em ordem.
- Imagens em WebP com JPG de reserva (`picture`), com `alt`, `width`/`height` e `loading="lazy"` abaixo da dobra.
- Formulário com `fieldset`/`legend`, `label` ligado a cada campo, tipos HTML5 (`email`, `tel`, `date`),
  `required`, `pattern`, `maxlength` e `autocomplete`.
- Acessibilidade: link "Pular para o conteúdo", `aria-current` no menu, foco visível, tabelas com `caption` e `scope`.
- Mobile-first: `meta viewport`, imagens fluidas e uma coluna única, que se adapta a qualquer largura.
- SEO: `title` e `meta description` diferentes em cada página, `lang="pt-BR"`.
- HTML e CSS validados no W3C (Nu Html Checker), sem erros e sem avisos.

## Sobre as máscaras de CPF, telefone e CEP

Sem JavaScript, o navegador não formata o texto enquanto a pessoa digita. Por isso os campos usam
`pattern`, `placeholder`, `maxlength` e `title`: o formulário só é aceito se o valor estiver no formato
`000.000.000-00`, `(11) 90000-0000` e `00000-000`. A máscara automática pode ser feita depois, com JavaScript.

## Como publicar no GitHub

1. Crie um repositório **público** no GitHub (por exemplo, `ong-mata-ciliar`).
2. Envie todos os arquivos desta pasta, mantendo as subpastas `css` e `img`.
3. Para ter o site no ar com HTTPS: em *Settings > Pages*, escolha a branch `main` e a pasta `/ (root)`.

## Observações

Nome, CNPJ, telefone, e-mail, chave Pix e dados bancários são fictícios.
As imagens são ilustrações geradas para o exemplo e podem ser trocadas por fotos reais da ONG.
