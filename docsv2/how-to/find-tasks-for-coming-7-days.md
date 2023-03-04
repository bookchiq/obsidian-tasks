---
publish: true
---

# Find all tasks for the coming 7 days

## Motivation

I would like to create a list of tasks that will be due in the coming 7 days.

How can I write this without using a hard-coded (fixed) date?

## tl;dr

Use `due before in 7 days`.

## The hard-coded way

This page was written on 8th September 2022, that is 2022-09-08, and the following search gave the desired results, using a fixed date:

    ```tasks
    not done
    due before 2022-09-15
    ```

## Setting up data to test the rules

Just as when writing software, when writing a new search rule it's worth generating good test data to satisfy yourself you really are getting the tasks you want.

In this case, as of `2022-09-08`, we want tasks up to and including `2022-09-15`, but no further. So here is a good continuous range of due dates, for testing our new search on that date:

```text
Example tasks, to test the filter:

- [ ] 0 days 📅 2022-09-08
- [ ] 1 days 📅 2022-09-09
- [ ] 2 days 📅 2022-09-10
- [ ] 3 days 📅 2022-09-11
- [ ] 4 days 📅 2022-09-12
- [ ] 5 days 📅 2022-09-13
- [ ] 6 days 📅 2022-09-14
- [ ] 7 days 📅 2022-09-15
- [ ] 8 days 📅 2022-09-16
- [ ] 9 days 📅 2022-09-17
```

With the above search, these tasks give this result:

```text
0 days 📅 2022-09-08
1 days 📅 2022-09-09
2 days 📅 2022-09-10
3 days 📅 2022-09-11
4 days 📅 2022-09-12
5 days 📅 2022-09-13
6 days 📅 2022-09-14
7 tasks
```

## The general way

The way to select dates before a specific future date is `before in ...`. So for our current search, we would use `due before in 7 days`:

    ```tasks
    not done
    due before in 7 days
    ```

With the above date, that search gives the desired result:

```text
0 days 📅 2022-09-08
1 days 📅 2022-09-09
2 days 📅 2022-09-10
3 days 📅 2022-09-11
4 days 📅 2022-09-12
5 days 📅 2022-09-13
6 days 📅 2022-09-14
7 tasks
```

## More Information

Relevant documentation sections:

- Some examples are written in the [[queries/filters#dates|Dates section of the Filters docs]].
- And perhaps more useful are the date-based examples in the [[queries/examples|Queries Examples page]].

---

## View this page on the old documentation site

> [!Info] Request for feedback
> This page is an experimental migration of the Tasks user docs to Obsidian Publish. When the conversion is good enough, this will become the live site.
>
> For comparison, you can view [this page on the old documentation site](https://obsidian-tasks-group.github.io/obsidian-tasks/how-to/find-tasks-for-coming-7-days/).

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
