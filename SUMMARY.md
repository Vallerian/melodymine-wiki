# Table of contents

## Guide

* [🎵 Introduction](README.md)
* [💡 Installation](guide/installation.md)
* [✨ Features](guide/features.md)

## Essentials

* [📜 Commands](essentials/commands.md)
* [📃 Permissions](essentials/permissions.md)
* [📝 Placeholders](essentials/placeholders.md)

## API

* [⚙️ Usage](api/usage.md)
* [🔷 Events](api/events/README.md)
  * [🔹 Call](api/events/call/README.md)
    * [PreStartCallEvent](api/events/call/prestartcallevent.md)
    * [PostStartCallEvent](api/events/call/poststartcallevent.md)
    * [PreAcceptCallEvent](api/events/call/preacceptcallevent.md)
    * [PostAcceptCallEvent](api/events/call/postacceptcallevent.md)
    * [PreDenyCallEvent](api/events/call/predenycallevent.md)
    * [PostDenyCallEvent](api/events/call/postdenycallevent.md)
    * [PreEndCallEvent](api/events/call/preendcallevent.md)
    * [PostEndCallEvent](api/events/call/postendcallevent.md)
    * [PreEndPendingCallEvent](api/events/call/preendpendingcallevent.md)
    * [PostPendingCallEndEvent](api/events/call/postpendingcallendevent.md)
    * [PreToggleCallEvent](api/events/call/pretogglecallevent.md)
    * [PostToggleCallEvent](api/events/call/posttogglecallevent.md)
  * [🔹 Sound](api/events/sound/README.md)
    * [PreChangeSoundVolumeEvent](api/events/sound/prechangesoundvolumeevent.md)
    * [PostChangeSoundVolumeEvent](api/events/sound/postchangesoundvolumeevent.md)
    * [PrePauseSoundEvent](api/events/sound/prepausesoundevent.md)
    * [PostPauseSoundEvent](api/events/sound/postpausesoundevent.md)
    * [PrePlaySoundEvent](api/events/sound/preplaysoundevent.md)
    * [PostPlaySoundEvent](api/events/sound/postplaysoundevent.md)
    * [PreStopSoundEvent](api/events/sound/prestopsoundevent.md)
    * [PostStopSoundEvent](api/events/sound/poststopsoundevent.md)
  * [🔹 Websocket](api/events/websocket/README.md)
    * [PlayerEndVoiceEvent](api/events/websocket/playerendvoiceevent.md)
    * [PlayerJoinWebEvent](api/events/websocket/playerjoinwebevent.md)
    * [PlayerLeaveWebEvent](api/events/websocket/playerleavewebevent.md)
    * [PlayerStartVoiceEvent](api/events/websocket/playerstartvoiceevent.md)
    * [PreEnableVoiceEvent](api/events/websocket/preenablevoiceevent.md)
    * [PostEnableVoiceEvent](api/events/websocket/postenablevoiceevent.md)
    * [PreSetVolumeEvent](api/events/websocket/presetvolumeevent.md)
    * [PostSetVolumeEvent](api/events/websocket/postsetvolumeevent.md)
  * [🔹 Control](api/events/control/README.md)
    * [PlayerChangeControlWebEvent](api/events/control/playerchangecontrolwebevent.md)
    * [PlayerChangeTalkEvent](api/events/control/playerchangetalkevent.md)
    * [PrePlayerMuteEvent](api/events/control/preplayermuteevent.md)
    * [PostPlayerMuteEvent](api/events/control/postplayermuteevent.md)
    * [PreUnMutePlayerEvent](api/events/control/preunmuteplayerevent.md)
    * [PostUnMutePlayerEvent](api/events/control/postunmuteplayerevent.md)
    * [PrePlayerSetSelfMuteEvent](api/events/control/preplayersetselfmuteevent.md)
    * [PostPlayerSetSelfMuteEvent](api/events/control/postplayersetselfmuteevent.md)
    * [PrePlayerSetDeafenEvent](api/events/control/preplayersetdeafenevent.md)
    * [PostPlayerSetDeafenEvent](api/events/control/postplayersetdeafenevent.md)
  * [🔹 Manager](api/events/manager/README.md)
    * [PlayerChangeServerEvent](api/events/manager/playerchangeserverevent.md)
    * [PreEnableAdminModeEvent](api/events/manager/preenableadminmodeevent.md)
    * [PostEnableAdminMode](api/events/manager/postenableadminmode.md)
    * [PreDisableAdminModeEvent](api/events/manager/predisableadminmodeevent.md)
    * [PostDisableAdminMode](api/events/manager/postdisableadminmode.md)
    * [PreRenewDataEvent](api/events/manager/prerenewdataevent.md)
    * [PostRenewDataEvent](api/events/manager/postrenewdataevent.md)
    * [PreSendQRCodeEvent](api/events/manager/presendqrcodeevent.md)
    * [PostSendQRCodeEvent](api/events/manager/postsendqrcodeevent.md)
    * [PreSendSoundSettingsEvent](api/events/manager/presendsoundsettingsevent.md)
    * [PostSendSoundSettingsEvent](api/events/manager/postsendsoundsettingsevent.md)
