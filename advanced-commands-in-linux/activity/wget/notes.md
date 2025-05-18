# 🧠 Advanced Commands in Linux

**Topic(s):** Download anything with wget & Shorten the wget command

---

## 📌 Summary

A short summary of what was covered.

> Introduced essential Linux commands for navigating and managing the file system using `cd`, `ls`, `pwd`, `mkdir`, and `rmdir`.
> Following commands that was introduced. `wget`, and `man`.

---

## 💻 Exercises

Below are the commands I used to perform the activity. Trial and Error.

> wget

> man wget

> wget [url]

> wget [url] —page-requisites

> wget [url] —page-requisites —rejected-log-rejects.log

> wget [url] —page-requisites —rejected-log-rejects.log —span-hosts

> wget [url] —page-requisites —rejected-log-rejects.log —span-hosts —convert-links

And there's a part creating get.sh file. Below is the command structure:

wget [url] \
--page-requisites \
—-rejected-log-rejects.log \
—-span-hosts \
—-convert-links
—-recursive \
—-level=inf \
—-no-parent \
—-wait=2 \
—-limit-rate=1024k

This is the part get.sh needed to change the permission first.

> chmod +x ./get.sh

Then run, ./get.sh

Shortening the wget command. Get version first.

> wget or > wget —-version

Final command for the ‘get.sh’ file:

> wget [url] -p -k -r -l inf -np

or you can use:

> wget [url] -pkrlinf -np
