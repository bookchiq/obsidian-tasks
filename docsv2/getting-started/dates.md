---
publish: true
---

# Dates

You don't have to use all available dates.
Maybe due dates are sufficient for you.
Don't over-engineer your task management.

> [!info]
> Instead of adding an emoji and a date manually, you can use the `Tasks: Create or edit` command when creating or editing a task.
When you use the command, you can also set dates like "Monday", "tomorrow", or "next week" and Tasks will automatically save the date in the correct format.
You can find out more in [[getting-started/create-or-edit-task|‘Create or edit Task’ Modal]].

> [!info]
> If you prefer to type, it is now very easy to add emojis and other information for you tasks using [[getting-started/auto-suggest|Intelligent Auto-Suggest]].

---

## 📅 Due

Tasks can have dates by when they must be done: due dates.
In order to specify the due date of a task, you must append the "due date signifier 📅" followed by the date it is due to the end of the task.
The date must be in the format `YYYY-MM-DD`, meaning `Year-Month-Day` with leading zeros.
For example: `📅 2021-04-09` means the task is due on the 9th of April, 2021.

```markdown
- [ ] take out the trash 📅 2021-04-09
```

---

## ⏳ Scheduled

Tasks can have dates on which you plan to work on them: scheduled dates.
Scheduled dates are different from due dates as you can schedule to finish a task before it is due.

Scheduled dates use an hourglass emoji instead of a calendar emoji.

```markdown
- [ ] take out the trash ⏳ 2021-04-09
```

See [[getting-started/use-filename-as-default-date|Use Filename as Default Date]] for how to optionally make Tasks use any dates in file names as the scheduled date for all undated tasks in that file.

> [!quote] Released
'Use Filename as Default Date' was introduced in Tasks 1.18.0.

---

## 🛫 Start

It can happen that you cannot work on a task before a certain date.
Or you want to hide a task until a certain date.
In that case you can use start dates.

Start dates use a departing airplane emoji instead of a calendar emoji.

```markdown
- [ ] take out the trash 🛫 2021-04-09
```

When [[queries/filters#start-date|filtering]] queries by start date,
the result will include tasks without a start date.
This way, you can use the start date as a filter to filter out any tasks that you cannot yet work on.

Such filter could be:

````markdown
```tasks
starts before tomorrow
```
````

## Finding mistakes in dates

Tasks does not automatically report any problem tasks that have invalid dates, such as on the 32nd day of a month. These task will silently not be found by date-based searches.

However, it is possible to search for any tasks with invalid dates in your vault: see
[[queries/filters#finding-tasks-with-invalid-dates|Finding Tasks with Invalid Dates]].

---

## View this page on the old documentation site

> [!Info] Request for feedback
> This page is an experimental migration of the Tasks user docs to Obsidian Publish. When the conversion is good enough, this will become the live site.
>
> For comparison, you can view [this page on the old documentation site](https://obsidian-tasks-group.github.io/obsidian-tasks/getting-started/dates/).

> [!Bug] Please report any problems
>
> We are keeping a list of [[migration#Current Status and Known Problems|Known Problems]] with the conversion.
>
> If you notice any other problems in this page, compared to [the old one](https://obsidian-tasks-group.github.io/obsidian-tasks/getting-started/dates/), please let us know in [#1706](https://github.com/obsidian-tasks-group/obsidian-tasks/issues/1706#issuecomment-1454284835).
>
> Please include:
>
> - The URL of this problem page
> - A screenshot of the problem.
>
> Thank you!
