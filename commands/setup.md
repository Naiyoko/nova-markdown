# Setup Module

Commands for setting up the bot.

> [!WARNING]
> All commands in this module require role with `Manage Server` permission or **Bot Manager** role.

## Set Bot's Prefix

Set bot's prefix to a new prefix. The change only apply to current server. To reset it to default prefix, run the command without any arguments.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set prefix <new_prefix>
```

Arguments | Required | Description
-----------|----------|------------
`new_prefix` | no | New bot prefix, max 5 chars.

#### [Show slash version](#tab/slash)

This command not applicable on slash command.

- - -

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set prefix >>` | Set bot's prefix to `>>`.
`[prefix]set prefix` | Reset bot's prefix to default prefix.

#### [Show slash version](#tab/slash)

This command not applicable on slash command.

- - -

## Add Partnership Channel

Add a text channel to be tracked for partnership.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set partnerchannel add [channel]
```
#### Aliases

- `set partnerchannel +`

#### [Show slash version](#tab/slash)
```css
/set partnerchannel add [channel]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`channel` | yes | Text channel to be added to partnership tracking list.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set partnerchannel add #partnership` | Add #partnership channel to partnership tracking list.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set partnerchannel add #partnership` | Add #partnership channel to partnership tracking list.

- - -

## Remove Partnership Channel

Remove a text channel from being tracked for partnership.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set partnerchannel remove [channel]
```
#### Aliases

- `set partnerchannel rem`
- `set partnerchannel -`

#### [Show slash version](#tab/slash)
```css
/set partnerchannel remove [channel]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`channel` | yes | Text channel to be removed from partnership tracking list.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set partnerchannel remove #partnership` | Remove #partnership channel to partnership tracking list.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set partnerchannel remove #partnership` | Remove #partnership channel to partnership tracking list.

- - -

## List Partnership Channels

List partnership-tracked channels.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set partnerchannel list
```

#### [Show slash version](#tab/slash)
```css
/set partnerchannel list
```
- - -

## Clean Partnership Channels

Clean partnership-tracked channels from invalid/deleted channels.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set partnerchannel clean
```

#### [Show slash version](#tab/slash)
```css
/set partnerchannel clean
```
- - -

## Add Affiliate Channel

Add a text channel to be tracked for affiliate.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set affiliatechannel add [channel]
```
#### Aliases

- `set affiliatechannel +`

#### [Show slash version](#tab/slash)
```css
/set affiliatechannel add [channel]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`channel` | yes | Text channel to be added to affiliate tracking list.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set affiliatechannel add #affiliate` | Add #affiliate channel to affiliate tracking list.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set affiliatechannel add #affiliate` | Add #affiliate channel to affiliate tracking list.

- - -

## Remove Affiliate Channel

Remove a text channel from being tracked for affiliate.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set affiliatechannel remove [channel]
```
#### Aliases

- `set affiliatechannel rem`
- `set affiliatechannel -`

#### [Show slash version](#tab/slash)
```css
/set affiliatechannel remove [channel]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`channel` | yes | Text channel to be removed from affiliate tracking list.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set affiliatechannel remove #affiliate` | Remove #affiliate channel to affiliate tracking list.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set affiliatechannel remove #affiliate` | Remove #affiliate channel to affiliate tracking list.

- - -

## List Affiliate Channels

List affiliate-tracked channels.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set affiliatechannel list
```

#### [Show slash version](#tab/slash)
```css
/set affiliatechannel list
```
- - -

## Clean Affiliate Channels

Clean affiliate-tracked channels from invalid/deleted channels.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set affiliatechannel clean
```

#### [Show slash version](#tab/slash)
```css
/set affiliatechannel clean
```
- - -

## Inspect Partner Channels

Check/inspect bot permission on current partner channels.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]checkpermission partner
```
#### Aliases

- `checkperm partner`

#### [Show slash version](#tab/slash)
```css
/checkpermission partner
```
- - -

## Inspect Affiliate Channels

Check/inspect bot permission on current affiliate channels.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]checkpermission affiliate
```
#### Aliases

- `checkperm affiliate`

#### [Show slash version](#tab/slash)
```css
/checkpermission affiliate
```
- - -

## Add Ignored Partnership Role

Add a role to ignored partnership role list. 

