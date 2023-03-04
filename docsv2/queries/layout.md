---
publish: true
---

# Layout commands

## Hiding/Showing Elements

You can hide and show individual elements of the rendered list with the "hide" and "show" commands
together with the name of the element.

The following elements exist:

- `edit button`
- `backlink`
- `urgency`
- `priority`
- `start date`
- `scheduled date`
- `due date`
- `done date`
- `recurrence rule`
- `task count`

> [!quote] Released
`urgency` was introduced in Tasks 1.14.0.

All of these elements except `urgency` are shown by default, so you will use the command `hide`
if you do not want to show any of them, or the command `show` to show the urgency score.

> [!quote] Released
The `show` commands were introduced in Tasks 1.14.0.

Example:

    ```tasks
    no due date
    path includes GitHub
    hide recurrence rule
    hide task count
    hide backlink
    show urgency
    ```

---

## Short Mode

In short mode, query results will only show the emojis, but not the concrete recurrence rule or dates.
You can hover over the task to see the rule and dates in a tooltip.

The command is `short mode`.

Example:

    ```tasks
    not done
    short mode
    ```

---

## View this page on the old documentation site

> [!Info] Request for feedback
> This page is an experimental migration of the Tasks user docs to Obsidian Publish. When the conversion is good enough, this will become the live site.
>
> For comparison, you can view [this page on the old documentation site](https://obsidian-tasks-group.github.io/obsidian-tasks/queries/layout/).

> [!Bug] Please report any problems
>
> We are keeping a list of [[migration#Current Status and Known Problems|Known Problems]] with the conversion.
>
> If you notice any other problems in this page, compared to [the old one](https://obsidian-tasks-group.github.io/obsidian-tasks/queries/layout/), please let us know in [#1706](https://github.com/obsidian-tasks-group/obsidian-tasks/issues/1706#issuecomment-1454284835).
>
> Please include:
>
> - The URL of this problem page
> - A screenshot of the problem.
>
> Thank you!
