<div align="center">
  <img src="https://github.com/Kocaki182/ServerUI-N/assets/129764133/6b6b60f5-d2d3-4040-b8fa-067105c0154a" alt="ServerUI"/>
  <h3 align="center"><u>ServerUI-N Docs</u></h3>
</div>

<detail>
<li>
<a href="#guild-ui-testing">Guild-UI</a>
</li>
<li><a href="#betterrtp">RTP (void(0))</a></li>
</detail>

## 🛡Guild-UI [testing]
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
#You can rtp With addTag "rtp_ui"
#You can add command into npc
# CD 10sec

#Copy this command and add to npc
tag @initiator add rtp_npc

#Based
tag @s add rtp_npc
```
<br />

### INFO (guide)
```javascript
/**
 * Check Docs @minecraft/server-ui or @JaylyDev
 */
 
 /**
  * module : "import { ActionFormData } minecraft/server-ui"
  * @ActionFormData
  * @title
  * @body
  * @button
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
  * @title
  * @textField
  * @dropdown
  * @slider
  */

//You can add this to NPc with tag "info_ui"
```
<br />

### Rebuilt
- HomeSystem (Change to Database & support all dimension)
- WarpSystem (Change to Database)
- ChatSystemUI (change to Database)
<br />

### Fixed
- MaskShop
- MessageSystem
<br />

### Disabled Features
- SudoSystem
<br />

### Features
inludes [serverUI v11-link DC](https://discord.com/channels/1003279583476453467/1048900022915313704/1128499602056822827)
- WarpUI
- HomeUI
- ClearLag (command) <on|off|clear>
- BetterRTP (AntiKepentok)
- Invsee (Only support Inventory)
- NickUI
- GuildUI
<br />

### TagList
- WarpTag
```mcfunction
tag (selector/objectname) add warp_ui
```
- Rtp
```mcfunction
tag (selector/objectname) add rtp_ui
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
<br />

[Back To UP](#)