> [!IMPORTANT]
> Any partnerships from user with any roles from ignored partnership roles **won't be tracked by bot**. So be careful with this setting. 

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set ignoredpartnerrole add [role]
```
#### Aliases

- `set ignoredpartnerrole +`

#### [Show slash version](#tab/slash)
```css
/set ignoredpartnerrole add [role]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`role` | yes | Role to be added to ignored partnership tracking list.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set ignoredpartnerrole add @mods` | Add `mods` role to ignored partnership tracking list.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set ignoredpartnerrole add @mods` | Add `mods` role to ignored partnership tracking list.

- - -

## Remove Ignored Partnership Role

Remove a role from ignored partnership tracking list.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set ignoredpartnerrole remove [role]
```
#### Aliases

- `set ignoredpartnerrole rem`
- `set ignoredpartnerrole -`

#### [Show slash version](#tab/slash)
```css
/set ignoredpartnerrole remove [role]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`role` | yes | Role to be removed from ignored partnership tracking list.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set ignoredpartnerrole remove @mods` | Remove `mods` role from ignored partnership tracking list.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set ignoredpartnerrole remove @mods` | Remove `mods` role from ignored partnership tracking list.

- - -

## List Ignored Partnership Roles

List roles in ignored partnership tracking list.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set ignoredpartnerrole list
```

#### [Show slash version](#tab/slash)
```css
/set ignoredpartnerrole list
```
- - -

## Clean Ignored Partnership Role

Clean ignored partnership tracking list from invalid/deleted roles.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set ignoredpartnerrole clean
```

#### [Show slash version](#tab/slash)
```css
/set ignoredpartnerrole clean
```
- - -

## Add Ignored Affiliate Role

Add a role to ignored affiliate role list. 

> [!IMPORTANT]
> Any affiliate from user with any roles from ignored affiliate roles **won't be tracked by bot**. So be careful with this setting. 

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set ignoredaffiliaterole add [role]
```
#### Aliases

- `set ignoredaffiliaterole +`

#### [Show slash version](#tab/slash)
```css
/set ignoredaffiliaterole add [role]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`role` | yes | Role to be added to ignored affiliate tracking list.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set ignoredaffiliaterole add @mods` | Add `mods` role to ignored affiliate tracking list.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set ignoredaffiliaterole add @mods` | Add `mods` role to ignored affiliate tracking list.

- - -

## Remove Ignored Affiliate Role

Remove a role from ignored affiliate tracking list.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set ignoredaffiliaterole remove [role]
```
#### Aliases

- `set ignoredaffiliaterole rem`
- `set ignoredaffiliaterole -`

#### [Show slash version](#tab/slash)
```css
/set ignoredaffiliaterole remove [role]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`role` | yes | Role to be removed from ignored affiliate tracking list.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set ignoredaffiliaterole remove @mods` | Remove `mods` role from ignored affiliate tracking list.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set ignoredaffiliaterole remove @mods` | Remove `mods` role from ignored affiliate tracking list.

- - -

## List Ignored Affiliate Roles

List roles in ignored affiliate tracking list.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set ignoredaffiliaterole list
```

#### [Show slash version](#tab/slash)
```css
/set ignoredaffiliaterole list
```
- - -

## Clean Ignored Affiliate Role

Clean ignored affiliate tracking list from invalid/deleted roles.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set ignoredaffiliaterole clean
```

#### [Show slash version](#tab/slash)
```css
/set ignoredaffiliaterole clean
```
- - -

## Set Partner Cooldown

Set cooldown for a user posting partnership from same server.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set cooldown partner <duration>
```

#### [Show slash version](#tab/slash)
```css
/set cooldown partner <duration>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`duration` | no | Cooldown duration (in minutes)


### Remarks and Limitations

Cooldown applies per user instead per server. So if different user posted same server link one after another, they will have their own cooldown timer.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set cooldown partner 60` | Set partner cooldown to 60 minutes.
`[prefix]set cooldown partner` | Disable partner cooldown.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set cooldown partner 60` | Set partner cooldown to 60 minutes.
`/set cooldown partner` | Disable partner cooldown.

- - -

## Set Affiliate Cooldown

Set cooldown for a user posting affiliate from same server.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set cooldown affiliate <duration>
```

#### [Show slash version](#tab/slash)
```css
/set cooldown affiliate <duration>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`duration` | no | Cooldown duration (in minutes)


### Remarks and Limitations

Cooldown applies per user instead per server. So if different user posted same server link one after another, they will have their own cooldown timer.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set cooldown affiliate 60` | Set affiliate cooldown to 60 minutes.
`[prefix]set cooldown affiliate` | Disable affiliate cooldown.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set cooldown affiliate 60` | Set affiliate cooldown to 60 minutes.
`/set cooldown affiliate` | Disable affiliate cooldown.

