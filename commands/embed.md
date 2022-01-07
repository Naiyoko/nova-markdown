# Embed Module

Module for creating and managing saved embeds.

> [!WARNING]
> All commands in this module require role with `Manage Messages` permission or **Bot Manager** role.

## Creating Embed

Launch an interactive setup for creating new embed.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]embed create [embed_name]
```

#### Aliases

- `embed new`
- `eb create`
- `eb new`

#### [Show slash version](#tab/slash)
```css
/embed create [embed_name]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`embed_name` | yes | Name for embed. Name must only contains alphanumeric, dash or underscore characters. Max length 32 characters.

### Remarks and Limitations

Here are the acceptable values for embed creator input.

Element | Accepted value
---|---
`author` | 256 characters text.
`authoricon` | HTTPS-only image URL. Only displayed if author set.
`title` | 256 characters text.
`description` | 4096 characters text.
`thumbnail` | Image URL.
`color` | Valid [HTML color names](https://www.html-color-names.com/color-chart.php) or color hex.
`image` | Image URL.
`footer` | 2048 characters text.
`footericon` | HTTPS-only image URL. Only displayed if footer set.

All elements except `color` accept [variables](variables.md).

> [!WARNING]
> The whole embed creator setup has 15 minutes timeout counted from the time when command executed. If you need more than 15 minutes to set it up, you can save the embed and edit it later.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]embed create welcome` | Creating new embed with name `welcome`.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/embed create welcome` | Creating new embed with name `welcome`.

- - -

## Editing Embed

Launch an interactive setup for editing an existing embed.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]embed edit [embed_name]
```
#### Aliases

- `eb edit`

#### [Show slash version](#tab/slash)
```css
/embed edit [embed_name]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`embed_name` | yes | Name for saved embed to be edited.


### Remarks and Limitations

Same with [Creating Embed](#remarks-and-limitations) section.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]embed edit welcome` | Edit existing embed with name `welcome`.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/embed edit welcome` | Edit existing embed with name `welcome`.

- - -

## Listing Embed

List saved/existing embeds for current server.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]embed list
```
#### Aliases

- `eb list`

#### [Show slash version](#tab/slash)
```css
/embed list
```
- - -

## Deleting Embed

Delete saved/existing embed for current server.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]embed delete [embed_name]
```
#### Aliases

- `eb delete`

#### [Show slash version](#tab/slash)
```css
/embed delete
```
- - -
Arguments | Required | Description
-----------|----------|------------
`embed_name` | yes | Name for saved embed to be deleted.


### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]embed delete example` | Delete existing embed with name `example`.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/embed delete example` | Delete existing embed with name `example`.

- - -

## Viewing Embed

View/show saved embed by sending it to current channel.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]embed view [embed_name]
```
#### Aliases

- `embed show`
- `eb view`
- `eb show`

#### [Show slash version](#tab/slash)
```css
/embed view [embed_name]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`embed_name` | yes | Name for saved embed to be viewed.


### Remarks and Limitations

If you're executing the command using **slash command**, make sure that the bot **has access** to **send messages** to current channel. It's because slash commands can still be responded by bot even the bot doesn't have permission to send messages or even view the channel.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]embed view welcome` | View existing embed with name `welcome`.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/embed view welcome` | View existing embed with name `welcome`.

- - -

## Importing Embed

Import yaml-template format as new embed. Can support importing from [hastebin](https://haste.luminova.moe) link as well as via attached file.

> [!WARNING]
> Due to slash command limitation, only import via hastebin link is supported via slash command.

> [!IMPORTANT]
> We **don't recommend** to edit the template by hand if you don't have prior experience in yaml file.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]embed import [data]
```
#### Aliases

- `eb import`

Arguments | Required | Description
-----------|----------|------------
`data` | yes | Choose one of: yaml data text, attached text file, hastebin link.

#### [Show slash version](#tab/slash)
```css
/embed import [haste_link]
```

Arguments | Required | Description
-----------|----------|------------
`haste_link` | yes | Hastebin link to yaml template.

- - -


### Remarks and Limitations

Due to current slash command limitation, only hastebin link is supported in slash version. Pasting template data directly or using attached file only supported via traditional-style command.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]embed import https://haste.luminova.moe/template` | Import embed from https://haste.luminova.moe/template link.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/embed import https://haste.luminova.moe/template` | Import embed from https://haste.luminova.moe/template link.

- - -

## Exporting Embed

Export saved embed to yaml-template format.

> [!IMPORTANT]
> We **don't recommend** to edit the template by hand if you don't have prior experience in yaml file.

### Command Overview

#### [Show prefix version](#tab/cnext)
```css
[prefix]embed export [embed_name]
```
#### Aliases

- `eb export`

#### [Show slash version](#tab/slash)
```css
/embed export [embed_name]
```
- - -
Arguments | Required | Description
-----------|----------|------------
`embed_name` | yes | Name for saved embed to be exported.


### Remarks and Limitations

If the size of template exceeds 2048 characters, it will be uploaded to [our hastebin service](https://haste.luminova.moe) instead.

### Examples

#### [Show prefix version](#tab/cnext)
Example Command | Description
-----|-----
`[prefix]embed export welcome` | Export existing embed with name `welcome`.

#### [Show slash version](#tab/slash)
Example Command | Description
-----|-----
`/embed export welcome` | Export existing embed with name `welcome`.

- - -