# Setting up partnership requirements
#### This tutorial will guide you through configuring Nova's highly customizable partnership requirement features - involving a minimum server member requirement, a minimum server age, etc. These are divided into separate sections on this page.
* [Set up a minimum server age requirement]()
* [Set a cooldown before a user can partner with the same server twice]()
* [Configuring what Nova does when certain requirements are not met]()


## Setting up a minimum server member requirement
#### This section will tell you how to have Nova check if a server has enough members to meet your requirements before considering it a valid partnership or affiliate.
> [!NOTE] When Nova counts how many members a server has, bots won't be counted.

> [!WARNING] The `/` indicates instructions to use **one or the other** in your command, **not both**.
1. The help page for this command can be viewed using `[prefix]help setmemberreq`. You can set separate member requirements for both partnerships and affiliates. By default, Nova does not have any member count requirements active.

2. So for example, let's set a member requirement of 60. We can do that using `[prefix]setmemberreq partner`/`affiliate 60`.

3. Now, if a partnership or affiliate is posted with a server below 60 members, by default, Nova will ping them with a message telling them that the server doesn't meet your member requirements. This will also not award them a point for that partnership.