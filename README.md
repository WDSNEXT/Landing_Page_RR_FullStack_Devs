<p align="center">
  <a href="https://rrdevsfullstack.netlify.com/">
    <img src="https://rrdevsfullstack.netlify.com/assets/img/logo.svg" alt="RR FullStack Devs" width="150">
  </a>
</p>

<h3 align="center">RR FullStack Devs</h3>

<p align="center">
  Comunidade de Developers FullStack do estado de Roraima.
  <br>

<a href="https://rrdevsfullstack.netlify.com/"><strong>-- #Bora. Participe! --</strong></a>
<br>
<br>

  <a href="https://app.netlify.com/sites/rrdevsfullstack/deploys">
    <img src="https://api.netlify.com/api/v1/badges/7a65b587-5cb4-4e92-9a01-3f4291934841/deploy-status" alt="Netlify Status">
  </a>

  <a href="https://david-dm.org/WDSNEXT/Landing_Page_RR_FullStack_Devs" title="dependencies status">
    <img src="https://david-dm.org/WDSNEXT/Landing_Page_RR_FullStack_Devs/status.svg"/>
  </a>

  <a href="https://david-dm.org/WDSNEXT/Landing_Page_RR_FullStack_Devs?type=dev" title="devDependencies status">
    <img src="https://david-dm.org/WDSNEXT/Landing_Page_RR_FullStack_Devs/dev-status.svg"/>
  </a>
</p>

## Iniciando

Leia todo o [README](https://github.com/WDSNEXT/Landing_Page_RR_FullStack_Devs/blob/master/README.md) para obter todas as informacoes
sobre como usar e personalizar este template.

-[Baixe a versao mais recente](https://github.com/WDSNEXT/Landing_Page_RR_FullStack_Devs) do RR FullStack Devs diretamente do GitHub official da Comunidade.
-Clone o repositorio: `git clone https://github.com/WDSNEXT/Landing_Page_RR_FullStack_Devs.git`.

## Documentacao

Para executar todos os scripts voce precisar ter instalado localmente em sua maquina o NodeJs. Caso nao tenha instalado [baixe aqui](https://nodejs.org/en/download/) e instale.

### Executando o projeto localmente

Execute a instalacao das dependencias. Em seguida execute o servidor local:

```bash
npm install
npm run start
```

Como servidor local usamos o [BrowserSync](https://www.browsersync.io/). Lembrando que ao usar o BrowserSync ele nos dara a possibilidade de
abrir o projeto local `http://localhost:3000` e tambem a todos os dispositivos conectados a sua rede local `http://seuip:3000`. Aproveite e acesse o projeto
via smartphone para ver se nao a erros na parte Responsiva do site ou abra em outro computador. Ele mostrara no console o endereco a ser usado. Legal nao e.

### Personalizando o projeto

Depois de instalado as dependencias e ver o projeto default rodando lindamente e hora e personalizar para ficar a seu gostos e para voce.
Abra o projeto no seu editor de codigo preferido. Uma dica para quem usa Visual Studio Code e so abrir o terminal na raiz do projeto e digitar `code .`

#### Estrutura do projeto

- `src/` Contem todos os arquivos nao compilados do projeto e nela que vc trabalhara sempre.
  - `assets/` Contem os arquivos estaticos usados no projeto(imagens, css).
    - `img` contem as imagens usadas no projeto.
    - `sass` Pasta importantissima, pois contem o arquivos que geraram o css final.
- `dist/` Sera gerada pelo script de build: `npm run build` e contera o projeto final pronto pra producao.
- `node-modules/` Pasta que contem todas as dependencias do projeto. Caso apague e so instalar novamente `npm install`

## Personalizando o Gradiente

Primeiramente abra o aquivos `_variables.scss` localizado em `/src/assets/sass/abstracts/_variables.scss`:

```sass
// GRADIENTE PAGE COLORS
$color-primary: #4A00EA;
$color-secondary: #8E2DE2;
```
No lugar das cores padrao substitua por cores que voce melhor gostar para criar o gradiente que ficara acima da imagem criando um efeito belissino.
Feito isso salve e veja se mudou no projeto final. Lembre-se de esta executando o script de desenvolvimento `npm run start` se nao estive execute
digitando o comando no terminal.

## Personalizando a imagem de fundo (background)

Para personalizar a imagem de fundo, primeiramente escolha uma imagem e salve-a em `/src/assets/img/`. Uma vez feito isso,
agora abra o `index.html` localizada em `/src/index.html`.

```html
  <div
      class="wallpaper wallpaper--filter"
      style="background-image: url('/assets/img/background@3x.jpg');background-size: cover;background-position: center;"
    >
      &nbsp;
  </div>
```

substitua `background@3x.jpg` pela imagem que voce escolheu. E salve.
