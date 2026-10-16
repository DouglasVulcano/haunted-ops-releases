---
id: PUB-001
titulo: O que a página de downloads é
estado: ativa
aplica: [README.md, .github/**]
palavras: [releases, github, readme, instaladores, latest, latest.json, windows, macos, source code]
depende: [DEC-001, DEC-002]
atualizado: 2026-10-16
conferido: dedd663
---
## Regra
- Repositório público `DouglasVulcano/haunted-ops-releases`: só o `README.md` (a página) e as imagens em `.github/`.
  O código do jogo nunca entra; o "Source code" que o GitHub põe em cada release é este repositório.
- As releases são feitas pelo `tools/release.ps1` do jogo, nunca à mão: nasce rascunho, confere a quantidade de
  arquivos, publica como `latest` e apaga as releases e tags anteriores. Fica só a versão mais recente.
- Arquivos de cada release, sem versão no nome (os links `releases/latest/download/<arquivo>` não mudam):
  `HauntedOps-Setup.exe` (instalador do Windows, atualiza o jogo a cada abertura), `HauntedOps-Windows.zip`,
  `HauntedOps-Setup-macOS.zip` e `HauntedOps-macOS.zip` (quando há Mac), `HauntedOpsServer-linux-x86_64.zip` e
  `latest.json` (versões, versão de rede e SHA-256, lido pelo launcher e pelo servidor). Renomear quebra a
  atualização.
- Android não sai aqui (DEC-002): só pela Google Play. Versão só de Android não gera release; a versão desta página
  é a do PC.
- As notas da release (`docs/releases/v<versão>.md` do jogo) também aparecem no site (SITE-006 do site): markdown
  simples.
- Push neste repositório e release nova são ações para fora: só com o ok do dono na hora.

## Por quê
30/set: todos precisam da mesma versão para jogar juntos, e só a versão atual fica disponível. 14/out: o jogo da
Play passou a ser pago e a conferir a compra no login.

## Conferir
`prototipo/tools/release.ps1` no repositório do jogo; `gh release list --repo DouglasVulcano/haunted-ops-releases`
deve mostrar uma release só.
