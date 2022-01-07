# Frequently Asked Questions

## Why isn't Nova responding?
1. Make sure you're using the **correct prefix**. Nova's default prefix is a **lowercase L followed by a question mark**. You can ping Nova and it will respond with the server's current prefix.

2. Ensure Nova has the **correct permissions**. Even if you granted Nova all of the requested permissions when you invited it, incorrect **server permissions** can override them. Go to your **per-channel permission settings**, add Nova, and **manually enable** `Send Messages`, `Read Messages`, `View Channel`, and `Embed Links`. 

3. Make sure that nova is currently **online** for responding to commands.


## My partner/affiliate reply won't update!
1. Check your `replymessage` command. It should look like: `[prefix]set replymessage [partnersuccess|affiliatesuccess] <Your text/mentions here> %% <EmbedName>`.

2. Make sure you have the correct `partnerchannel` and `affiliatechannel` set. Use `[prefix]set [partnerchannel|affiliatechannel] list` to show the partner and affiliate channels you currently have added. Use `[prefix]set [partnerchannel|affiliatechannel] remove #channel` to remove channels.

> [!NOTE] 
> The `|` indicates to use one or the other ***(ex: partnerchannel OR affiliatechannel)***

## Slash command doesn't appear?

Re-authenticate (re-invite) the bot with `applications.commands` scope. Use [this link](https://discord.com/api/oauth2/authorize?client_id=711428816127393844&permissions=470150208&scope=bot%20applications.commands) to re-invite the bot **with** slash command support.

## What if I don't want slash commands?

Re-authenticate (re-invite) the bot without `applications.commands` scope. Use [this link](https://discord.com/api/oauth2/authorize?client_id=711428816127393844&permissions=470150208&scope=bot) to re-invite the bot **without** slash command support.

> ***You can join our [support server](https://discord.gg/cAKmRVrsjR) for further support if none of these resolve your issue.***
