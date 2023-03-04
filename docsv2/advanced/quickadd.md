---
publish: true
---

# Quickadd

The [quickadd](https://github.com/chhoumann/quickadd) plugin can help when creating tasks.
Additional to the official command to create a task, you can use a quickadd command with a custom capture format.

For example:

```markdown
{% raw %}#task {{VALUE:task name}} ⏰ {{VDATE:reminder date and time,YYYY-MM-DD HH:mm}} {{VALUE:⏫,🔼,🔽, }} 🔁 {{VALUE:recurrence}} 🛫 {{VDATE:start date,YYYY-MM-DD}} ⏳ {{VDATE:scheduled date,YYYY-MM-DD}} 📅 {{VDATE:due date,YYYY-MM-DD}}{% endraw %}
```

You can remove/leave some fields to make different types of tasks. And each one can have its own command.

## Some Examples

Task with due date only:

`{% raw %}#task {{VALUE:task name}} 📅 {{VDATE:due date,YYYY-MM-DD}}{% endraw %}`

<video controls width="100%">
    <source src="https://user-images.githubusercontent.com/38974541/143467768-cf183171-296c-4229-81ca-a8f820b7a66e.mov" />
</video>

---

Task with priority and reminder date and due date:

`{% raw %}#task {{VALUE:task name}} ⏰ {{VDATE:reminder date and time,YYYY-MM-DD HH:mm}} {{VALUE:⏫,🔼,🔽, }} 📅 {{VDATE:due date,YYYY-MM-DD}}{% endraw %}`

<video controls width="100%">
    <source src="https://user-images.githubusercontent.com/38974541/143468599-ae598f7d-cc84-4fc9-8293-eae72cf81f8a.mov" />
</video>

---

Task with recurrence and scheduled date and start date:

`{% raw %}#task {{VALUE:task name}} 🔁 {{VALUE:recurrence}} 🛫 {{VDATE:start date,YYYY-MM-DD}} ⏳ {{VDATE:scheduled date,YYYY-MM-DD}}{% endraw %}`

<video controls width="100%">
    <source src="https://user-images.githubusercontent.com/38974541/143468440-c83b5f91-c923-4f30-9c52-7c69e64978c9.mov" />
</video>

## How to add quickadd command

1. Install [nldates](https://github.com/argenos/nldates-obsidian) and [quickadd](https://github.com/chhoumann/quickadd)
2. choose the `capture` choice, then make it visible on the command palette by clicking on the flash emoji
3. Enable the `save as task` option, then enable the `capture format` option and paste your custom format

## Tip for repeated dates (to reduce friction)

If you notice that you are adding the same date multiple times, say for example the due date and the reminder date are the same.
Then you can give them the same name, this way you'll write the date only once and Quickadd will instert it in multiple places.

Here is the format for the current example:

```markdown
{% raw %}#task {{VALUE:task name}} ⏰ {{VDATE:same date,YYYY-MM-DD}} {{VDATE:time,HH:mm}} 📅 {{VDATE:same date,YYYY-MM-DD}}{% endraw %}
```

---

## View this page on the old documentation site

> [!Info] Request for feedback
> This page is an experimental migration of the Tasks user docs to Obsidian Publish. When the conversion is good enough, this will become the live site.
>
> For comparison, you can view [this page on the old documentation site](https://obsidian-tasks-group.github.io/obsidian-tasks/advanced/quickadd/).

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
