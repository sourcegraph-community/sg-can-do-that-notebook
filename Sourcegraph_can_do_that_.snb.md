# Sourcegraph can do that?!

All the best things about Sourcegraph that nobody ever bothered to tell you.

Inspired by [VS Code Can Do That?!](https://vscodecandothat.com/)

## 00: Find me pattern matches but only in repositories that have a particular dependency
> via [@beyang](https://twitter.com/beyang/status/1551727744714678272)

```sourcegraph
repo:contains(file:package\.json content:jest) test(:[1]) patterntype:regexp 
```

---

## 01: Filter out any files you don't want in your search query

> via [@jdorfman](https://twitter.com/jdorfman)

```sourcegraph
repo:sindresorhus/awesome -file:(pull_request_template.md|contributing.md) patterntype:regexp Awesome
```

---