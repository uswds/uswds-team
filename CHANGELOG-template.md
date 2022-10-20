# Changelog
These releases may contain markup changes and potentially breaking changes.
A warning icon (:warning:) indicates where we've made an update that might be a breaking change for your project.

## [Version #]
<!--
Every release should have an entry.
Releases should be listed in reverse chronological order, with the newest release listed first.
-->

[Release date]
<!--
Include the date the version was released.
The date should be in the following format: January 1, 2000. -->

### [Category name]
<!-- Categorize items into the following section headings.
Include only the sections that apply to this release.
Sections should be presented in alphabetical order by section heading.
If it isn't clear how to categorize an item, put it inside the `General` section.
### General
### Accessibility
### Performance
### Visual
-->

[Itemized list of all user-affected changes.]

[Example item format:

- [Brief statement that summarizes the change] (#[Related PR])
  - [Optional 1-2 sentence description included in a nested list item.]
  - ⚠️ **User action required:** <!-- Include this section and header if this change requires user action -->
      - [Optional summary of breaking changes with explanation of what action the user must take.]
      - [If there are code changes that the user must update, include demonstrations of the differences with diff code snippets, shown in the example below.]

```diff
- This line was removed.
+ This line is added.
This line has stayed the same.
```
]
<!--
Whenever possible, change items should:
- Include a brief description of the update that focuses on user benefit
- Use a consistent set of verbs to begin each statement
  Examples: "Fixed", "Added", "Improved", "Optimized", "Updated" at the start of the summary helps indicate change type
- Use plain language and be human-readable
- Make content scannable by keeping lines short
- Include a link to the related PR
- Be categorized under the appropriate section headings
- Include instructions for required user action
-->

### Dependency updates

| Name              | Old                                     | New                      |
| :---------------- | --------------------------------------- | ------------------------ |
| [Dependency name] | [Previous version number or `-` if new] | [Current version number] |
| [Removed dependency name] | [Previous version number] | REMOVED |
<!--
Share any dependency updates using the provided table structure.
If no updates, write `_No dependency updates_`
-->

[ ] critical, [ ] high, [ ] moderate vulnerabilities in dependencies
<!--
If no vulnerabilities, write `0 vulnerabilities in dependencies`
-->

[ ] critical, [ ] high, [ ] moderate vulnerabilities in devDependencies
<!--
If no vulnerabilities, write `0 vulnerabilities in devDependencies`
-->

Release TGZ SHA-256 hash:[ ]
