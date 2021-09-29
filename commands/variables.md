# Variables

<!-- TODO: What are variables, how variables works -->

These are available variables that can be used in Embeds, Welcome Messages or Custom Replies. Keep in mind that some variables only works under certain condition (Like partner custom replies).

## User Object

| Variable          | Description                             |
| ----------------- | --------------------------------------- |
| `$(user.name)`    | User's username                         |
| `$(user.nick)`    | User's nickname                         |
| `$(user.tag)`     | User's tag (ex. 0001)                   |
| `$(user.proper)`  | User's username+tag (ex. Username#0001) |
| `$(user.id)`      | User's ID                               |
| `$(user.mention)` | User's mention                          |
| `$(user.avatar)`  | User's avatar link                      |

## Guild Object

| Variable                       | Description                                                       |
| ------------------------------ | ----------------------------------------------------------------- |
| `$(guild.name)`                | Current server's name                                             |
| `$(guild.icon)`                | Current server's icon                                             |
| `$(guild.members)`             | Current server's member count (ex. 123)                           |
| `$(guild.members.ordinal)`     | Current server's member count in ordinal (ex. 123rd)              |
| `$(guild.age)`                 | Current server's age (days)                                       |
| `$(guild.memberreq.partner)`   | Minimum member requirement to partner with this server.           |
| `$(guild.memberreq.affiliate)` | Minimum member requirement to P4P/Affiliate with this server.     |
| `$(guild.agereq.partner)`      | Minimum server age requirement to partner with this server.       |
| `$(guild.agereq.affiliate)`    | Minimum server age requirement to P4P/Affiliate with this server. |

## Partnerships

| Variable                             | Description                                         |
| ------------------------------------ | --------------------------------------------------- |
| `$(user.partner.point)`              | Current user's all time partner point (server-wide) |
| `$(user.partner.rank)`               | Current user's all time rank (server-wide)          |
| `$(user.partner.rank.ordinal)`       | Same as above but in ordinal form (1st, 2nd, ...)   |
| `$(user.partner.weeklypoint)`        | Current user's weekly partner point (server-wide)   |
| `$(user.partner.weeklyrank)`         | Current user's weekly rank (server-wide)            |
| `$(user.partner.weeklyrank.ordinal)` | Same as above but in ordinal form (1st, 2nd, ...)   |
| `$(user.partner.xp)`                 | Current user's XP (global)                          |
| `$(user.partner.level)`              | Current user's level (global)                       |

## Invites

| Variable                       | Description                                              |
| ------------------------------ | -------------------------------------------------------- |
| `$(invite.guild.name)`         | Server's name from posted invite                         |
| `$(invite.guild.id)`           | Server's ID from posted invite                           |
| `$(invite.guild.icon)`         | Server's icon link from posted invite                    |
| `$(invite.guild.age)`          | Server's age (days) from posted invite                   |
| `$(invite.guild.member)`       | Member count of posted invite                            |
| `$(invite.guild.online)`       | Online member count from posted invite                   |
| `$(invite.cooldown.partner)`   | Remaining cooldown time for posting this partner again   |
| `$(invite.cooldown.affiliate)` | Remaining cooldown time for posting this affiliate again |
| `$(invite.blacklist.reason)`   | Reason why server with this invite blacklisted.          |