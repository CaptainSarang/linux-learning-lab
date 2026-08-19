You've joined a Linux administration team. You've been given a directory called:

/home/josh/permissions-lab

Your job is to create some files and configure their permissions according to the company's requirements.

###Task 1 — Create the lab environment

Create:

/home/josh/permissions-lab

Inside it, create:

reports
scripts
private

Then verify that they exist.

###Task 2 — Create files

Inside reports, create:

daily-report.txt
financial-report.txt

Inside scripts, create:

backup.sh
monitor.sh

Inside private, create:

passwords.txt
###Task 3 — Configure report permissions

The company's policy says:

Everyone in the organization should be able to read the reports, but only the owner should be able to modify them.

Configure both files in reports accordingly.

Think carefully about:

owner
group
others

Then verify your result.

###Task 4 — Configure scripts

The scripts need to be executable by the owner, group, and others.

However:

Only the owner should be able to modify the scripts.

Configure both .sh files accordingly.

Verify your permissions.

###Task 5 — Protect the private file

passwords.txt contains sensitive information.

Company policy says:

Only the owner should be able to read or modify this file.

Configure the permissions appropriately.

Verify your result.

###Task 6 — Interpret permissions

Suppose you run:

ls -l

and see:

-rwxr-xr-x backup.sh
-rw-r--r-- daily-report.txt
-rw------- passwords.txt

Explain in your own words:

A. Who can execute backup.sh?

B. Who can modify daily-report.txt?

C. Who can read passwords.txt?

###Task 7 — Symbolic permissions

You have this file:

-rw-r--r--

You need to add execute permission to the owner only, without changing the existing permissions of the group or others.

What command would you use?

###Task 8 — Remove permissions

You have:

-rwxrwxrwx

The security administrator tells you:

Remove write permission from the group and others, but leave the owner's permissions unchanged.

What command would you use?

###Task 9 — Change ownership

Suppose the following users/groups exist:

alex
developers

You want:

Owner: alex
Group: developers

for:

scripts/backup.sh

What command would accomplish this?


...

## Results

[Show relevant ls -l output]

## What I Learned

[Your own explanation]
