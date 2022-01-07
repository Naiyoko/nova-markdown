# Utilities Module

Collections of utilities commands.

## Get Bot's Latency (Ping)

Get current latency (ping) of the bot.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]ping
```

#### [Show slash version](#tab/slash)
```css
/ping
```
- - -

## Get user's avatar

Get user's global avatar and server's avatar if they have server avatar set.

> [!NOTE]
> This functionality has [**context menu support**](context_menu.md).

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]avatar <user>
```
#### Aliases

- `av`

#### [Show slash version](#tab/slash)
```css
/avatar <user>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`user` | no | Target user, set to current user who executed the command if not set.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]avatar` | Display your avatar.
`[prefix]avatar @member` | Display `member`'s avatar.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/avatar` | Display your avatar.
`/avatar @member` | Display `member`'s avatar.

- - -

## Get user's info

Get user's information like ID, creation date, etc.

> [!NOTE]
> This functionality has [**context menu support**](context_menu.md).

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]userinfo <user>
```
#### Aliases

- `whois`

#### [Show slash version](#tab/slash)
```css
/whois <user>
```
- - -
Arguments | Required | Description
-----------|----------|------------
`user` | no | Target user, set to current user who executed the command if not set.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]userinfo` | Display your user info.
`[prefix]userinfo @member` | Display `member`'s user info.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/whois` | Display your user info.
`/whois @member` | Display `member`'s user info.

- - -

## Get role's info

Get information about a role like ID, color, etc.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]roleinfo [role]
```

#### [Show slash version](#tab/slash)
```css
/roleinfo [role]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`role` | yes | Role to be checked

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]roleinfo @verified` | Displays information of `verified` role.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/roleinfo @verified` | Displays information of `verified` role.

- - -

## Get channel's info

Get information about a channel like ID, type, etc. Can be used to check voice channels, category channels as well as other type of channels.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]channelinfo [channel]
```

#### [Show slash version](#tab/slash)
```css
/channelinfo [channel]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`channel` | yes | Channel to be checked

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]channelinfo #verify` | Displays information of `verify` channel.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/channelinfo #verify` | Displays information of `verify` channel.

- - -

## Get server's info

Get information about current server.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]serverinfo
```

#### [Show slash version](#tab/slash)
```css
/serverinfo
```
- - -


## Get snowflake info

Get timestamp information from snowflake (Discord ID).

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]snowflakeinfo [snowflake]
```

#### [Show slash version](#tab/slash)
```css
/snowflakeinfo [snowflake]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`snowflake` | yes | Snowflake (Discord ID) to be checked

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]snowflakeinfo 711428816127393844` | Displays timestamp information of `711428816127393844`.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/snowflakeinfo 711428816127393844` | Displays timestamp information of `711428816127393844`.

- - -

## Get invite's info

Get information about a server invite.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]inviteinfo [invite]
```
#### Aliases

- `checkinvite`
- `ci`

#### [Show slash version](#tab/slash)
```css
/inviteinfo [invite]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`invite` | yes | Discord invite link or code.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]inviteinfo test` | Displays invite information from invite code `test`.
`[prefix]inviteinfo discord.gg/example` | Displays invite information from invite link `discord.gg/example`.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/inviteinfo test` | Displays invite information from invite code `test`.
`/inviteinfo discord.gg/example` | Displays invite information from invite link `discord.gg/example`.

- - -

