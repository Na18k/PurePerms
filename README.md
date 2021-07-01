# =========================================
# Em desenvolvimento
# =========================================

# General

PurePerms by 64FF00 is a permissions manager for PocketMine-MP. 

It can be used in conjunction with PureChat to display players groups in chat.

#Traduçao pt-BR

Tradução feita por Na18k

# Commands

Comando | Descrição | Permissão
--- | --- | ---
`/addgroup <group>` | Adiciona um novo grupo para a lista de grupos. | pperms.command.addgroup
`/addparent <target_group> <parent_group>` | Adiciona um grupo a lista de herança de outro grupo. | pperms.command.addparent
`/defgroup <group> [world]` | Permite que você defina um grupo padrão. | pperms.command.defgroup
`/fperms` | Encontrar permissões de um puglin em especifico | pperms.command.fperms
`/groups` | Mostra a lista de todos os grupos. | pperms.command.groups
`/grpinfo <group> [world]` | Mostra informações sobre um grupo. | pperms.command.grpinfo
`/listgperms <group> <page> [world]` | Mostra todas as permissões de um grupo. | pperms.command.listgperms
`/listuperms <player> <page> [world]` | Mostra todas as permissões de um usuário. | pperms.command.listuperms
`/ppinfo` | Mostra informações sobre PurePerms. | pperms.command.ppinfo
`/ppsudo <login / register>` | Registrar ou fazer login na sua conta Noeul. | pperms.command.ppsudo
`/ppreload` | Reloads all PurePerms configurations. | pperms.command.ppreload
`/rmgroup <group>` | Removes a group from the groups list. | pperms.command.rmgroup
`/rmparent <target_group> <parent_group>` | Removes a group from another group inheritance list. | pperms.command.rmparent
`/setgperm <group> <permission> [world]` | Adds a permission to the group. | pperms.command.setgperm
`/setgroup <player> <group> [world]` | Sets group for the user. | pperms.command.setgroup
`/setuperm <player> <permission> [world]` | Adds a permission to the user. | pperms.command.setuperm
`/unsetgperm <group> <permission> [world]` | Removes a permission from the group. | pperms.command.unsetgperm
`/unsetuperm <player> <permission> [world]` | Removes a permission from the user. | pperms.command.unsetuperm
`/usrinfo <player> [world]` | Shows info about a user. | pperms.command.usrinfo

# Config

``` YAML

# PurePerms by 64FF00 (xktiverz@gmail.com, @64ff00 for Twitter)

# 제 블로그 이외에 허락없이 마음대로 플러그인 배포하실 시에는 바로 한국어 파일 삭제 조치하고 공유 중단합니다

---
# Set default data provider for PurePerms
# - mysql, yamlv1, yamlv2
data-provider: yamlv1

# Set the default language for PurePerms (<3)
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
default-language: en

# Disable /op permission for all players
# - true / false
disable-op: true

# Setting this option will allow you to use per-world permissions
# - true / false
enable-multiworld-perms: false

# Enables 'Noeul', a 'pointless' security management system for PurePerms
# - true / false
enable-noeul-sixtyfour: false

# MySQL Settings (Only configure this if you are going to use MySQL data provider)
mysql-settings:
  host: "PurePerms-FTW.loveyou.all"
  port: 3306
  user: "YourUsernameGoesHere"
  password: "YourPasswordGoesHere"
  db: "YourDBNameGoesHere"
  
# Sets a minimum length for a Noeul password when registering a new account
# - int  
noeul-minimum-pw-length: 6
  
# Special thanks to @jazzwhistle for helping me with this cool feature! #JAZZWHISTLE-FTW
# Ranks that can only be set on console
# Also, users with a superadmin-rank can only have their rank changed on console
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

# Features

- Set up permissions for different groups!
- Multi-group inheritance system to allow you to inherit group permissions
- Multi-language support, just choose your favorite language in config.yml! (Currently supports Czech, English, German, Korean, Japanese, Russian, Italian, Indonesian, Slovak, Spanish, Turkish, and Ukrainian! :D)
- Supports YAML + MySQL providers
- Provides simple and flexible PurePerms API for plugin developers
- And so on... ;)
