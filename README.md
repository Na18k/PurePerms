# =====================
# Em desenvolvimento a tradução
# =====================

# Geral

PurePerms by 64FF00 is a permissions manager for PocketMine-MP. 

It can be used in conjunction with PureChat to display players groups in chat.
=========================
Traduçao pt-BR

Tradução feita por Na18k
=========================

# Comandos

Comando | Descrição | Permissão
--- | --- | ---
`/addgroup <group>` | Adiciona um novo grupo para a lista de grupos. | pperms.command.addgroup
`/addparent <target_group> <parent_group>` | Adiciona um grupo à lista de herança de outro grupo. | pperms.command.addparent
`/defgroup <group> [world]` | Permite que você defina um grupo padrão. | pperms.command.defgroup
`/fperms` | Encontrar permissões de um puglin em especifico | pperms.command.fperms
`/groups` | Mostra a lista de todos os grupos. | pperms.command.groups
`/grpinfo <group> [world]` | Mostra informações sobre um grupo. | pperms.command.grpinfo
`/listgperms <group> <page> [world]` | Mostra todas as permissões de um grupo. | pperms.command.listgperms
`/listuperms <player> <page> [world]` | Mostra todas as permissões de um usuário. | pperms.command.listuperms
`/ppinfo` | Mostra informações sobre PurePerms. | pperms.command.ppinfo
`/ppsudo <login / register>` | Registrar ou fazer login na sua conta Noeul. | pperms.command.ppsudo
`/ppreload` | Recarrega todas as configurações do PurePerms. | pperms.command.ppreload
`/rmgroup <group>` | Remove um grupo da lista de grupos. | pperms.command.rmgroup
`/rmparent <target_group> <parent_group>` | Remove um grupo da lista de herança de outro grupo. | pperms.command.rmparent
`/setgperm <group> <permission> [world]` | Adiciona uma permissão à um grupo. | pperms.command.setgperm
`/setgroup <player> <group> [world]` | Define um grupo para um usuário | pperms.command.setgroup
`/setuperm <player> <permission> [world]` | Adiciona uma permissão a um usuário. | pperms.command.setuperm
`/unsetgperm <group> <permission> [world]` | Remove uma permissão de um grupo. | pperms.command.unsetgperm
`/unsetuperm <player> <permission> [world]` | Remove uma permissão de um usuário. | pperms.command.unsetuperm
`/usrinfo <player> [world]` | Mostra informações de um usuário. | pperms.command.usrinfo

# Configurações

``` YAML

# PurePerms by 64FF00 (xktiverz@gmail.com, @64ff00 for Twitter)

# 제 블로그 이외에 허락없이 마음대로 플러그인 배포하실 시에는 바로 한국어 파일 삭제 조치하고 공유 중단합니다

---
# Definir o provedor de dados padrão do PurePerms
# - mysql, yamlv1, yamlv2
data-provider: yamlv1

# Defina o idioma padrão do PurePerms (<3)
# - en, ko, jp, ru, ua, it, sp, cz, sk, de, idn, tr, pt-BR
# English message resource by @64FF00 and @Samueljh1 (GitHub)
# Korean message resource by @64FF00 (GitHub)
# Japanese message resource by @onebone and @haniokasai (GitHub)
# Russian message resource by @vvzar and @Pub4Game (GitHub)
# Ukrainian message resource by @samalero (GitHub)
# Italian message resource by @AryToNeX (GitHub)
# Spanish message resource by @iksaku and @JoahDave (Github) 
# Czech message resource by @Michael2010117 (GitHub)
# Slovak message resource by @Michael2010117 (GitHub)
# German message resource by @Exxarion (GitHub)
# Indonesian message resource by @DevillordMCPE (GitHub)
# Turkish messages resource by @PainTR (GitHub)
# Portuguese messages resource by @Na18k (GitHub)
default-language: pt-BR

# Desativar a permissão /op para todos os players
# - true / false
disable-op: true

# Essa opção permitirá que você use permissões por mundo
# - true / false
enable-multiworld-perms: false

# Habilita 'Noeul', um sistema de gerenciamento de segurança 'sem sentido' ao PurePerms
# - true / false
enable-noeul-sixtyfour: false

# Configurações MySQL (Configure isso apenas se for usar um provedor de dados MySQL)
mysql-settings:
  host: "PurePerms-FTW.loveyou.all"
  port: 3306
  user: "SeuUsuarioVaiAqui"
  password: "SuaSenhaVaiAqui"
  db: "SeuNomeDeBancoDeDadosVaiAQui"
  
# Define o comprimento mínimo para uma senha Noeul ao registrar uma nova conta
# - int  
noeul-minimum-pw-length: 6
  
# Agradecimentos especiais a @jazzwhistle por ter ajudado com esse recurso legal! #JAZZWHISTLE-FTW
# Classificações que só podem ser definidas no console
# Além disso, os usuários com uma classificação de superadministrador só podem ter sua classificação alterada no console 
# - array
superadmin-ranks: ["OP"]
```

```
YAML
---
Guest:
  alias: 'gst'
  isDefault: true
  inheritance: []
  permissions:
  - -essentials.kit
  - -essentials.kit.other
  - -pocketmine.command.me
  - pchat.colored.format
  - pchat.colored.nametag
  - pocketmine.command.list
  - pperms.command.ppinfo
  worlds: []
```

# Características

- Configure permissões para diferentes grupos!
- Sistema de herança multi-grupo para permitir que você herde as permissões do grupo
- Suporte Multi-linguagem, basta escolher seu idioma favorito em config.yml! (Suporta atualmente Czech, English, German, Korean, Japanese, Russian, Italian, Indonesian, Slovak, Spanish, Turkish, Ukrainian and Portuguese! :D)
- Suporte a provedores YAML + MySQL
- PurePerms fornece uma API simples e flexível para desenvolvedores de plug-ins
- E muito mais... ;)
