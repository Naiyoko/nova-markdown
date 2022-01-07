# Partnership Module

Commands for managing partnership/affiliate.

## Check Partnership Stat

Show partnership stat of a user or current user.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]partnerstat <user>
```
#### Aliases

- `profile`
- `pstat`
- `ps`

#### [Show slash version](#tab/slash)
```css
/partnerstat <user>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`user` | no | Target user, sets to current user if not set.


## Check Server's Partnership Overview

Check current server's partnership overview and settings.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]serverprofile
```
#### Aliases

- `partnerinfo`
- `pinfo`

#### [Show slash version](#tab/slash)
```css
/serverprofile 
```
- - -

## Check Partnership Leaderboard

Check current server's partnership leaderboard.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]partnerleaderboard <alltime|weekly>
```
#### Aliases

- `pboard`
- `plb`

#### [Show slash version](#tab/slash)
```css
/partner leaderboard [alltime|weekly]
```
- - -

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]partnerleaderboard` | Show current server's all time leaderboard.
`[prefix]partnerleaderboard weekly` | Show current server's weekly leaderboard.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/partner leaderboard alltime` | Show current server's all time leaderboard.
`/partner leaderboard weekly` | Show current server's weekly leaderboard.

- - -

## Clear Partnership Leaderboard

> [!WARNING]
> This command requires role with `Manage Server` permission or **Bot Manager** role.

Clear partnership leaderboard entirely or just from left users.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]partnerclear <alltime|weekly|leftusers>
```
#### Aliases

- `pclear`

#### [Show slash version](#tab/slash)
```css
/partner clearlb <alltime|weekly|leftusers>
```
- - -

### Remarks and Limitations

Clearing all time leaderboard will also clear weekly one.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]partnerclear` | Clear all time leaderboard.
`[prefix]partnerclear weekly` | Clear weekly leaderboard.
`[prefix]partnerclear leftusers` | Clear leaderboard from left users. 

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/partner clearlb alltime` | Clear all time leaderboard.
`/partner clearlb weekly` | Clear weekly leaderboard.
`/partner clearlb leftusers` | Clear leaderboard from left users. 

- - -

## Clear User's Point

> [!WARNING]
> This command requires role with `Manage Server` permission or **Bot Manager** role.

Clear user's partner point.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]partnerclearuser [alltime|weekly] [user]
```
#### Aliases

- `pclearuser`

#### [Show slash version](#tab/slash)
```css
/partner clearuser [alltime|weekly] [user]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`user` | yes | Target user.


### Remarks and Limitations

Clearing all time point will also clear weekly one.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]partnerclearuser alltime @User` | Clear `User`'s all time point.
`[prefix]partnerclearuser weekly @User` | Clear `User`'s weekly point.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/partner clearuser alltime @User` | Clear `User`'s all time point.
`/partner clearuser weekly @User` | Clear `User`'s weekly point.

- - -

## Modify User's Point

> [!WARNING]
> This command requires role with `Manage Server` permission or **Bot Manager** role.

Manually adding/removing user's partner point.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]modifypoint [add|remove|rem|+|-] <amount> [user]
```
#### Aliases

- `mpoint`
- `mp`

#### [Show slash version](#tab/slash)
```css
/partner modifypoint [add|remove] [amount] [user]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`amount` | no | Amount to be added/removed.
`user` | yes | Target user.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]modifypoint add 10 @User` | Add `User`'s point by 10.
`[prefix]modifypoint - @User` | Remove `User`'s point by 1.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/partner modifypoint add 10 @User` | Add `User`'s point by 10.
`/partner modifypoint remove 1 @User` | Remove `User`'s point by 1.

- - -

## Add Server(s) to Blacklist

> [!WARNING]
> This command requires role with `Manage Server` permission or **Bot Manager** role.

Add server id to partnership/affiliate blacklist optionally with reason.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]partnerblacklist add [server_ids] <reason>
```
#### Aliases

- `pblacklist add`
- `pblacklist +`
- `pbl add`
- `pbl +`

Arguments | Required | Description
-----------|----------|------------
`server_ids` | yes | List of server ids to be blacklisted, separated with comma, don't put space in between.
`reason` | no | Reason for blacklist.

#### [Show slash version](#tab/slash)
```css
/blacklist add [server_ids] <reason>
```
Arguments | Required | Description
-----------|----------|------------
`server_ids` | yes | List of server ids to be blacklisted, separated with comma.
`reason` | no | Reason for blacklist.

- - -

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]partnerblacklist add 123456789012345678 Scammer server` | Add server `1234567890123456` to blacklist with reason.
`[prefix]partnerblacklist add 123456789012345678,987654321098765432` | Add server `123456789012345678` and `987654321098765432` to blacklist.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
/blacklist add server_ids:`123456789012345678` reason:`Scammer server` | Add server `1234567890123456` to blacklist with reason.
/blacklist add server_ids:`123456789012345678,987654321098765432` | Add server `123456789012345678` and `987654321098765432` to blacklist.

