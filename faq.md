# Frequently Asked Questions
#### Why isn't Nova responding?
1. Make sure you're using the **correct prefix**. Nova's default prefix is a **lowercase L followed by a question mark**. You can ping Nova and it will respond with the server's current prefix.

2. Ensure Nova has the **correct permissions**. Even if you granted Nova all of the requested permissions when you invited it, incorrect **server permissions** can override them. Go to your **per-channel permission settings**, add Nova, and **manually enable** `Send Messages`, `Read Messages`, `View Channel`, and `Embed Links`. 
#
#### My partner/affiliate reply won't update!
1. Check your `setcustomreply` command. It should look like: `[prefix]setcustomreply parntersuccess`/`affiliatesuccess Your text/mentions here %% EmbedName`.

2. Make sure you have the correct `partnerchannel` and `affiliatechannel` set. Use `[prefix]partnerchannel`/`affiliatechannel list` to show the partner and affiliate channels you currently have added. Use `[prefix]partnerchannel`/`affiliatechannel remove #chan` to remove channels.

> [!NOTE] The `/` indicates to use one or the other ***(ex: partnerchannel OR affiliatechannel)***

## 
***You can join our [support server](https://discord.gg/cAKmRVrsjR) for further support if none of these resolve your issue.***
