Watcher
=======

Watcher observes and controls maintenance access on production IT assets, like databases and servers. It acts as man-in-the-middle between the maintainer and the TI asset, logging actions, filtering commands and recording outputs.

Usage scenario
--------------

Imagine troubles on a software and the developer needs production access to fix the bug. What happens if you can't trust the developer a credential to the production database server? You can give him a Watcher credential and fine grain control and monitor their queries. And if ssh access is also needed? You can use Watcher again.

*Disclaimer: Keep in mind that Watcher is in development.*

1. The system administrator create users with production access, like a user with permission to query a production database server or to ssh to a production web server. This user don´t need to be root, but just have access for basic incident handler. In fact, you can create as many users as your organization needs. You can create a user with simple access for basic troubleshooting and other with advanced permissions for more complex issues.
2. The Watcher administrator configure those users on Watcher, setting their  owners and access policies.
3. The troubleshooter ask permission to access Watcher with one of the users  created by the system administrator.
4. The user owner approves the access for a period and choose at least one  allowed access policy.
5. The troubleshooter access Watcher and start in browser query and ssh  manager to access the required servers. With this access he can send  queries and commands to server, but just the one the user created by the system administrator have permission.
6. The watchers and the user owner can real time monitor the troubleshooter. Depending  on the access policy, some commands sent from troubleshooter need approval. Also, everything is record for future auditing.
