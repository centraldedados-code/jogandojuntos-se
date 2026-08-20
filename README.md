# Jogando Juntos SE - Portal de Monitoramento

Pasta pronta para publicar no GitHub Pages, no mesmo padrao dos outros
sistemas do Instituto BR Arte (Prospera Nacional, Jogando Juntos RJ etc).

## Conteudo desta pasta

```
jogandojuntos-se/
  index.html                          <- portal (senha, dashboard, territorios, metas, pastas)
  assets/
    logo-instituto-br-arte.png        <- logo do Instituto BR Arte
    logo_laranja.png                  <- logo Jogando Juntos pela Cidadania
```

## Como publicar

1. Crie (ou reaproveite) um repositorio no GitHub da organizacao, por
   exemplo `centraldedados-code/jogandojuntos-se`.
2. Suba esta pasta inteira para a raiz do repositorio (pode ser via
   upload direto pela interface do GitHub, ou `git add` / `git commit`
   / `git push` se preferir linha de comando).
3. No repositorio, va em **Settings > Pages** e ative o GitHub Pages
   apontando para a branch `main` (ou `master`), pasta raiz (`/`).
4. O GitHub gera uma URL parecida com:
   `https://centraldedados-code.github.io/jogandojuntos-se/`
5. Confirme que essa URL bate com os caminhos ja usados dentro do
   `index.html` (`src="https://centraldedados-code.github.io/jogandojuntos-se/assets/..."`).
   Se o nome do repositorio ou da organizacao for diferente do que eu
   assumi aqui, troque esses dois caminhos no `index.html` (dentro da
   tag `<img>` da tela de senha e do cabecalho) para bater com a URL
   real gerada pelo GitHub Pages.

## Senha de acesso

A senha configurada no `index.html` (constante `SENHA`) e no `Setup.gs`
(aba CONFIG) e `Brarte@2026`, igual aos outros sistemas da familia.

## URL da API (Apps Script)

Ja preenchida na constante `APPS_SCRIPT_URL` do `index.html` com a URL
de implantacao que voce testou:
`https://script.google.com/macros/s/AKfycby789JHX9xEq4biIPqWphv29reXNz2Z3u8pCRSgrcfqh1nrihs2tKaJ8H7KoF9wYjoDpQ/exec`

Se voce gerar uma nova implantacao (nova URL, nao so nova versao), vai
precisar atualizar essa constante e subir o `index.html` de novo.
