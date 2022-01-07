# Changelog

## Version 2.0.0 - Rewrite edition (Date: 8 November 2021)

Basically rewrite almost everything in the bot to new library ([DSharpPlus](https://github.com/DSharpPlus/DSharpPlus)) for a better future as it supports a lot of new discord's features.

### New Features

Only major new features listed.

- Slash Commands support. See [here](commands/index.md) for more details.
- Context Menu support. See [here](commands/context_menu.md) for more details.
- Brand new embed creator.
- `set strictmode` - Set the bot to only track partnership/affiliate to people with PM/AM role.

### Removed Features

- Old version of embed creator `buildembed`. Deprecated in favor of new embed creator.
- Old version of edit embed. Deprecated in favor of new embed creator.

### Changed Features

- Changed paginator to use button instead reaction.
- Changed confirmation message to use button instead prompting "yes/no".
- Moved non-command help topics under new command `topic`.
- Moved detailed examples from help commands to docs page as it's more difficult to maintain for changes.
- Changed some commands in favor of organization. Refer table below for reference.

| Old Command            | New Command                  |
| ---------------------- | ---------------------------- |
| `setprefix`            | `set prefix`                 |
| `partnerchannel`       | `set partnerchannel`         |
| `affiliatechannel`     | `set affiliatechannel`       |
| `ignoredpartnerrole`   | `set ignoredpartnerrole`     |
| `ignoredaffiliaterole` | `set ignoredaffiliaterole`   |
| `setcooldown`          | `set cooldown`               |
| `setagereq`            | `set agereq`                 |
| `setmemberreq`         | `set memberreq`              |
| `setrole`              | `set managerrole`            |
| `setbotmanager`        | `set managerrole botmanager` |
| `setnickformat`        | `set nickformat`             |
| `setautoweekly`        | `set autoweekly`             |
| `setcustomreply`       | `set replymessage`           |
| `overridebehavior`     | `set overridebehavior`       |
| `setpmchannel`         | `set pmchannel`              |
| `setpmwelcomemessage`  | `set replymessage pmwelcome` |
| `setwelcomechannel`    | `set welcomechannel`         |
| `setwelcomemessage`    | `set replymessage welcome`   |
| `setleavechannel`      | `set leavechannel`           |
| `setleavemessage`      | `set replymessage leave`     |
| `addmanager`           | `managers add`               |
| `removemanager`        | `managers remove`            |
| `listmanager`          | `managers list`              |
| `createembed`          | `embed create`*              |
| `editembed`            | `embed edit`*                |
| `deleteembed`          | `embed delete`               |
| `listembed`            | `embed list`                 |
| `viewembed`            | `embed view`                 |
| `importembed`          | `embed import`               |
| `exportembed`          | `embed export`               |

> [!NOTE]
> Commands marked by `*` will have different behavior compared to old version since it will utilize the new embed creator