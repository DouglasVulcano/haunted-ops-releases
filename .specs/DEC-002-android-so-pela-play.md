---
id: DEC-002
titulo: Android só pela Google Play, sem APK público
estado: ativa
aplica: []
palavras: [android, apk, google play, pago, integrity, decisão]
depende: []
atualizado: 2026-10-16
conferido: dedd663
---
## Regra
Decidido pelo dono em 14/out/2026 (ok ao plano de licença e reembolso, versão 0.16.14).
- Nenhum APK do jogo vai para a página de downloads. O Android é só pela Google Play (teste fechado hoje).
- O `latest.json` sai com `android: null` e o README aponta o Android para o grupo de testadores.
- O APK de teste (lado a lado) continua só para uso local, nunca publicado.

## Por quê
O jogo da Play é pago e confere a compra no login (Play Integrity). Um APK público seria o jogo de graça, por fora
da Play. O APK da 0.16.13 foi apagado da release pública no mesmo dia.

## Conferir
`prototipo/tools/release.ps1` no jogo (`android = $null`); a release atual não tem `.apk`.
