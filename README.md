# Haunted Ops · releases

**Soldados contra fantasmas.** FPS de bomba 5v5 em low poly. Os soldados defendem os locais A e B com pistola e fumaça. Os fantasmas somem quando param, atacam com faca e tentam plantar a bomba.

Este repositório tem só as **versões para baixar** (executáveis, notas e hashes). O código do jogo é privado.

## Baixar

➡️ **[Última versão para Windows](https://github.com/DouglasVulcano/haunted-ops-releases/releases/latest/download/HauntedOps-Windows.zip)**

Todas as versões ficam em [Releases](https://github.com/DouglasVulcano/haunted-ops-releases/releases).

| Arquivo | Para quê |
|---|---|
| `HauntedOps-Windows.zip` | O jogo. Descompacte e abra `HauntedOps.exe`. |
| `HauntedOpsServer-linux-x86_64.zip` | Servidor dedicado (Linux) para hospedar salas. |
| `SHA256SUMS.txt` | Hashes para conferir se o download não foi alterado. |
| `latest.json` | Versão, data e hashes em formato de máquina. |

### Conferir o download (opcional)
```powershell
Get-FileHash .\HauntedOps-Windows.zip -Algorithm SHA256
```
Compare com a linha do arquivo em `SHA256SUMS.txt`.

### Aviso do Windows
O executável ainda não é assinado digitalmente. Se aparecer "O Windows protegeu o computador", clique em **Mais informações** e depois em **Executar assim mesmo**.

## Como jogar
- **Jogar agora:** entra numa sala da rede local ou num servidor oficial (São Paulo). O servidor oficial liga quando alguém entra (cerca de 1 min na primeira vez) e desliga sozinho quando fica vazio.
- **Entrar com código:** cole o código da sala que um amigo mandou (ex.: `60N09-947SQ`).
- **Criar sala:** escolha as regras e mande o código para os amigos.

| Tecla | Ação |
|---|---|
| WASD / Espaço | mover / pular |
| Shift / Ctrl | andar em silêncio / agachar |
| Mouse esquerdo / direito | atirar ou corte / estocada |
| R / F | recarregar / inspecionar |
| C | fumaça (soldado) ou névoa (fantasma) |
| E / G | plantar ou desarmar / largar a bomba |
| Tab | placar |

**Requisitos:** Windows 10 ou 11, 64 bits, placa de vídeo com Vulkan.

## Versões
Veja o [CHANGELOG](CHANGELOG.md). Todos na mesma sala precisam da mesma versão.
