[![Terminology Folder](/screens/terminologyfolder.png)](https://apps.apple.com/us/app/terminology-dictionary/id687798859)

# Custom Terminology Actions
Updated `04212023-013356`

- [WTF](https://davidblue.wtf/drafts/52E57AEC-3902-4A6E-AB93-180A2C67D41F.html)
- [Local](shareddocuments:///private/var/mobile/Library/Mobile%20Documents/com~apple~CloudDocs/Written/52E57AEC-3902-4A6E-AB93-180A2C67D41F.md)
- [Terminology Dictionary App Store Review](drafts://open?uuid=0624BF75-F9EB-417D-AB63-6C2F0D245B82)
- [Draft](drafts://open?uuid=52E57AEC-3902-4A6E-AB93-180A2C67D41F)

---

[![Drafts Definition Action](https://user-images.githubusercontent.com/43663476/233560921-83692f85-bc29-44d5-8c2f-6b7a990dd90f.jpeg)](https://github.com/extratone/terminology/issues/3)

## [Drafts Definition](terminology://x-callback-url/importAction?name=Drafts-definition&shortName=Drafts&description=Send%20term%20and%20full%20Markdown%20definitions%20to%20Drafts.&urlTemplate=drafts://create?text%3D%5B%5Bdefinitions%5D%5D%250A%5B%5Bnote%5D%5D%26tag%3Dvocabulary&dispatchType=0) [#3](https://github.com/extratone/terminology/issues/3)

- **Name** - `Drafts Definition`
- Shortname - `Drafts`

### Template

```
drafts://create?text=[[definitions]]%0A[[note]]&tag=vocabulary
```

```
terminology://x-callback-url/importAction?name=Drafts-definition&shortName=Drafts&description=Send%20term%20and%20full%20Markdown%20definitions%20to%20Drafts.&urlTemplate=drafts://create?text%3D%5B%5Bdefinitions%5D%5D%250A%5B%5Bnote%5D%5D%26tag%3Dvocabulary&dispatchType=0
```

---

[![Bear Vocabulary Action](https://user-images.githubusercontent.com/43663476/233561642-d2c4abbd-c22b-47a8-9bcc-28fc8691d396.jpeg)](https://github.com/extratone/terminology/issues/4)

## [Bear Vocabulary](terminology://x-callback-url/importAction?name=Bear%20Vocabulary&shortName=Bear&description=Send%20term%20and%20full%20Markdown%20definitions%20to%20Bear.&urlTemplate=bear://x-callback-url/create?title%3D%5B%5Bterm%5D%5D%26tags%3Dvocabulary%26open_note%3Dyes%26text%3D-%2520%5BTerminology%5D(%5B%5Bterm_url%5D%5D)%250A%250A---%250A%250A%5B%5Bdefinitions%5D%5D%250A%250A%5B%5Bnote%5D%5D&dispatchType=0) [#4](https://github.com/extratone/terminology/issues/4)

- **Name** - `Bear Vocabulary`
- Shortname - `Bear`

### Template

```
bear://x-callback-url/create?title=[[term]]&tags=vocabulary&open_note=yes&text=-%20[Terminology]([[term_url]])%0A%0A---%0A%0A[[definitions]]%0A%0A[[note]]
```

```
terminology://x-callback-url/importAction?name=Bear%20Vocabulary&shortName=Bear&description=Send%20term%20and%20full%20Markdown%20definitions%20to%20Bear.&urlTemplate=bear://x-callback-url/create?title%3D%5B%5Bterm%5D%5D%26tags%3Dvocabulary%26open_note%3Dyes%26text%3D-%2520%5BTerminology%5D(%5B%5Bterm_url%5D%5D)%250A%250A---%250A%250A%5B%5Bdefinitions%5D%5D%250A%250A%5B%5Bnote%5D%5D&dispatchType=0
```

---

[![DayOne Vocabulary Entry Action Result](/terminology/screens/dayone)](https://github.com/extratone/terminology/issues/7)

## [DayOne Vocabulary Entry](terminology://x-callback-url/importAction?name=Day%20One%20Vocabulary%20Entry&shortName=DayOne&description=&urlTemplate=dayone://post?entry%3D%5B%5Bdefinitions%5D%5D%250A%5B%5Bnote%5D%5D%26journal%3DDavod%26tags%3Dvocabulary&dispatchType=0)

- **Name** - `DayOne Vocabulary Entry`
- Shortname - `DayOne`

### Template

```
dayone://post?entry=[[definitions]]%0A[[note]]&journal=Davod&tags=vocabulary
```

```
terminology://x-callback-url/importAction?name=Day%20One%20Vocabulary%20Entry&shortName=DayOne&description=&urlTemplate=dayone://post?entry%3D%5B%5Bdefinitions%5D%5D%250A%5B%5Bnote%5D%5D%26journal%3DDavod%26tags%3Dvocabulary&dispatchType=0
```

---

## Action Tag Reference

*Sourced from [**Agiletortoise's Zendesk**](https://agiletortoise.zendesk.com/hc/en-us/articles/200689454-Terminology-Tag-Reference)*

- `[[term]]` : The current term being browsed in the app.
- `[[term_url]]` : A URL that can be used to open Terminology directly to the current term on any device with Terminology installed.
- `[[termly_url]]` : ~~The URL for the term at [Term.ly](http://term.ly/), Terminology’s online companion. This link is useful to share definitions with people who do not have Terminology or an iOS device, for that matter.~~
- `[[definition]]` : The full text of the definitions and related words currently being browsed, in [Markdown](http://daringfireball.net/projects/markdown/) format.
- `[[note]]` : The text of a user note attached to the current term.
- `[[clipboard]]` : Current contents of the iOS clipboard.