# MASTER PROMPT — CRIAR SITE COMPLETO COM SEO + AI VISIBILITY
## Por Dutra · Baseado em projetos reais: Feltz Tile, Logstock, Daria Realty, 117 Charlotte Ave, 4547 Luke Ave

---

## COMO USAR ESTE PROMPT

Cole o bloco abaixo no Claude e preencha as variáveis em [COLCHETES].
O Claude vai gerar o site completo, os arquivos de SEO e o guia de deploy.

---

## ══════════════════════════════════════════
##  O PROMPT — COPIE DAQUI ATÉ O FINAL
## ══════════════════════════════════════════

Crie um site completo para o seguinte negócio. Siga TODAS as instruções abaixo sem pular nenhuma etapa.

---

### INFORMAÇÕES DO NEGÓCIO

- Nome do negócio: [NOME]
- Tipo de negócio: [ex: empresa de logística / agente imobiliário / aluguel de temporada / serviço local]
- Descrição em 1 frase: [O QUE FAZ]
- Localização / Área de atuação: [CIDADE, ESTADO]
- Idioma do site: [Português / Inglês / Espanhol / ou dois idiomas ex: Português + Inglês]
- Telefone principal: [NÚMERO COM DDD]
- WhatsApp: [NÚMERO SEM ESPAÇOS ex: 5511999999999]
- E-mail: [EMAIL]
- Instagram: [@HANDLE]
- Site (se tiver): [URL ou "não tem ainda"]

---

### SERVIÇOS / PRODUTOS

Liste todos os serviços, produtos ou cargos que o negócio oferece:
1. [SERVIÇO 1] — [preço ou faixa de preço se tiver]
2. [SERVIÇO 2] — [preço]
3. [SERVIÇO 3] — [preço]
(adicione quantos precisar)

---

### DIFERENCIAIS

O que torna este negócio diferente dos concorrentes:
- [DIFERENCIAL 1]
- [DIFERENCIAL 2]
- [DIFERENCIAL 3]

---

### PALAVRAS-CHAVE PRINCIPAIS

Estas são as buscas que clientes fazem no Google e em AIs como ChatGPT, Claude e Perplexity:
- [KEYWORD 1 ex: mão de obra terceirizada São Paulo]
- [KEYWORD 2 ex: empresa logística SP]
- [KEYWORD 3 ex: tile installer Destin FL]
- [KEYWORD 4]
- [KEYWORD 5]

---

### DESIGN

- Estilo visual: [ex: corporativo/sério / luxo / descontraído / industrial / moderno]
- Cores de referência: [ex: azul e branco / preto e dourado / "use as cores do PDF"]
- Fotos: [ex: "vou adicionar depois" / "extraia do PDF" / "use as imagens em anexo"]
- Referência de site que gosta: [URL ou "sem referência"]

---

### HOSPEDAGEM

