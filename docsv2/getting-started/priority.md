---
publish: true
---

# Priority

## Priorities and Order

Tasks can have a priority.
In order to specify the priority of a task, you can append one of the "priority signifiers", shown here in decreasing order of priority:

1. ⏫ for high priority
2. 🔼 for medium priority
3. use no signifier to indicate no priority
4. 🔽 for low priority

If a task has no priority at all, it is considered between low and medium priority.
This means that the priority of 🔽 low tasks is considered lower than the priority of tasks without any specific priority.
The idea is that you can easily filter out unimportant tasks without needing to assign a priority to all relevant tasks.

```markdown
- [ ] take out the trash 🔼
```

## Easy adding of Priorities

Instead of adding the emoji manually, you can:

- Use the `Tasks: Create or edit` command when creating or editing a task.
  You will be able to select the priority from the options in the [[getting-started/create-or-edit-task|‘Create or edit Task’ Modal]].
- Using [[getting-started/auto-suggest|Intelligent Auto-Suggest]],
  start typing the first few characters of `high`, `medium` or `low`, and press <return> to accept the suggested signifier.

## Related Tasks Block Instructions

The following instructions use the priority signifiers in tasks.

- `priority is (above, below)? (low, none, medium, high)`
  - [[queries/filters#priority|Documentation]]
- `sort by priority`
  - [[queries/sorting#basics|Documentation]]
- `group by priority`
  - [[queries/grouping#basics|Documentation]]
- `hide priority`
  - [[queries/layout|Documentation]]

---

## View this page on the old documentation site

> [!Info] Request for feedback
> This page is an experimental migration of the Tasks user docs to Obsidian Publish. When the conversion is good enough, this will become the live site.
>
> For comparison, you can view [this page on the old documentation site](https://obsidian-tasks-group.github.io/obsidian-tasks/getting-started/priority/).

> [!Bug] Please report any problems
>
> We are keeping a list of [[migration#Current Status and Known Problems|Known Problems]] with the conversion.
>
> If you notice any other problems in this page, compared to the old one, please let us know in [#1706](https://github.com/obsidian-tasks-group/obsidian-tasks/issues/1706#issuecomment-1454284835).
>
> Please include:
>
> - The URL of the problem page
> - A screenshot of the problem.
>
> Thank you!
