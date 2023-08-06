<div align="center">
  <img src="https://github.com/Kocaki182/ServerUI-N/assets/129764133/6b6b60f5-d2d3-4040-b8fa-067105c0154a" alt="ServerUI"/>
  <h3 align="center"><u>ServerUI-N Docs</u></h3>

  <p align="center">
    <a href="https://github.com/Kocaki182/ServerUI-N/issues">Report Bug/issue</a>
    •
    <a href="https://github.com/Kocaki182/ServerUI-N/issues">Request</a>
  </p>
</div>
<a href="https://www.mediafire.com/file/1o2k9lcvim6nt21/SERVER_UI_N_v15.zip/file">Download ServerUI N V15 Here</a>
<h3>Addon Depend : Nakata ServerUI</h3>
<h3>MePlaud : @Nperma</h3>
<h3>Contribute :</h3>
<li><a>@Void(0)</a></li>
<li><a href="https://discord.gg/mgMdzHZe">SkyBound Community</a></li>


<detail>
<h3>List</h3>
<li><a href="#features">Features</a></li>
<li><a href="#taglist">List Tag</a></li>
<li><a href="#rebuilt">Rebuilt</a></li>
<li><a href="#fixed">Fixed</a></li>
<li><a href="#disabled-features">Disabled Features</a></li>
<li>
<a href="#guild-ui-testing">Guild-UI</a>
</li>
<li><a href="#betterrtp">RTP (void(0))</a></li>
<li><a href="#info">Info-Setting</a></li>
  <li><a href="#onlinepoint-setting">onpPRIZE-setting</a></li>
</detail>

### Update V14.5
- nerf warp (add cooldown)
- nerf home (add cooldown & cancel isMoving)
- Improved NickSystem
- add ID
- add button visible_id(menu/nickUI)
- add button iduserlist(adminmenu/chat)
### Update V15
- Rebuilt ScoreboardSetting [scsetting](#scoreboardsetting)
- Improved & Rebuilt RankList(show TagAcces if player HasTag("admin"))

### Features
inludes ServerUI V11 [ServerUI Nakata DC](https://discord.gg/pwfPKMpx)
- BetterRTP (AntiKepentok)
- Invsee (Only support Inventory)
- NickUI
- GuildUI
- OnlineUI
<br />

### Rebuilt
- HomeSystem (Change to Database & support all dimension)
- WarpSystem (Change to Database)
- ChatSystemUI (change to Database & not used ability mute now)
<br />

### Fixed
- MaskShop
- MessageSystem
<br />

### Disabled Features
- ClearLag (command) <on|off|clear>
- SudoSystem
- RandomTeleportToPlayer
<br />

### TagList
- WarpTag
```mcfunction
tag (selector/objectname) add warp_ui
```
- HomeTag
```mcfunction
tag (selector/objectname) add home_ui
```
- InfoTag
```mcfunction
tag (selector/objectname) add info_ui
```
- RtpTag
```mcfunction
tag (selector/objectname) add rtp_p
```
- RankTag
```mcfunction
# PrefixTag = "rank:"
tag (selector/objectname) add rank:(rankName)
```
- NickUI
```mcfunction
#Permission to acces UI "nickPerm"
#Permission OpenUI "nick_ui"
```
- OnlineUI
```mcfunction
tag (selector/objectname) add on_ui
```
<br />

### 🛡Guild-UI [testing]
- ### No have Guild
- create
- join
- ### Has Guild
- invite [unless member]
- kick [Founder]
- promotecofounder [Founder]
- promoteelder [Founder & CoFounder]
- joinlog
- showmemberlist
- chat-guild
- Quit [unless founder]
<br />

### BetterRTP
```mcfunction
#You can rtp With addTag "rtp_p"
#You can add command into npc
# CD 10sec

#Copy this command and add to npc
tag @initiator add rtp_p

#Based
tag @s add rtp_p
```
<br />

### INFO
filepath : scripts/mainMenu/modules/info.js
```javascript
/**
 * Check Docs @minecraft/server-ui or @JaylyDev
 */
 
 /**
  * module : "import { ActionFormData } minecraft/server-ui"
  * ActionFormData
  * title
  * body
  * button
  * 
  * example:
  * const form = new ActionFormData()
  * .title("Tutorial")
  * .body("Follow TT @Npolose\nMekimek")
  * .button("exit");
  * form.show(this.object/player); or form.show(this.object/player).then(res => {})
  * 
  * 
  * @module : import { ModalFormData } from "@minecraft/server-ui"
  * @ModalFormData
  * title
  * textField
  * dropdown
  * slider
  */

//You can add this to NPc with tag "info_ui"

//Script You must Edit in ""
const Title = "ServerName-Info";

const MainInfo = "Filepath: scripts/mainMenu/modules/info.js";

const infoSerper = "none";

const infoUpdet = "none";

const infoEpent = "none";
```
<br />

### ONLINEPOINT-SETTING
```javascript
// Filepath: scripts/mainMenu/setting/onlinepoint/mainUI
/**
 * id: "name"
 * price: number
 * prizeGet: number/quantityGet
 * type: ["tag","give"]
 * namebutton: "buttonname"
 * texture: "filepath.textures" #optional
 **/
```
<br />

### ScoreboardSetting
```javascript
/**
       * @NAME <PlayerName>
       * @GUILD <Guildname>
       * @MONEY <moneyScore>
       * @[MONEY] <moneyMetric>
       * @RANK <PlayerRank>
       * @ONCOUNT <onlineScore>
       * @KILLCOUNT <killScore>
       * @DEATHCOUNT <deathScore>
       * @DROPCOUNT <itemdropScore>
       * @PING <pingScore>
       * @TPS <tpsScore>
       * @TIME:H <hour>
       * @TIME:M <minutes>
       * @TIME:S <second>
       * @DATE <date>
       * @L <line> (only can use in template
       */
```
### Template Scoreboard
```mcfunction
§k||§r   §l§bServerName§r   §k||§r@L| §bName: §7@NAME@L| §bRank: §r@RANK@L| §bGuild: §6@GUILD§r@L| [Server-Stats]@L| §7ping: §d@PING§r@L| §7online: §a@ONCOUNT§5/§230§r@L| §7itemDrop: @DROPCOUNT@L  ip.server
```
<br />

[Back To UP](#)
