---
layout: post
title:  "SQL WITH Statement"
categories: [SQL]
---

The WITH statement is a replacement of subqueries. But it gives the ability to name and organize subqueries.

## Example
```SQL
    WITH 
    PublishedPosts AS (
        SELECT *
        FROM Posts
        WHERE Published = 1 
    ),
    AuthorsWithPublishedPosts AS
    (
        SELECT *
        FROM Authors AS a JOIN PublishedPosts AS p ON a.PostId = p.Id				
    )

    SELECT DISTINCT * FROM AuthorsWithPublishedPosts
```