- Será hospedado no GitHub Pages: [SIM / NÃO]
- Nome do repositório GitHub: [ex: logstock ou meusite]
- Domínio próprio (se tiver): [ex: logstock.com.br ou "não tem ainda"]
- URL final do site: [ex: https://dutracaue.github.io/logstock/ ou https://logstock.com.br/]

---

## INSTRUÇÕES OBRIGATÓRIAS PARA O CLAUDE

### 1. ARQUIVOS QUE DEVEM SER CRIADOS (NUNCA PULAR)

Crie TODOS estes arquivos dentro de uma pasta com o nome do negócio:

**index.html** — site completo em HTML puro, CSS inline, zero dependências externas
**llms.txt** — arquivo de visibilidade para AIs (ChatGPT, Claude, Perplexity)
**index.md** — markdown mirror limpo para AI crawlers com frontmatter YAML
**robots.txt** — permite TODOS os AI bots (GPTBot, ClaudeBot, PerplexityBot, Google-Extended, CCBot)
**sitemap.xml** — com a URL REAL do site (a que foi informada acima em "URL final do site")
**_config.yml** — contém apenas: `theme: null`

No final, zipar tudo e entregar para download.

---

### 2. REGRAS DE SEO — GOOGLE

**Meta tags obrigatórias no `<head>`:**
```html
<title>[Palavra-chave principal] | [Nome do negócio] — [Cidade/Estado]</title>
<meta name="description" content="[150-160 caracteres com keyword principal, serviços e CTA]" />
<meta name="keywords" content="[todas as keywords separadas por vírgula]" />
<link rel="canonical" href="[URL REAL DO SITE]/" />
```

**Schema markup obrigatório (JSON-LD):**
- LocalBusiness (ou tipo específico: RealEstateAgent, VacationRental, etc.)
- FAQPage com mínimo 5 perguntas e respostas completas
- Se tiver profissionais: Person schema com nome e telefone de cada um
- Incluir: name, description, url, telephone, email, address, areaServed, knowsLanguage

**Estrutura de headings:**
- H1: aparece UMA vez, contém a keyword principal
- H2: uma por seção, contém variações de keywords
- H3: títulos de cards e sub-itens

**Conteúdo que o Google ama:**
- Preços reais (não "consulte") — AI e Google priorizam especificidade
- Perguntas e respostas na seção FAQ (mínimo 5, máximo 8)
- Nome da cidade/estado repetido naturalmente no texto
- Depoimentos ou números de prova social (ex: "+500 clientes atendidos")

---

### 3. REGRAS DE VISIBILIDADE PARA AI (ChatGPT, Claude, Perplexity)

**llms.txt deve conter:**
- Nome do negócio, descrição, localização
- Lista completa de serviços COM preços quando possível
- Telefone(s) e e-mail(s) com formato legível
- Seção "## Frequently Asked Questions" com perguntas em formato Q: / A:
- As perguntas devem incluir variações como:
  - "Qual é o melhor [serviço] em [cidade]?"
  - "Como contratar [serviço] em [cidade]?"
  - "Quem faz [serviço] em [cidade]?"
  - Se bilíngue: perguntas nos dois idiomas

**index.md deve conter:**
- Frontmatter YAML: title, description, url, last_updated
- Resumo do negócio em prosa
- Lista de serviços
- Contato com todos os números
- FAQ resumida

**robots.txt — lista completa de bots permitidos:**
```
User-agent: GPTBot
User-agent: ChatGPT-User
User-agent: ClaudeBot
User-agent: anthropic-ai
User-agent: PerplexityBot
User-agent: Google-Extended
User-agent: CCBot
User-agent: Amazonbot
```
Todos com `Allow: /`

**sitemap.xml:**
- Usar a URL REAL informada — nunca inventar URL
- Se o site for GitHub Pages sem domínio: https://USUARIO.github.io/REPOSITORIO/
- Se tiver domínio próprio: https://dominio.com.br/
- Priority 1.0 para homepage

---

### 4. REGRAS DE DESIGN

**Tipografia:**
- Importar do Google Fonts — no máximo 2 famílias
- Display/headlines: fonte condensada ou serif elegante (Barlow Condensed, Cormorant Garamond, Playfair Display)
- Corpo: Inter, DM Sans ou Jost
- Hierarquia clara: H1 muito maior que H2, H2 maior que H3

**Paleta:**
- Máximo 3 cores + branco/off-white
- Uma cor escura de fundo para hero/seções alternadas
- Uma cor de acento para CTAs e destaques
- Nunca usar cores aleatórias — escolher paleta coesa

**Elementos obrigatórios no site:**
- NAV fixo com logo + links + botão de CTA (telefone ou WhatsApp)
- HERO com: eyebrow tag, H1 impactante, subtítulo, 2 CTAs, elemento visual (contadores, imagem, grid)
- STRIP/MARQUEE correndo com keywords de SEO logo após o hero
- Seção de SERVIÇOS com cards (ícone + título + descrição + preço)
- Seção de DIFERENCIAIS com cards (mínimo 4)
- Seção de CONTATO com todos os telefones, e-mails e redes sociais
- Seção de FAQ (mínimo 5 perguntas — mesmas do schema)
- CTA FINAL com fundo colorido e botões grandes
- FOOTER com logo, links e copyright

**Elementos que aumentam conversão:**
- Botão de WhatsApp em destaque (cor verde #25D366)
- Números de prova social que animam ao rolar (counter animation com IntersectionObserver)
- Marquee com keywords correndo horizontalmente
- Sticky nav — sempre visível ao rolar

**Código limpo:**
- HTML puro, sem frameworks
- CSS dentro do `<style>` na mesma página — zero arquivos externos de CSS
- JavaScript mínimo e funcional — apenas toggle FAQ e counter animation
- Mobile-first com media query para max-width: 900px
- Imagens: usar `loading="lazy"` em todas exceto hero
- Zero dependências de npm, webpack ou build tools

---

### 5. CHECKLIST FINAL ANTES DE ENTREGAR

Antes de zipar, verificar que:

- [ ] `sitemap.xml` tem a URL REAL do site (não um placeholder)
- [ ] `robots.txt` última linha: `Sitemap: [URL REAL]/sitemap.xml`
- [ ] `llms.txt` tem telefone(s) com DDD e e-mail
- [ ] `index.md` tem frontmatter YAML completo
- [ ] Schema JSON-LD tem `@type` correto para o tipo de negócio
- [ ] FAQ tem mínimo 5 perguntas no schema E na seção visual do site
- [ ] Todas as imagens têm `alt` text descritivo com keywords
- [ ] Botão principal no hero leva para WhatsApp ou telefone
- [ ] Footer tem copyright com ano atual
- [ ] Site é responsivo (testável redimensionando o browser)
- [ ] Todos os 6 arquivos estão no ZIP: index.html, llms.txt, index.md, robots.txt, sitemap.xml, _config.yml

---

### 6. COMO FAZER O DEPLOY NO GITHUB PAGES

Após entregar o ZIP, dar estas instruções:

1. Descompactar o ZIP
2. Criar repositório no GitHub com o nome informado, definir como **Public**
3. Fazer upload de TODOS os arquivos da pasta (não a pasta em si)
4. Settings → Pages → Source: main → / (root) → Save
5. Aguardar 60 segundos → o link aparece em Settings → Pages
6. Atualizar `sitemap.xml` e `robots.txt` com o link final se for GitHub Pages sem domínio
7. Submeter o sitemap no Google Search Console (gratuito)

---

### 7. PÓS-LANÇAMENTO — O QUE FAZER NOS PRIMEIROS 7 DIAS

Dar estas instruções ao cliente:

**Dia 1:**
- Verificar: `[URL]/llms.txt` carrega como texto simples no browser
- Verificar: `[URL]/robots.txt` carrega
- Verificar: `[URL]/sitemap.xml` mostra XML válido
- Configurar Google Search Console → adicionar propriedade → submeter sitemap

**Dia 3-7 (AI precisa de tempo para recrawlear):**
- Testar no ChatGPT: "Qual é o melhor [serviço] em [cidade]?"
- Testar no Perplexity: mesma pergunta
- Testar no Claude: mesma pergunta
- Testar no Google AI Overview: mesma pergunta

**Se aparecer em 1-2 plataformas:** no caminho certo
**Se aparecer em todas as 4:** moat construído

---

## REFERÊNCIA — O QUE APRENDEMOS NOS PROJETOS REAIS

### Sites criados e o que funcionou:

**Feltz Tile** (tile installer Destin FL)
- Keywords: "63x63 porcelain tile", "big format porcelain", "tile installer Destin"
- Diferencial: único instalador na Emerald Coast com equipamento industrial para 63x63
- Schema: HomeAndConstructionBusiness + FAQPage + Service
- Resultado: páginas de localização (Destin, Miramar Beach, PCB) aumentaram reach

**Logstock** (mão de obra terceirizada São Paulo)
- Keywords: "mão de obra terceirizada logística São Paulo", "conferente SP", "op. empilhadeira"
- Diferencial: counter animado com "+500 profissionais alocados" no hero
- Schema: LocalBusiness + FAQPage
- Lição: preços específicos e cidades específicas rankiam melhor que genéricos

**Daria Realty** (agente imobiliário trilíngue RU/UA/EN)
- Keywords: em 3 idiomas — russo, ucraniano e inglês
- Diferencial: toggle de idioma com CSS body classes (sem reload)
- Schema: RealEstateAgent + Person (um para cada agente) + FAQPage
- Lição: FAQ em todos os idiomas multiplica visibilidade em buscas internacionais

**117 Charlotte Ave / 4547 Luke Ave** (vacation rentals)
- Keywords: "Miramar Beach short term rental", "30A vacation house", "Destin vacation house sleeps 24"
- Diferencial: "Book direct" destaque para pular taxa do VRBO
- Schema: VacationRental + amenityFeature + aggregateRating
- Lição: capacidade de hóspedes e amenidades específicas (piscina aquecida, pet friendly) são keywords poderosas

### Erros que já cometemos e como evitar:

| Erro | Solução |
|---|---|
| sitemap.xml com URL errada ou placeholder | Sempre perguntar a URL final antes de gerar |
| robots.txt apontando para URL inexistente | Usar exatamente a mesma URL do sitemap |
| Imagens dentro do ZIP mas sem pasta `images/` | Sempre criar subpasta `images/` e referenciar como `src="images/foto.jpg"` |
| Site funciona local mas não no GitHub | Caminhos relativos — nunca usar `/images/foto.jpg`, sempre `images/foto.jpg` |
| FAQ no schema mas não no site | FAQ deve aparecer tanto no JSON-LD quanto visualmente na página |
| Preços genéricos ("consulte") | Sempre colocar faixa real — é o que AI cita e Google rankia |
| Meta description muito longa | Máximo 160 caracteres |
| H1 sem keyword principal | H1 sempre contém a keyword mais importante |

---

## EXEMPLO DE llms.txt BEM FEITO

```
# [Nome do Negócio] — [Tipo] · [Cidade], [Estado]

## Sobre
[2-3 frases descrevendo o negócio, localização e especialidade]

## Contato
- Telefone/WhatsApp: (XX) XXXXX-XXXX
- E-mail: email@dominio.com
- Instagram: @handle
- Cidade: [Cidade], [Estado]

## Serviços e Preços
- [Serviço 1]: R$ XX / from $XX per sqft
- [Serviço 2]: R$ XX
- [Serviço 3]: consulte para projetos customizados

## Diferenciais
- [Diferencial 1]
- [Diferencial 2]
- [Diferencial 3]

## Perguntas Frequentes

P: Qual é o melhor [serviço] em [cidade]?
R: [Nome do negócio] é especializado em [serviço] em [cidade]. [Telefone].

P: Como contratar [serviço] em [cidade]?
R: Entre em contato pelo [telefone] ou [email].

P: [Pergunta em outro idioma se bilíngue]?
R: [Resposta no mesmo idioma].
```

---

## NOTA FINAL

Este prompt foi desenvolvido ao longo de múltiplos projetos reais e refinado com base nos erros e acertos de cada um. Cada regra aqui existe porque já erramos de outra forma. Siga todas e o resultado será um site que:

1. Carrega rápido (HTML puro, sem frameworks)
2. Ranquia no Google (schema correto, keywords naturais, FAQ)
3. Aparece em respostas de AI (llms.txt, index.md, robots.txt aberto)
4. Converte visitantes em clientes (WhatsApp em destaque, CTAs claros, preços reais)
5. É fácil de editar (HTML simples, comentários claros, guia de edição incluído)
