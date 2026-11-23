# Nova Tiers Mod — Minecraft 1.21.11 (Fabric)

Mod oficial cliente para **Minecraft Java Edition 1.21.11 (Fabric)** que exibe os rankings da **Nova Tiers** diretamente no jogo.

## Recursos
- **Nametags em tempo real:** Mostra a tag de tier colorida (`[HT1]`, `[LT2]`, etc.) acima da cabeça dos jogadores avaliados.
- **Tab List:** Exibe o tier ao lado de cada jogador na lista do Tab (`PlayerListHud`).
- **Todos os 9 modos oficiais:** `overall`, `vanilla` (Crystal), `sword`, `uhc`, `nethpot`, `smp`, `axe`, `diapot`, `mace` e `spearmace` (Spear Mace).
- **Comandos no Chat:**
  - `/tier <nick>` ou `/novatiers lookup <nick>` — Mostra pontuação total, patente, região, guilda e todos os tiers do jogador.
  - `/novatiers mode <modo>` — Escolhe qual modo aparece nas nametags e no Tab (`overall`, `vanilla`, `sword`, `uhc`, `nethpot`, `smp`, `axe`, `diapot`, `mace`, `spearmace`).
  - `/novatiers toggle` — Ativa/desativa o mod.
  - `/novatiers toggle nametag` | `tab` | `points` — Personaliza onde os badges aparecem.
  - `/novatiers refresh` — Atualiza a lista imediatamente do servidor Nova Tiers.
  - `/novatiers url <link>` — Altera a URL da API do seu site Nova Tiers.

## Como compilar o `.jar` (Java 21)
1. Instale o **Java 21 (Eclipse Temurin JDK 21)** e o **Gradle** (ou gere o wrapper com `gradle wrapper`).
2. Na pasta do projeto, execute:
   ```bash
   gradle build
   ```
   *(ou `./gradlew build` se estiver usando o Gradle Wrapper).*
3. O arquivo compilado estará em `build/libs/novatiers-mod-1.21.11-1.0.0.jar`.
4. Copie esse `.jar` junto com o **Fabric API 1.21.11** para a pasta `.minecraft/mods/`.

## Configuração (`config/novatiers.json`)
Na primeira inicialização, o mod cria `config/novatiers.json` já apontando para o servidor da Nova Tiers.
