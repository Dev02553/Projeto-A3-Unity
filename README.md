🎮 Platformer 2D – Unity (Android) – Projeto Acadêmico “Mario-like”

Jogo de plataforma 2D feito em Unity (C#) visando Android. O projeto recria mecânicas clássicas de correr, pular, coletar moedas, inimigos simples, blocos interativos e fim de fase.

Nota legal: este projeto é apenas inspirado em jogos de plataforma. Não utiliza marcas ou personagens registrados. Use arte/áudio originais ou com licença livre (ex.: CC0/CC-BY) e credite em CREDITS.md.

✨ Funcionalidades

Moedas colecionáveis e HUD de pontuação

Inimigos com patrulha e derrota por salto

Blocos interativos (quebra/surpresa)

Power-ups genéricos (ex.: boost de pulo/velocidade)

Checkpoints e bandeira de conclusão

Controles touch (Android) + teclas no Editor

🧩 Estrutura recomendada
Assets/
  Scenes/          # MainMenu, Level1, GameOver, Victory
  Scripts/
    Core/          # GameManager, EventBus
    Player/        # Movimento, pulo, power-ups
    Enemies/       # IA simples (State)
    Items/         # Moedas, blocos, pickups
    UI/            # HUD
  Art/             # Sprites originais ou CC
  Audio/           # SFX/Música originais ou CC
  Prefabs/
Packages/
ProjectSettings/
UserSettings/

🛠️ Stack

Unity 2021/2022 LTS • C# • Android Build Support • Physics 2D

🚀 Como executar

git clone https://github.com/Dev02553/Projeto-A3-Unity.git

Abrir no Unity Hub (versão LTS recomendada).

Carregar Scenes/MainMenu e apertar Play.

Para Android: File ▸ Build Settings ▸ Android ▸ Build (IL2CPP, ARMv7/ARM64, minSdk ≥ 21).

📖 Extended Description

Player Controller: física 2D com coyote time opcional, amortecimento de input e checagem de piso.

Enemy AI (State): patrulha → colisão → derrotado. Inversão por “pinos” invisíveis.

Event Bus (Observer-like): HUD reage a OnCoinCollected, OnPowerUpPicked, OnCheckpoint.

Object Pooling: moedas/partículas para reduzir GC.

Config por dados: ScriptableObject para inimigos/power-ups.

GameManager: fluxo de fase, troca de cena, pause, contadores.

📜 Licença & Créditos

Licença sugerida: MIT (crie LICENSE).

Liste autores/links de arte/áudio em CREDITS.md.

Não inclua logos ou personagens de terceiros.

👨‍💻 Autor

David Silva Rodrigues

📝 README.md (EN)
🎮 Platformer 2D – Unity (Android) – Academic Mario-like

A 2D platformer made with Unity (C#) for Android. Classic mechanics: run, jump, coin collection, simple enemies, interactive blocks, stage goal.

Legal note: this project is inspired by platformers. Do not include protected brands/characters. Use original or open-licensed art/audio (e.g., CC0/CC-BY) and credit in CREDITS.md.

✨ Features

Collectible coins & score HUD

Patrol enemies, stomp to defeat

Interactive blocks (break/surprise)

Generic power-ups (jump/speed boost)

Checkpoints & goal flag

Touch controls (Android) + editor keys

🧩 Suggested structure

(same tree as PT section)

🛠️ Tech

Unity 2021/2022 LTS • C# • Android Build Support • 2D Physics

🚀 How to run

git clone https://github.com/Dev02553/Projeto-A3-Unity.git

Open with Unity Hub (LTS).

Load Scenes/MainMenu and Play.

Android: File ▸ Build Settings ▸ Android ▸ Build (IL2CPP, ARMv7/ARM64, minSdk ≥ 21).

📖 Extended Description

(same ideas as PT: Player Controller, State enemies, Event Bus, Pooling, ScriptableObjects, GameManager).

📜 License & Credits

MIT recommended. Put asset attributions in CREDITS.md. Avoid third-party IP.

👨‍💻 Author

David Silva Rodrigues

⚙️ .gitignore (Unity)

Crie um arquivo .gitignore na raiz contendo (trecho essencial):

[Ll]ibrary/
[Tt]emp/
[Oo]bj/
[Bb]uild/
[Bb]uilds/
[Ll]ogs/
[Mm]emoryCaptures/
Assets/AssetStoreTools*
*.csproj
*.sln
*.user
*.unityproj
*.pidb
*.suo
*.svd
*.pdb
*.apk
*.aab
*.keystore
.DS_Store
*.unitypackage


Se usar Addressables/cache, adicione as pastas correspondentes.

📦 Git LFS (recomendado para binários grandes)
git lfs install
git lfs track "*.png" "*.jpg" "*.wav" "*.mp3" "*.psd" "*.ttf"
git add .gitattributes
git add .
git commit -m "Init Unity project with LFS"
git push origin main

🧹 Sobre os assets que você subiu

No repo atual aparecem imagens com marca/sprite do Mario e backgrounds de Super Mario World. Esses materiais são protegidos por direitos autorais e não são adequados para um repositório público. Troque por:

CC0/CC-BY (ex.: OpenGameArt, Kenney, Itch asset packs gratuitos);

Arte original feita por você.

(Se quiser, eu listo 3–5 packs CC0 populares pra plataforma 2D e já monto um CREDITS.md.)

▶️ Próximos passos práticos

Abra o seu projeto Unity local e confirme que possui: Assets/, Packages/, ProjectSettings/.

Remova do repositório os arquivos com IP de terceiros.

Adicione o .gitignore e habilite Git LFS.

git add . → git commit -m "Initial Unity project" → git push.

Substitua as artes por CC0/autorais e crie LICENSE + CREDITS.md.

Cole o README.md acima na raiz do repo.

Quer que eu já te entregue um CREDITS.md padrão + LICENSE (MIT) e uma seção de screenshots apontando para as imagens certas? Também posso sugerir packs CC0 que combinam com estética “retro/platformer”.
