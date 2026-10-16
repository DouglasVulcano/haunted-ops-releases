---
id: DEC-001
titulo: Só a versão mais recente fica disponível
estado: ativa
aplica: []
palavras: [versão, latest, releases antigas, apagar, decisão]
depende: []
atualizado: 2026-10-16
conferido: dedd663
---
## Regra
Decidido pelo dono em 30/set/2026.
- A página de downloads mostra e guarda só a versão mais recente do jogo. As releases anteriores e as tags delas
  são apagadas assim que a nova está no ar (o `tools/release.ps1` do jogo faz isso).
- Ninguém baixa versão antiga: todos precisam da mesma versão para jogar juntos.

## Por quê
Versões diferentes não jogam juntas (versão de rede). O launcher e o servidor só usam a mais nova (`latest.json`).

## Conferir
`gh release list --repo DouglasVulcano/haunted-ops-releases` mostra uma release só.
