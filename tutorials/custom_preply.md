# Customizing your partnership & affiliate responses.
##### This tutorial will show you how to customize each aspect of Nova's partnership and affiliate replies. Add the prefix to the beginning of each command in this tutorial.

1. First, create an embed. You can create one using `createembed EmbedName`. Note that your embed name will be **case-sensitive**.

2. Now that you have your embed created, we can start editing it. We edit it by using `editembed EmbedName [element] [value]`. `Element` is where we will decide what part of the embed to edit, and `value` is what we want to edit it to.

3. Let's run `help editembed`. This will shows us all of the available elements we can edit (as shown **here**):

![ElementsScreenshot](https://cdn.discordapp.com/attachments/589603067146534913/892791544648708147/unknown.png)

4. So let's edit one as an example. Run `editembed EmbedName description Test reply here! Mentioning roles or users does not work inside of embeds`. As you can see, when we run `viewembed EmbedName`, we can see the description we just edited:

![EditDesc](https://cdn.discordapp.com/attachments/711551301334597662/892792864910757928/unknown.png)

5. Let's do one more, to give you an example on how to use what are called **variables**. Variables are exactly what the word describes - they change, depending on, well, variables. For example, let's edit the title of our embed. Let's run `editembed EmbedName title Thank you for partnering, $(user.nick)!`. What this will do, is replace `$(user.nick)` with the name of whoever posted the partnership/affiliate as shown **here**:

![VarExample](https://cdn.discordapp.com/attachments/711551301334597662/892794745582141450/unknown.png)

All variables work the same way - you can view all available variables and see a description of what they do by running `help variables`.

#### You can see which elements show on the embed via a color-coded guide **here**:

![ColorCode](https://cdn.discordapp.com/attachments/731631449194627143/743858854466551959/example_2.png)
