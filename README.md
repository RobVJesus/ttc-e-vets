# TTC e VETS - Posso ajudar?

Aplicativo estático (HTML + JSON) que organiza por tema as perguntas e
respostas publicadas no grupo de veteranos "TTC e Veteranos 2 / Posso
ajudar?". Segue o mesmo padrão dos outros projetos (Postagens Úteis, Balcão
de Negócios): `index.html` lê os dados de um arquivo `postagens.json`
publicado ao lado dele.

## Arquivos

- `index.html` — o aplicativo (também traz uma cópia dos dados embutida,
  usada somente se o `postagens.json` não puder ser carregado).
- `postagens.json` — os dados reais (categorias + perguntas/respostas).

## Sobre a privacidade dos remetentes

O grupo tem cerca de 370 participantes diferentes. Muitas mensagens foram
enviadas por números de telefone que não têm nome salvo no WhatsApp — ou
seja, o remetente aparece só como o número. Para não publicar números de
telefone de terceiros numa página pública, cada número foi substituído por
um identificador anônimo e sequencial ("Veterano #1", "Veterano #2" etc.),
mantendo consistência (o mesmo número sempre vira o mesmo identificador,
então ainda dá pra acompanhar quem respondeu o quê numa mesma conversa).

Remetentes que já usavam um apelido/identificação própria no grupo (ex.:
"TTC+Fulano", "5521-SO Mesquita") foram mantidos como estavam, já que são
identificações que os próprios usaram publicamente no grupo — mesmo padrão
já usado no Balcão de Negócios.

Se preferir um tratamento diferente (por exemplo, remover remetentes por
completo, ou anonimizar também os apelidos), me avise e eu ajusto.

## Como publicar no GitHub Pages

1. Crie um repositório (ex.: `ttc-vets-posso-ajudar`) em
   `github.com/RobVJesus`.
2. Envie `index.html` e `postagens.json` para a raiz do repositório.
3. Em **Settings → Pages**, habilite o GitHub Pages (Source: "Deploy from a
   branch", branch `main`, pasta `/ (root)`).
4. Use o link que aparecer em **Settings → Pages** (com o botão "Visit
   site") — não digite o endereço de cabeça, pois nomes com acentos/espaços
   podem gerar um nome de repositório diferente do esperado.
5. Lembre-se: no plano gratuito do GitHub, o Pages só funciona com
   repositório **público**.

## Como salvar edições feitas no site

1. Use o site normalmente — pesquise, adicione, edite ou exclua perguntas,
   respostas e categorias.
2. Para tornar as mudanças permanentes, clique no botão **"JSON"** no topo
   da página — isso baixa um `postagens.json` atualizado.
3. Substitua o `postagens.json` do repositório pelo arquivo baixado e faça
   o commit.
