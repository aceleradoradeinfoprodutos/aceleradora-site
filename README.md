# Aceleradora de Infoprodutos — Página de Aplicação

Página de vendas / aplicação da Aceleradora de Infoprodutos.

## Stack

- HTML estático (arquivo único, self-contained)
- Meta Pixel integrado (ID: `1832130584199265`)
- Deploy: Vercel (via GitHub)

## Eventos rastreados no Meta Pixel

- `PageView` — dispara automaticamente ao carregar a página
- `Lead` — dispara quando alguém clica em qualquer CTA com palavra-chave de aplicação
  ("aplicar", "escalar", "quero", "diagnóstico", "entrar no programa")
- `InitiateCheckout` — dispara UMA vez por sessão no primeiro clique de CTA de aplicação

## Deploy

### Opção 1 — via Vercel (recomendado)

1. Suba este repositório no GitHub
2. Entre em [vercel.com](https://vercel.com), clique em **Add New → Project**
3. Selecione este repositório
4. Deixe as configurações padrão (Framework: Other)
5. Clique em **Deploy**

Site vai ficar no ar em segundos, com HTTPS automático.

### Opção 2 — domínio próprio

Depois do deploy no Vercel, em **Settings → Domains** você aponta seu domínio.
DNS típico: adicionar registro `A` apontando para o IP do Vercel, ou `CNAME`
apontando para o domínio Vercel fornecido.

## Estrutura do arquivo

O `index.html` contém toda a página em um único arquivo (2.2MB), com imagens
embutidas em base64. Isso torna o deploy trivial — não depende de servidor
processando nada, funciona em qualquer host estático.
