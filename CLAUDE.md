# haunted-ops-releases: a página pública de downloads do Haunted Ops

@../haunted-ops-devkit/ecossistema/REGRAS_COMUNS.md

Repositório PÚBLICO no GitHub. Guarda só o `README.md` (a página), as fotos em `.github/` e as
releases com os instaladores da versão mais recente. O código do jogo nunca vem para cá.

## Publicar
- **Push aqui publica a página na hora** para todo mundo: só com o ok dele.
- As releases são criadas pelo `tools/release.ps1` do jogo (`../haunted-ops`), que também apaga as anteriores.
  Não criar nem apagar release à mão.

## Vizinhos
- Central: `../haunted-ops-devkit` (ficha do ecossistema e `eco.py`). Jogo: `../haunted-ops`. Site: `../haunted-ops-site`.

## O que vem de fora (não editar à mão)
- Os blocos `<!-- eco:mapas-fotos -->` (tabela de fotos) e a linha que termina em
  `<!-- eco:mapas-lista -->` são GERADOS pela central. Mude a ficha
  (`../haunted-ops-devkit/ecossistema/ecossistema.json`) e rode
  `python ../haunted-ops-devkit/ecossistema/eco.py gerar`.

## Regras que já deram erro
- Nada de APK aqui: o Android é só pela Google Play (o jogo confere a compra no login).
- Os nomes dos arquivos da release não levam a versão: o link `.../releases/latest/download/...` do site
  sempre aponta para a mais nova.
- Foto nova em `.github/`: tirada do jogo atual, sem interface.

## Specs
Regra de um assunto: `grep -il <palavra> .specs/*.md` (ou o índice `.specs/INDEX.md`) e abra só o que casa.
Os lembretes de `.claude/rules/specs/` carregam sozinhos ao mexer nas pastas de cada spec.
