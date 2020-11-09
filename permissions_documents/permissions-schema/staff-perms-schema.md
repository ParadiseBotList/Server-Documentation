---
sort: 1
---

# Staff Permissions

Below is a table of all current permissions and their hexidecimal values:

---

## Flags

###### Permission Flags

| Permission                 | Value                  | Description                                                 |
| -------------------------- | ---------------------- | ----------------------------------------------------------- |
| ADMINISTRATOR              | 0x0001                 | Grants all permissons. |
| VIEW_AUDIT_LOG             | 0x0002                 | Allows the user to view Audit Logs. |
| VIEW__SERVER_INSIGHTS      | 0x0003                 | Allows the user to view Server Insights. |
| SUPER_ADMIN                | 0x0004                 | Allows the user to edit Server Info (Name etc). |
| MANAGE_ROLES               | 0x0005                 | Allows the user to add and remove roles from members. |
| MANAGE_CHANNELS            | 0x0006                 | Allows the user to add, edit and delete channels.  |
| KICK_MEMBERS               | 0x0007                 | Allows the user to kick a server member.  |
| BAN_MEMBERS                | 0x0008                 | Allows the user to ban a server member. |
| CREATE_INVITE              | 0x0009                 | Allows the user to create server invites. |
| CHANGE_NICKNAME            | 0x0010                 | Allows the user to modify their nickname. |
| MANAGE_NICKNAMES           | 0x0011                 | Allows the user to modify any members nickname. |

> The default permission value for a staff member is `0x0001`.

---

## Schema

###### Permission Schema

| Permission                 | permLevel              | Description                                                 |
| -------------------------- | ---------------------- | ----------------------------------------------------------- |
| USER                       | 0                      | Allows execution of user level commands (help, ping etc) |
| BOT_DEV                    | 1                      | Allows for certification (User ID is stored internally) |
| BOT_OWNER                  | 2                      | Allows editing pages of all bots owned by the user. |
| MODERATOR                  | 3                      | Allows execution of some moderation commands |
| ADMINISTRATOR              | 4                      | Allows execution of all moderation commands |
| BOT_APPROVERS              | 5                      | Allows execution of all queue commands |
| PARADISE_DEV               | 6                      | Allows controlling, editing & reverting changes of the Paradise Bots project. |
| HEAD_ADMIN                 | 7                      | Allows execution of staff level commands (check etc) |
| PARADISE_OWNER             | 8                      | Allows controlling, editing & reverting changes of the Paradise Bots project. |

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
