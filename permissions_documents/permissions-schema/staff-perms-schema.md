---
sort: 1
---

# Staff Permissions

Below is a table of all current permissions and their hexidecimal values:

---

## Flags
* Highest to Lowest

###### Permission Flags

| Permission                 | Value                  | Description                                                 |
| -------------------------- | ---------------------- | ----------------------------------------------------------- |
| SUPER_ADMIN                | 0x0001                 | Grants all permissons including Server Management. |
| ADMINISTRATOR              | 0x0002                 | Grants all permissons excluding Server Management. |
| VIEW_AUDIT_LOG             | 0x0003                 | Allows the user to view Audit Logs. |
| VIEW__SERVER_INSIGHTS      | 0x0004                 | Allows the user to view Server Insights. |
| MANAGE_ROLES               | 0x0005                 | Allows the user to add and remove roles from members. |
| MANAGE_CHANNELS            | 0x0006                 | Allows the user to add, edit and delete channels.  |
| KICK_MEMBERS               | 0x0007                 | Allows the user to kick a server member.  |
| BAN_MEMBERS                | 0x0008                 | Allows the user to ban a server member. |
| CREATE_INVITE              | 0x0009                 | Allows the user to create server invites. |
| CHANGE_NICKNAME            | 0x0010                 | Allows the user to modify their nickname. |
| MANAGE_NICKNAMES           | 0x0011                 | Allows the user to modify any members nickname. |

---

## Default Permissions

> ‼️ The default permission value for a staff member is `0x0001`.

---

## Schema

###### Permission Schema

| Permission                 | Level                  | Highest Value                   | Description                            |
| -------------------------- | ---------------------- | ------------------------------- | -------------------------------------- |
| MODERATOR                  | 1                      | 0x0003.                         | Responsible for Moderating the Server. |
| ADMINISTRATOR              | 2                      | 0x0002.                         | Responsible for Administrator Actions. |
| BOT_APPROVERS              | 3                      | 0x0002.                         | Responsible for the Bot List itself.   |
| PARADISE_DEV               | 4                      | 0x0001.                         | Responsible for the website maintenance.|
| HEAD_ADMIN                 | 5                      | 0x0001.                         | Responsible for the Staff Team as a whole.|
| PARADISE_OWNER             | 6                      | 0x0001.                         | Responsible for Paradise Bots as a whole. |

---

## Permission Hierarchy
* `Paradise Owners`
* `Head Admin`
* `Paradise Dev`
* `Administrator`
* `Approvers`
* `Moderators`

---

## Calculating a User's Permissions

Paradise Bots permissions are only a additive. Therefore a user's permissions are always exactly the union of their personal permissions and the permissions of every role that they have
