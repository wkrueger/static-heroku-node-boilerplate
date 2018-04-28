# static heroku node boilerplate

_Uma forma de hospedar uma página estática quebra-galho de grátis em poucos passos._

## Aqui nois vai

* Se você ainda não a possui, crie uma conta no [heroku](https://heroku.com).
* Se você ainda não o possui, instale o [heroku CLI](https://devcenter.heroku.com/articles/heroku-cli).

1.  Crie um projeto no heroku `heroku create <nome opcional>`. Anote o endereço git.
2.  Clone este repositório. `git clone https://github.com/wkrueger/static-heroku-node-boilerplate.git`
3.  Dentro da pasta clonada, adicione a origem remota do seu projeto heroku `git remote add heroku <endereco>.git`, usando o endereço anotado na etapa 1.
4.  Faça suas alterações, adicione seu html. Faça o _commit_ `git commit -m hello`.
5.  Publique. `git push heroku master`.

---

_A quick n'dirty way to publish free static assets to the web._

## Howto

* If you still don't have one, create a [heroku account](https://heroku.com).
* If you still dont't have it, install the [heroku CLI](https://devcenter.heroku.com/articles/heroku-cli).

1.  Create a heroku project `heroku create <optional-name>`. Write down the given git repo.
2.  Clone this repo. `git clone https://github.com/wkrueger/static-heroku-node-boilerplate.git`
3.  Inside the cloned folder, add the heroku git remote: `git remote add heroku <that-address>.git`, using the address from step 1.
4.  Make your changes, add your html, commit. `git commit -m hello`.
5.  Publish. `git push heroku master`.

---

## Under the hood:

* Creates a node.js project with the `http-server` dependency.
* Calls `http-server` through the procfile.

## Viability:

* Heroku web dyno is absolutely not designed to host this kind of application. Node and `http-server` are not the best way to serve static files. This is absolutely non-production.
* Free heroku dynos "sleep" when unused. There will be a startup time when idle.