- - -


## Set Partner Minimum Member Requirement

Set minimum server member requirement for accepted partnership.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set memberreq partner <member_count>
```

#### [Show slash version](#tab/slash)
```css
/set memberreq partner <member_count>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`member_count` | no | Minimum server member count.


### Remarks and Limitations

- Server member count here is overall member count including both human and bots.
- Because of availability of this information from discord's end, in very rare cases server member count is not available.
- Due to how we cache invite information, server member count might not represent real time data and not updated immediately.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set memberreq partner 100` | Set minimum member requirement for partnership to 100.
`[prefix]set memberreq partner` | Disable minimum member requirement for partnership.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set memberreq partner 100` | Set minimum member requirement for partnership to 100.
`/set memberreq partner` | Disable minimum member requirement for partnership.

- - -

## Set Affiliate Minimum Member Requirement

Set minimum server member requirement for accepted affiliate.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set memberreq affiliate <member_count>
```

#### [Show slash version](#tab/slash)
```css
/set memberreq affiliate <member_count>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`member_count` | no | Minimum server member count.


### Remarks and Limitations

- Server member count here is overall member count including both human and bots.
- Because of availability of this information from discord's end, in very rare cases server member count is not available.
- Due to how we cache invite information, server member count might not represent real time data and not updated immediately.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set memberreq affiliate 100` | Set minimum member requirement for affiliate to 100.
`[prefix]set memberreq affiliate` | Disable minimum member requirement for affiliate.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set memberreq affiliate 100` | Set minimum member requirement for affiliate to 100.
`/set memberreq affiliate` | Disable minimum member requirement for affiliate.

- - -


## Set Partner Minimum Server Age Requirement

Set minimum server age requirement for accepted partnership.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set agereq partner <server_age>
```

#### [Show slash version](#tab/slash)
```css
/set agereq partner <server_age>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`server_age` | no | Minimum server age in days.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set agereq partner 7` | Set minimum server age requirement for partnership to 7 days.
`[prefix]set agereq partner` | Disable minimum server age requirement for partnership.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set agereq partner 7` | Set minimum server age requirement for partnership to 7 days.
`/set agereq partner` | Disable minimum server age requirement for partnership.

- - -

## Set Affiliate Minimum Server Age Requirement

Set minimum server age requirement for accepted affiliate.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set agereq affiliate <server_age>
```

#### [Show slash version](#tab/slash)
```css
/set agereq affiliate <server_age>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`server_age` | no | Minimum server age in days.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set agereq affiliate 7` | Set minimum server age requirement for affiliate to 7 days.
`[prefix]set agereq affiliate` | Disable minimum server age requirement for affiliate.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set agereq affiliate 7` | Set minimum server age requirement for affiliate to 7 days.
`/set agereq affiliate` | Disable minimum server age requirement for affiliate.

- - -

## Set PM Role

Set a role for Partner Manager. Required for `managers` command as well as strict mode.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set managerrole pm [role]
```

#### [Show slash version](#tab/slash)
```css
/set managerrole pm [role]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`role` | yes | Role for partner manager.


### Remarks and Limitations

- You can't set role above you or the bot as PM role.
- There will be warnings if PM role contains potentially dangerous permissions.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set managerrole pm @PM` | Set `PM` role as partner manager role.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set managerrole pm @PM` | Set `PM` role as partner manager role.

- - -

## Set AM Role

Set a role for Affiliate Manager. Required for `managers` command as well as strict mode.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set managerrole am [role]
```

#### [Show slash version](#tab/slash)
```css
/set managerrole am [role]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`role` | yes | Role for affiliate manager.


### Remarks and Limitations

- You can't set role above you or the bot as AM role.
- There will be warnings if AM role contains potentially dangerous permissions.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set managerrole am @AM` | Set `AM` role as affiliate manager role.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set managerrole am @AM` | Set `AM` role as affiliate manager role.

- - -

## Set Bot Manager Role

> [!WARNING]
> The command requires `Manage Server` permission. This is the only command where **bot manager** role doesn't bypass.

Set a role for Bot Manager. 

