# Brasil Desenvolvedor 🇧🇷

**Uma iniciativa por um Brasil que valoriza quem cria tecnologia.**

O Brasil Desenvolvedor é um projeto independente criado para apresentar uma proposta legislativa voltada ao desenvolvimento tecnológico brasileiro, ampliar o debate público e reunir manifestações voluntárias de apoio à iniciativa.

O projeto disponibiliza informações sobre a proposta, permite que os visitantes conheçam seu conteúdo e oferece um formulário online para registrar manifestações de apoio.

> **Importante:** este é um projeto independente. A proposta apresentada é um texto de iniciativa própria, não representa uma lei aprovada nem constitui, por si só, uma iniciativa legislativa oficial.

## 🎯 Objetivos

- Incentivar o desenvolvimento tecnológico no Brasil.
- Ampliar o acesso à informação sobre a proposta legislativa.
- Facilitar a participação pública por meio de manifestações voluntárias de apoio.
- Estimular o debate sobre medidas que possam fortalecer o ecossistema de tecnologia brasileiro.
- Demonstrar como ferramentas acessíveis podem ser utilizadas para criar projetos digitais de interesse público.

## 🌐 Acesse o projeto

- **Website:** https://brasildesenvolvedor.pages.dev/
- **API:** https://brasil-desenvolvedor-api.raphael-palhares1006.workers.dev/

## ✨ Funcionalidades

- Página pública com informações sobre o projeto.
- Apresentação do texto da proposta legislativa diretamente no site.
- Formulário para registrar manifestações de apoio.
- Proteção contra envios automatizados com Cloudflare Turnstile.
- Armazenamento de dados com Cloudflare D1.
- Interface responsiva para diferentes tamanhos de tela.
- API própria para processar as solicitações do formulário.

## 🛠️ Tecnologias utilizadas

| Tecnologia | Finalidade |
|---|---|
| HTML5 | Estrutura das páginas |
| CSS3 | Estilização e responsividade |
| JavaScript | Interatividade e comunicação com a API |
| Cloudflare Pages | Hospedagem do site |
| Cloudflare Workers | Execução da API |
| Cloudflare D1 | Banco de dados SQL |
| Cloudflare Turnstile | Proteção contra envios automatizados |

O projeto foi desenvolvido com foco em simplicidade, acessibilidade e utilização de serviços com opções gratuitas.

## 📁 Estrutura do projeto

```text
brasil-desenvolvedor/
├── site/
│   ├── index.html
│   ├── style.css
│   ├── script.js
│   ├── config.js
│   └── projeto-de-lei.md
├── docs/
│   └── projeto-de-lei.md
└── cloudflare/
    ├── worker.js
    ├── schema.sql
    └── wrangler.toml
```

- `site/`: arquivos do website.
- `site/config.js`: configurações públicas utilizadas pelo frontend.
- `site/projeto-de-lei.md`: texto da proposta apresentado no site.
- `docs/`: documentação do projeto.
- `cloudflare/worker.js`: código da API.
- `cloudflare/schema.sql`: estrutura inicial do banco de dados.
- `cloudflare/wrangler.toml`: configuração de desenvolvimento e implantação com Wrangler.

## 🚀 Executando localmente (Em Breve)

## 🤝 Contribuições

Sugestões, correções e melhorias são bem-vindas.

Para contribuir:

1. Faça um fork do repositório.
2. Crie uma branch para sua alteração.
3. Faça as modificações e teste o funcionamento.
4. Envie um pull request descrevendo o que foi alterado.

## 📜 Licença

O código-fonte deste projeto é disponibilizado sob a licença MIT, permitindo seu uso, cópia, modificação, distribuição e utilização comercial, desde que os avisos de direitos autorais e a licença sejam preservados.

A licença do código não se estende automaticamente à proposta legislativa, aos documentos, à identidade visual ou às marcas do projeto.

Consulte o arquivo ""LICENSE"" (./LICENSE) para conhecer os termos completos da licença aplicável ao código.

**Brasil Desenvolvedor — tecnologia, participação e iniciativa.**