- - -

## Remove Server(s) From Blacklist

> [!WARNING]
> This command requires role with `Manage Server` permission or **Bot Manager** role.

Remove server id from partnership/affiliate blacklist.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]partnerblacklist remove [server_ids]
```
#### Aliases

- `pblacklist remove`
- `pblacklist -`
- `pbl remove`
- `pbl -`

Arguments | Required | Description
-----------|----------|------------
`server_ids` | yes | List of server ids to be unblacklisted, separated with comma, don't put space in between.

#### [Show slash version](#tab/slash)
```css
/blacklist remove [server_ids] 
```
Arguments | Required | Description
-----------|----------|------------
`server_ids` | yes | List of server ids to be unblacklisted, separated with comma.

- - -

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]partnerblacklist remove 123456789012345678` | Remove server `1234567890123456` from blacklist.
`[prefix]partnerblacklist remove 123456789012345678,987654321098765432` | Remove server `123456789012345678` and `987654321098765432` from blacklist.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
/blacklist remove server_ids:`123456789012345678` | Remove server `1234567890123456` to blacklist.
/blacklist remove server_ids:`123456789012345678,987654321098765432` | Remove server `123456789012345678` and `987654321098765432` to blacklist.

- - -

## Set Blacklist Reason

> [!WARNING]
> This command requires role with `Manage Server` permission or **Bot Manager** role.

Set reason for already-blacklisted server.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]partnerblacklist reason [server_id] [reason]
```
#### Aliases

- `pblacklist reason`
- `pbl reason`

#### [Show slash version](#tab/slash)
```css
/blacklist reason [server_id] [reason]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`server_id` | yes | Blacklisted server id to be changed.
`reason` | yes | Reason for blacklist.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]partnerblacklist reason 987654321098765432 Scammer server` | Set reason for blacklisting server `987654321098765432`.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
/blacklist reason server_id:`987654321098765432` reason:`Scammer server` | Set reason for blacklisting server `987654321098765432`.

- - -

## List Blacklist

List current server's blacklisted servers.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]partnerblacklist list
```
#### Aliases

- `pblacklist list`
- `pbl list`

#### [Show slash version](#tab/slash)
```css
/blacklist list
```
- - -

## Add Managers

> [!WARNING]
> This command requires role with `Manage Roles` permission or **Bot Manager** role.

> [!NOTE]
> This functionality has [**context menu support**](context_menu.md).

Add managers role to user, nickname them and send welcome message for them. In this context, both means a position with both PM and AM position.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]managers add [pm|am|both] [user]
```
#### Aliases

- `managers +`
- `mgr add`
- `mgr +`

#### [Show slash version](#tab/slash)
```css
/managers add [pm|am|both] [user]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`user` | yes | Target user.


### Remarks and Limitations

- Nickname only applied if `set nickformat` set.
- PM welcome message will be sent only if both `replymessage pmwelcome` and `set pmchannel` set.
- Discord role hierarchy rules and limitations applies.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]managers add pm @User` | Give `User` PM position.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/managers add pm @User` | Give `User` PM position.

- - -

## Remove Managers

> [!WARNING]
> This command requires role with `Manage Roles` permission or **Bot Manager** role.

Remove managers role from user and reset their nickname if applicable. In this context, both means a position with both PM and AM position.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]managers remove [pm|am|both] [user]
```
#### Aliases

- `managers -`
- `mgr remove`
- `mgr -`

#### [Show slash version](#tab/slash)
```css
/managers remove [pm|am|both] [user]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`user` | yes | Target user.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]managers remove pm @User` | Remove PM position from `User`.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/managers remove pm @User` | Remove PM position from `User`.

- - -

## List Managers

List people with managers role.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]managers list [pm|am|both]
```
#### Aliases

- `mgr list`

#### [Show slash version](#tab/slash)
```css
/managers list [pm|am|both]
```
- - -
