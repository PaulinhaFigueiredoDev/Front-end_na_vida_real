# CSShortcut

> Um espaço para organizar e demonstrar estudos de desenvolvimento front-end.

## Stack

- Task Runner: [Gulp](https://gulpjs.com/docs/en/getting-started/quick-start/)
- HTML Template Engine: [Pug](https://pugjs.org/api/getting-started.html)
- CSS Preprocessador: [Stylus](https://stylus-lang.com)

## Executar localmente

**1 -** Instale as dependências:
```sh
$ npm install
```

**2 -** Inicie o servidor com livereload:
```sh
$ npm start
```

Para gerar os arquivos finais em `out/`, use `npm run build`.

## Folders Structure

	.
	├── README.md
	├── LICENSE.md
	├── CONTRIBUTING.md
	├── out/
	├── src/
	|   ├── icons/
	|   ├── assets/
	|   |   ├── img/
	|   |   ├── scripts/
	|   |   |   └── script.js
	|   |   └── styles/
	|   |       ├── modules/
	|   |       └── style.styl
	|   ├── partials/
	|   |   ├── footer.pug
	|   |   └── header.pug
	|   ├── layouts/
	|   |   └── default.pug
	|   ├── projects.pug
	|   └── index.pug
	├── gulpfile.js
	├── package.json
	├── projects.json
	├── .editorconfig
	└── .gitignore

## Automatic Tasks

- `$ npm run build`: Compila Pug, Stylus e imagens para `out/`.
- `$ npm start`: Observa alterações e inicia o servidor local.

## Versioning

To keep better organization of releases we follow the [Semantic Versioning 2.0.0](http://semver.org/) guidelines.

## Próximos passos

- adicionar exemplos interativos dos exercícios de JavaScript;
- publicar uma demonstração online;
- ampliar a cobertura de acessibilidade e testes.

## Licença
Este projeto está disponível sob a licença MIT.