> [!IMPORTANT]
> **Bot manager** role will bypass all required permissions for executing administrative commands even though the role doesn't have any required permissions by that command.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set managerrole botmanager <role>
```

#### [Show slash version](#tab/slash)
```css
/set managerrole botmanager <role>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`role` | no | Role for bot manager.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set managerrole botmanager @mods` | Set `mods` role as bot manager role.
`[prefix]set managerrole botmanager` | Remove/reset bot manager role.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set managerrole botmanager @mods` | Set `mods` role as bot manager role.
`/set managerrole botmanager` | Remove/reset bot manager role.

- - -

## Set PM Nick Format

Set nickname format for partner managers. Nick format will be applied on `managers add` command.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set nickformat pm <format>
```

#### [Show slash version](#tab/slash)
```css
/set nickformat pm <format>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`format` | no | Nickname format


### Remarks and Limitations

- You must put `$(user.name)` variable on nick format. `$(user.nick)` won't work.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set nickformat pm [PM] $(user.name)` | Set `[PM] $(user.name)` as nick format for PM.
`[prefix]set nickformat pm` | Reset nick format for PM.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set nickformat pm [PM] $(user.name)` | Set `[PM] $(user.name)` as nick format for PM.
`/set nickformat pm` | Reset nick format for PM.

- - -

## Set AM Nick Format

Set nickname format for affiliate managers. Nick format will be applied on `managers add` command.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set nickformat am <format>
```

#### [Show slash version](#tab/slash)
```css
/set nickformat am <format>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`format` | no | Nickname format


### Remarks and Limitations

- You must put `$(user.name)` variable on nick format. `$(user.nick)` won't work.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set nickformat am [AM] $(user.name)` | Set `[AM] $(user.name)` as nick format for AM.
`[prefix]set nickformat am` | Reset nick format for AM.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set nickformat am [AM] $(user.name)` | Set `[AM] $(user.name)` as nick format for AM.
`/set nickformat am` | Reset nick format for AM.

- - -

## Set PM+AM Nick Format

Set nickname format for people with both partner manager and affiliate manager position. Nick format will be applied on `managers add` command.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set nickformat both <format>
```

#### [Show slash version](#tab/slash)
```css
/set nickformat both <format>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`format` | no | Nickname format


### Remarks and Limitations

- You must put `$(user.name)` variable on nick format. `$(user.nick)` won't work.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set nickformat both [PM|AM] $(user.name)` | Set `[PM|AM] $(user.name)` as nick format for PM+AM.
`[prefix]set nickformat both` | Reset nick format for PM+AM.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set nickformat both [PM|AM] $(user.name)` | Set `[PM|AM] $(user.name)` as nick format for PM+AM.
`/set nickformat both` | Reset nick format for PM+AM.

- - -


## Set Weekly Auto-reset 

Set automatic weekly leaderboard reset. Default is off.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set autoweekly [value]
```

#### [Show slash version](#tab/slash)
```css
/set misc autoweekly [value]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`value` | yes | On/off (prefix) or true/false (slash)

### Remarks and Limitations

- Changing this settings will also clear weekly leaderboard.
- Next weekly reset will be based on when this setting enabled.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set autoweekly on` | Turn on weekly leaderboard auto-reset.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set misc autoweekly True` | Turn on weekly leaderboard auto-reset.

- - -

## Set PM/AM Strict Mode

Set if bot only track partnership/affiliate from people with PM/AM role only. Default is off.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set strictmode [value]
```

#### [Show slash version](#tab/slash)
```css
/set misc strictmode [value]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`value` | yes | On/off (prefix) or true/false (slash)

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set strictmode on` | Turn on PM/AM strict mode.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set misc strictmode True` | Turn on PM/AM strict mode.

- - -

## Set PM Channel

Set channel for PM welcome message.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set pmchannel <channel>
```

#### [Show slash version](#tab/slash)
```css
/set misc pmchannel <channel>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`channel` | yes | Target text channel.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set pmchannel #pm-chat` | Set PM channel to #pm-chat.
`[prefix]set pmchannel` | Clear PM channel setting.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set misc pmchannel #pm-chat` | Set PM channel to #pm-chat.
`/set misc pmchannel` | Clear PM channel setting.

- - -

## Set Member Welcome Channel

Set channel for member welcome message.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set welcomechannel <channel>
```

#### [Show slash version](#tab/slash)
```css
/set misc welcomechannel <channel>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`channel` | yes | Target text channel.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set welcomechannel #welcome` | Set member welcome channel to #welcome.
`[prefix]set welcomechannel` | Clear member welcome channel setting.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set misc welcomechannel #welcome` | Set member welcome channel to #welcome.
`/set misc welcomechannel` | Clear member welcome channel setting.

