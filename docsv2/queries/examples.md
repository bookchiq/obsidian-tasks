---
publish: true
---

# Examples

All open tasks that are due today:

    ```tasks
    not done
    due today
    ```

---

All open tasks that are due within the next two weeks, but are not overdue (due today or later):

    ```tasks
    not done
    due after yesterday
    due before in two weeks
    ```

---

All open tasks that are due within the next two weeks, and either have the #inbox tag, or are in an Inbox note:

    ```tasks
    not done
    (due after yesterday) AND (due before in two weeks)
    (tags include #inbox) OR (path includes Inbox)
    ```

---

All done tasks that are anywhere in the vault under a `tasks` heading (e.g. `## Tasks`):

    ```tasks
    done
    heading includes tasks
    ```

---

Show all tasks that aren't done, are due on the 9th of April 2021, and where the path includes `GitHub`:

    ```tasks
    not done
    due on 2021-04-09
    path includes GitHub
    ```

---

Show all open tasks that are due within two weeks and hide the due date and edit button:

    ```tasks
    not done
    due after 2021-04-30
    due before 2021-05-15
    hide due date
    hide edit button
    ```

---

Show all tasks that were done before the 1st of December 2020:

    ```tasks
    done before 2020-12-01
    ```

---

Show one task that is due on the 5th of May and includes `#prio1` in its description:

    ```tasks
    not done
    due on 2021-05-05
    description includes #prio1
    limit to 1 tasks
    ```

---

All open tasks that are due today or earlier, sorted by due date, then grouped together by the folder containing the task:

    ```tasks
    not done
    due before tomorrow
    sort by due
    group by folder
    ```

---

All open tasks that begin with a time stamp in `HH:mm` format, followed by any white space character:

    ```tasks
    not done
    description regex matches /^[012][0-9]:[0-5][0-9]\s/
    ```

---

## View this page on the old documentation site

> [!Info] Request for feedback
> This page is an experimental migration of the Tasks user docs to Obsidian Publish. When the conversion is good enough, this will become the live site.
>
> For comparison, you can view [this page on the old documentation site](https://obsidian-tasks-group.github.io/obsidian-tasks/queries/examples/).

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
