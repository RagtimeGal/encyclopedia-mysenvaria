---
title: "Callouts"
enableToc: true
tags:
  - topic/meta/writing_guidelines
type: article
status:
  scope: standard
  progress: complete
  future: []
---

> [!abstract|callout-meta-general] [[Meta/Meta|Meta]] || Fourth Wall Ahead!
> The following article is metatextual. It provides information on what the *Encyclopedia Mysenvaria* is, how it should be used, how you can use it, and how you can help improve it.

Callouts serve to communicate to readers metatextual information about the article they are reading without interfering with the article itself! They're simple but important metatextual communication tools that can simply be appended or prepended to articles without much worry. The injection of callouts is handled by a program which is run on every push to the GitHub repository.

This article lists each of the meta callouts that readers may encounter while browsing.
# Callouts Based On:
## An Article's Contents
### Names
> [!warning] [[Meta/Meta|Meta]] || Placeholders Ahead!
> Some names mentioned in this article are placeholders. Placeholder names may resemble the names of real people, places, or things. They may also be direct descriptions of whatever they are naming. Some may even be random strings of letters or numbers.
> 
> Temporary placeholders are used because conlanging is hard. If you've discovered a name which has the perfect opportunity to be updated please file a [GitHub issue](https://github.com/RagtimeGal/encyclopedia-mysenvaria/issues/new/choose).

Any articles which reference people, places, or things using temporary placeholder names should include this callout.

```JSON
"id": "names"
```
## An Article's Type
### Addendum
```yaml
type: addendum
```

> [!hint] [[Meta/Meta|Meta]] || Addendum Here!
> This article is an addendum, it provides metatextual context to a diegetic article. Visit the parent article here: {original_article}!

```JSON
"id": "addendum"
```

Whilst the above callout is placed at the beginning of addenda the following callout is placed at the end of articles which have addenda.

> [!hint] [[Meta/Meta|Meta]] || Addendum Ahead!
> This article has an addendum which provides metatextual context about this article. Visit the addendum here: {addendum_article}!

```JSON
"id": "has-addendum"
```
### Ledger
```YAML
type: ledger
```

> [!example] [[Meta/Meta|Meta]] || Lore Ledger #{ledger_number}!
> This article serves as a brief changelog and project update announcement for the *Mysenvaria*.
> 
> ... {previous_ledger}, **{current_ledger}**, {next_ledger} ...

```JSON
"id": "ledger"
```
### Template
```yaml
type: template
```

> [!warning] [[Meta/Meta|Meta]] || Template!
> This article is a Template. This callout and others like it in the article should be removed. 
> 
> Remember to modify the article's metadata as necessary! **Remove the template's draft key immediately.** Title, TOC, tags, type, and status should all be updated accordingly!

```JSON
"id": "template"
```
## An Article's Tags
### Meta
```YAML
tags:
  - topic/meta/*
```

> [!abstract] [[Meta/Meta|Meta]] || Fourth Wall Ahead!
> The following article is metatextual. It provides information on what the *Encyclopedia Mysenvaria* is, how it should be used, how you can use it, and how you can help improve it.

```JSON
"id": "meta-general"
```
## An Article's Progress
### Empty
```yaml
status:
  progress: empty
```

> [!note] [[Meta/Meta|Meta]] || Here be Dragons!
> This article provides no information on its given topic, it's an empty page. Think it's in urgent need of expansion? File a [GitHub issue](https://github.com/RagtimeGal/encyclopedia-mysenvaria/issues/new/choose).

```JSON
"id": "empty"
```
### Idea
```yaml
status:
  progress: idea
```

> [!note] [[Meta/Meta|Meta]] || This Article's an Idea!
> This article is in early infancy and the information it provides may not be canonical, accurate, or otherwise coherent. Think it's in urgent need of cohesion? File a [GitHub issue](https://github.com/RagtimeGal/encyclopedia-mysenvaria/issues/new/choose).

```JSON
"id": "idea"
```
### WIP
```yaml
status:
  progress: wip
```

> [!note] [[Meta/Meta|Meta]] || This Article's a Work in Progress!
> This article is currently actively in the process of being written, information it provides may not be canonical, accurate, or otherwise coherent. Think it's in urgent need of completion? File a [GitHub issue](https://github.com/RagtimeGal/encyclopedia-mysenvaria/issues/new/choose).

```JSON
"id": "wip"
```
### Stub
```yaml
status:
  progress: stub
```

> [!note] [[Meta/Meta|Meta]] || This Article's a Stub!
> This article provides a short overview of its topic but it needs to be more comprehensive before being considered complete. Think it's in urgent need of development? File a [GitHub issue](https://github.com/RagtimeGal/encyclopedia-mysenvaria/issues/new/choose).

```JSON
"id": "stub"
```
## An Article's Future
### Pending Future
```yaml
status:
  future: [pending]
```

> [!abstract] [[Meta/Meta|Meta]] || Pending Future Development!
> When the setting has developed further some sections of this article could be elaborated on. If you believe that the article requires urgent expansion please file a [GitHub issue](https://github.com/RagtimeGal/encyclopedia-mysenvaria/issues/new/choose).

```JSON
"id": "pending"
```
### Future Rewrite
```yaml
status:
  future: [rewrite]
```

> [!abstract] [[Meta/Meta|Meta]] || Rewrite Suspected in Future!
> Some sections of this article may need to be rewritten in the future to improve legibility. If you believe that this article requires an urgent rewrite please file a [GitHub issue](https://github.com/RagtimeGal/encyclopedia-mysenvaria/issues/new/choose). 

```JSON
"id": "rewrite"
```
### Future Review
```yaml
status:
  future: [review]
```

> [!abstract] [[Meta/Meta|Meta]] || Possible Revisions Required!
> It's unclear if this article will need to be revisited in the future. If you believe that this article requires an urgent review please file a [GitHub issue](https://github.com/RagtimeGal/encyclopedia-mysenvaria/issues/new/choose).

```JSON
"id": "review"
```
## An Article's Scope
### Generated
```yaml
status:
  scope: generated
```

> [!abstract] [[Meta/Meta|Meta]] || Beep Boop!
> All of, or a portion of, this article is generated by a program. If you believe there's an error in the generation of this article please file a [GitHub issue](https://github.com/RagtimeGal/encyclopedia-mysenvaria/issues/new/choose).

```JSON
"id": "generated"
```