- - -

## Set Member Leave Channel

Set channel for member leave message.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set leavechannel <channel>
```

#### [Show slash version](#tab/slash)
```css
/set misc leavechannel <channel>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`channel` | yes | Target text channel.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set leavechannel #goodbye` | Set member leave channel to #goodbye.
`[prefix]set leavechannel` | Clear member leave channel setting.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set misc leavechannel #goodbye` | Set member leave channel to #goodbye.
`/set misc leavechannel` | Clear member leave channel setting.

- - -

## Set Reply Message

Set up custom replies for partnership response as well as PM welcome message, member welcome and leave message.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set replymessage [options] <content> %% <embed_name>
```
#### Aliases

- `set customreply`

#### [Show slash version](#tab/slash)
```css
/replymessage [options] <content> <embed_name>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`options` | yes | One of [reply types](reply_options.md#reply-types) options.
`content` | no | Unembedded part of message.
`embed_name` | no | Name of embed for message.


### Remarks and Limitations

- Refer to [this page](reply_options.md#reply-types) for the list of available options.
- `content` part accepts [variables](variables.md).
- Due to current slash command limitation, `content` part doesn't support multiline. Use prefix command if you need multiline on `content` part.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set replymessage partnersuccess Thank you $(user.mention) for partnering with $(invite.guild.name)` | Set partner success message without embed.
`[prefix]set replymessage partnersuccess $(user.mention) %% partner_success` | Set partner success message with unembedded content and embed named `partner_success`.
`[prefix]set replymessage partnersuccess %% partner_success` | Set partner success message with embed named `partner_success`.
`[prefix]set replymessage partnersuccess` | Resets partner success message to default.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
/replymessage options:`PartnerSuccess` content:`Thank you $(user.mention) for partnering with $(invite.guild.name)` | Set partner success message without embed.
/replymessage options:`PartnerSuccess` content:`$(user.mention)` embed_name:`partner_success` | Set partner success message with unembedded content and embed named `partner_success`.
/replymessage options:`PartnerSuccess` embed_name:`partner_success` | Set partner success message with embed named `partner_success`.
/replymessage options:`PartnerSuccess` | Resets partner success message to default.

- - -

## Set Deletion Behavior

Set deletion behavior on invalid partnership/affiliate.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]set overridebehavior [parameter] [value]
```
Arguments | Required | Description
-----------|----------|------------
`parameter` | yes | [Parameter](reply_options.md#behavior-override-types) to be changed.
`value` | yes | New value (`keep`, `allow`, `delete`, `deny`).

#### [Show slash version](#tab/slash)
```css
/set misc overridebehavior [parameter] [keep_message]
```
Arguments | Required | Description
-----------|----------|------------
`parameter` | yes | [Parameter](reply_options.md#behavior-override-types) to be changed.
`keep_message` | yes | `True` to keep message, `False` to delete message.

- - -

### Remarks and Limitations

Refer to [this page](reply_options.md#behavior-override-types) for list of available parameters and its default value.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]set overridebehavior partnerinvalid allow` | Set the bot to allow (not delete) partner with invalid link.
`[prefix]set overridebehavior affiliatememreq delete` | Set the bot to delete affiliate that doesn't meet member req.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/set misc overridebehavior PartnerInvalid True` | Set the bot to allow (not delete) partner with invalid link.
`/set misc overridebehavior AffiliateMemReq False` | Set the bot to delete affiliate that doesn't meet member req.

- - -

## Test Replies

Test how replies/custom replies look like. You can optionally add server invite to see how the reply looks like with server invite.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]testreply [options] <invite>
```

#### [Show slash version](#tab/slash)
```css
/testreply [options] <invite>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`options` | yes | One of [reply types](reply_options.md#reply-types) options.
`invite` | no | Optional invite link/code for testing invite-related variables.

### Remarks and Limitations

- Replies will be sent to current channel for partner/affiliate replies.
- Replies will be sent to welcome/leave channel for welcome/leave message.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]testreply partnersuccess discord.gg/example` | Test how `partnersuccess` reply looks like with an invite context.
`[prefix]testreply welcome` | Test how welcome message looks like on welcome channel.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/testreply PartnerSuccess discord.gg/example` | Test how `partnersuccess` reply looks like with an invite context.
`/testreply Welcome` | Test how welcome message looks like on welcome channel.

- - -
