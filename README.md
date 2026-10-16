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

## 🚀 Executando localmente

### 1. Obtenha o código

Clone o repositório:

```bash
git clone URL_DO_REPOSITORIO
cd brasil-desenvolvedor
```

Substitua `URL_DO_REPOSITORIO` pelo endereço real do repositório no GitHub.

### 2. Configure o website

Entre na pasta `site/` e abra o arquivo `config.js`.

Configure a URL da API e a chave pública do Cloudflare Turnstile conforme o ambiente utilizado.

**Atenção:** a chave pública do Turnstile pode ser utilizada no frontend. A chave secreta deve permanecer somente no ambiente seguro do backend.

### 3. Configure a API

A API utiliza Cloudflare Workers e Cloudflare D1.

Antes de publicar, confira:

- Se o binding `DB` aponta para o banco de dados correto.
- Se as variáveis e os segredos exigidos pelo código estão configurados.
- Se as URLs permitidas para acesso à API correspondem ao domínio do website.
- Se a estrutura do banco de dados corresponde à versão atual da API.

O arquivo `cloudflare/schema.sql` contém o esquema inicial do banco. Verifique se ele corresponde à versão do código que será implantada antes de executá-lo.

### 4. Publique o projeto

O website pode ser publicado no Cloudflare Pages, enquanto a API pode ser implantada no Cloudflare Workers.

Consulte a documentação oficial:

- [Cloudflare Pages](https://developers.cloudflare.com/pages/)
- [Cloudflare Workers](https://developers.cloudflare.com/workers/)
- [Cloudflare D1](https://developers.cloudflare.com/d1/)
- [Cloudflare Turnstile](https://developers.cloudflare.com/turnstile/)

## 🔐 Segurança e privacidade

O projeto utiliza mecanismos para reduzir envios automatizados e armazenar as informações necessárias ao funcionamento do formulário.

Alguns cuidados importantes:

- Nunca publique chaves secretas, tokens ou credenciais no repositório.
- Não inclua arquivos `.env` com informações privadas.
- Restrinja o acesso ao banco de dados e aos recursos administrativos.
- Revise as regras de segurança e o tratamento dos dados antes de disponibilizar o formulário publicamente.
- Informe aos visitantes quais dados são coletados, para qual finalidade e por quanto tempo são mantidos.

A validação por CAPTCHA reduz determinados tipos de abuso, mas não comprova a identidade de quem envia o formulário. As manifestações registradas não devem ser interpretadas automaticamente como assinaturas oficiais ou como prova de apoio de pessoas únicas.

## 🤝 Contribuições

Sugestões, correções e melhorias são bem-vindas.

Para contribuir:

1. Faça um fork do repositório.
2. Crie uma branch para sua alteração.
3. Faça as modificações e teste o funcionamento.
4. Envie um pull request descrevendo o que foi alterado.

## 📜 Licença

A licença deste projeto deve ser definida pelo responsável pelo repositório.

Até que uma licença seja adicionada, não presuma que o código pode ser redistribuído ou utilizado sem restrições.

---

Desenvolvido de forma independente com o objetivo de incentivar o debate sobre o futuro da tecnologia no Brasil.

**Brasil Desenvolvedor — tecnologia, participação e iniciativa.**
