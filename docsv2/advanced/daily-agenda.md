---
publish: true
---

# Daily Agenda

Using the default `Daily-notes` plugin, **templates** with syntax like
{% raw %}`{{date+14d:YYYY-MM-DD}}`{% endraw %} won't load dates properly. Nevertheless, **Liam Cain**,
author of both the [Calendar Plugin](https://github.com/liamcain/obsidian-calendar-plugin)
and [Periodic Notes Plugin](https://github.com/liamcain/obsidian-periodic-notes), has
written code to create new daily notes (using both plugins) using the `date+Xd` format.
Therefore, if you want to use this format instead of the standard `Daily-notes` syntax,
make sure new notes are created via one of these two plugins, and not `Daily-notes`.

- **Calendar Plugin**: Just tap the day on the Calendar UI and a new daily note will be created
- **Periodic Notes Plugin**: Install, migrate from `Daily-notes` if needed, and tap the new `Open Today` ribbon on the left-side dock. Below is an example if today was August 14, 2021.

| | Daily Notes | Calendar | Periodic Notes |
|-|-------------|----------|----------------|
| template syntax | `due on {% raw %}{{date+14d:YYYY-MM-DD}}{% endraw %}` | `due on {% raw %}{{date+14d:YYYY-MM-DD}}{% endraw %}` | `due on {% raw %}{{date+14d:YYYY-MM-DD}}{% endraw %}` |
| output | `due on {% raw %}{{date+14d:YYYY-MM-DD}}{% endraw %}` | `due on 2021-08-28` | `due on 2021-08-28` |

## Example Daily Agenda **template**

    ## Tasks
    ### Overdue
    ```tasks
    not done
    due before {% raw %}{{date:YYYY-MM-DD}}{% endraw %}
    ```

    ### Due today
    ```tasks
    not done
    due on {% raw %}{{date:YYYY-MM-DD}}{% endraw %}
    ```

    ### Due in the next two weeks
    ```tasks
    not done
    due after {% raw %}{{date:YYYY-MM-DD}}{% endraw %}
    due before {% raw %}{{date+14d:YYYY-MM-DD}}{% endraw %}
    ```

    ### No due date
    ```tasks
    not done
    no due date
    ```

    ### Done today
    ```tasks
    done on {% raw %}{{date:YYYY-MM-DD}}{% endraw %}
    ```

---

## View this page on the old documentation site

> [!Info] Request for feedback
> This page is an experimental migration of the Tasks user docs to Obsidian Publish. When the conversion is good enough, this will become the live site.
>
> For comparison, you can view [this page on the old documentation site](https://obsidian-tasks-group.github.io/obsidian-tasks/advanced/daily-agenda/).

> [!Bug] Please report any problems
>
> We are keeping a list of [[migration#Current Status and Known Problems|Known Problems]] with the conversion.
>
> If you notice any other problems in this page, compared to [the old one](https://obsidian-tasks-group.github.io/obsidian-tasks/advanced/daily-agenda/), please let us know in [#1706](https://github.com/obsidian-tasks-group/obsidian-tasks/issues/1706#issuecomment-1454284835).
>
> Please include:
>
> - The URL of this problem page
> - A screenshot of the problem.
>
> Thank you!
