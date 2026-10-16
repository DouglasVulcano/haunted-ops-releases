---
id: PUB-002
titulo: Trechos gerados e fotos do README
estado: ativa
aplica: [README.md, .github/**]
palavras: [eco, gerado, mapas-fotos, mapas-lista, fotos, jpg, banner, ecossistema.json]
depende: [PUB-001]
atualizado: 2026-10-16
conferido: dedd663
---
## Regra
- Dois trechos do `README.md` são GERADOS pela central a partir de `haunted-ops-devkit/ecossistema/ecossistema.json`
  (campo `releases` de cada mapa: `foto`, `alt`, `legenda`, `frase`):
  - entre `<!-- eco:mapas-fotos -->` e `<!-- /eco:mapas-fotos -->`: a tabela de fotos, duas por linha;
  - a linha que termina com `<!-- eco:mapas-lista -->`: "Quatro mapas: ..." (o resto da linha é trocado).
- Não editar à mão: mudar na ficha e rodar `python ../haunted-ops-devkit/ecossistema/eco.py gerar --repo releases`.
  Entram os mapas no menu e marcados `divulgado`; o que ainda não chegou ao PC e à Play ganha "(chega na versão X)".
- Fotos dos mapas em `.github/<mapa>.jpg`: JPG 960x530, capturas do jogo atual (as de hoje têm de 41 a 70 KB).
- Banner `.github/banner.jpg`: 1280x640, com link para o site. Mudou a cara de um mapa que está no banner (hoje o
  Pátio de Armas do Castelo): refazer o banner.
- Foto que deixou de ser usada sai de `.github/`.
- O resto do README (Baixar, lista do jogo, Sobre este repositório) é texto daqui e se edita à mão.

## Por quê
16/out o README ganhou os quatro mapas com fotos do jogo atual, e os textos de mapa passaram a vir da ficha única
para não ficarem diferentes do site e do jogo.

## Conferir
`python ../haunted-ops-devkit/ecossistema/eco.py conferir --repo releases`.
