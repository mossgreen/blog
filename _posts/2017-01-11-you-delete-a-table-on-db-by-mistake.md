---
layout: post
title: What you should do after updating a table by mistake?
---

So sorry that I wrongly updated the database of company with the following script:

```
update dbo.country
set country = 'Australia'
 -- where countryID = 'AU'
```

I didn't select the last line, so that the data under country column had been updated. Origainal data lost and cannot be rollback. I write this blog to record what I've after that:

1. Call manager, report the mistake
2. Call DBA, ask for a backup instance
3. Migrate  the data back from the backup instance to production
4. Write an Email to tell manager all done

