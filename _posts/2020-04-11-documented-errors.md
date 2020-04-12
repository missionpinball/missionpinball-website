---
layout: post
author: jab
title: Error Codes and Knowledgebase with Common Pitfalls and Solution
tags: [software, MPF, errors, knowledge_base]
---
Nobody likes error messages and we want to help you to get rid of them as fast
as possible.
For that reason, we added an error code and a link in 0.53.
We now started to write documentation for common errors (based on reports in
our forum).

If you see something like this:

    mpf.exceptions.config_file_error.ConfigFileError: Config File Error in ConfigValidator: Config validation error: Entry system11:system11:ac_relay_driver = "c_acSelect" is not valid. Device c_acSelect of type coils not defined Error Code: CFE-ConfigValidator-6 (https://docs.missionpinball.org/en/dev/logs/CFE-ConfigValidator-6.html)
    2020-04-11 13:37:13,337 : INFO : root : MPF run loop ended. 

Then you got successfully found error `CFE-ConfigValidator-6`.
If you want to get rid of it (in case the error itself is not clear) we
added a [page for that in the docs](https://docs.missionpinball.org/en/dev/logs/CFE-ConfigValidator-6.html).
We documented what the cause of this error is and what common pitfalls are
which might cause this error.

There are even [more documented errors](https://docs.missionpinball.org/en/dev/logs/index.html)
in the docs.
Have a look and let us know in the forum if we missed a common pitfall
somewhere ([contributions welcome](https://docs.missionpinball.org/en/dev/about/contributing_to_mpf_docs.html)
as usual).

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