* [🔶 MelodyManager](api/melodymanager/README.md)
  * [🔸 Call](api/melodymanager/call/README.md)
    * [startCall()](api/melodymanager/call/startcall.md)
    * [endCall()](api/melodymanager/call/endcall.md)
    * [endPendingCall()](api/melodymanager/call/endpendingcall.md)
    * [acceptCall()](api/melodymanager/call/acceptcall.md)
    * [denyCall()](api/melodymanager/call/denycall.md)
    * [toggleCall()](api/melodymanager/call/togglecall.md)
  * [🔸 Sound](api/melodymanager/sound/README.md)
    * [playSound()](api/melodymanager/sound/playsound.md)
    * [pauseSound()](api/melodymanager/sound/pausesound.md)
    * [stopSound()](api/melodymanager/sound/stopsound.md)
    * [changeSoundVolume()](api/melodymanager/sound/changesoundvolume.md)
  * [🔸 Websocket](api/melodymanager/websocket/README.md)
    * [enableVoice()](api/melodymanager/websocket/enablevoice.md)
    * [disableVoice()](api/melodymanager/websocket/disablevoice.md)
    * [setVolume()](api/melodymanager/websocket/setvolume.md)
  * [🔸 Control](api/melodymanager/control/README.md)
    * [setPlayerSelfMute()](api/melodymanager/control/setplayerselfmute.md)
    * [setPlayerDeafen()](api/melodymanager/control/setplayerdeafen.md)
    * [mute()](api/melodymanager/control/mute.md)
    * [unMute()](api/melodymanager/control/unmute.md)
  * [🔸 Manager](api/melodymanager/manager/README.md)
    * [getMelodyPlayer()](api/melodymanager/manager/getmelodyplayer.md)
    * [getMelodyPlayerFromSocketID()](api/melodymanager/manager/getmelodyplayerfromsocketid.md)
    * [sendStartLink()](api/melodymanager/manager/sendstartlink.md)
    * [sendStartQRCode()](api/melodymanager/manager/sendstartqrcode.md)
    * [enableAdminMode()](api/melodymanager/manager/enableadminmode.md)
    * [disableAdminMode()](api/melodymanager/manager/disableadminmode.md)
    * [toggleLogger()](api/melodymanager/manager/togglelogger.md)
    * [showPlayerIsTalking()](api/melodymanager/manager/showplayeristalking.md)
    * [renewData()](api/melodymanager/manager/renewdata.md)
    * [sendSoundSetting()](api/melodymanager/manager/sendsoundsetting.md)
    * [checkPlayerWebConnection()](api/melodymanager/manager/checkplayerwebconnection.md)
* [👨 MelodyPlayer](api/melodyplayer.md)
* [🔊 Sounds](api/sounds.md)

## MISC

* [💫 Troubleshooting](misc/troubleshooting.md)
* [📄 FAQ](misc/faq.md)