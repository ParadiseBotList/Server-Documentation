---
sort: 3
---

# Moderation and Punishments

Moderating the server is relatively straight-forward.  I won't go through the entire [Paradise Bot Documentation](https://docs.paradisebots.net/commands) here but I will go over some of the specific commands we'll be using.

---

## Message/Chat Management

Chat management is fairly straight forward.  You can mass-delete messages.  This might be necessary to clean up any drama or inappropriate messages.

### Purge or delete messages

```
p>clear x
```

Where `x` is the number of messages to purge.  Keep in mind that purges do not show up in the official delete logs.

---

## User Management

### Mutes

Muting a member will add the "Muted" role to the user.  Muted members can:

- See the Information & Support channels.
- All other chat channels are hidden.

To mute a member, issue the following command:

```
p>mute @Someone <mute reason>
```

Some examples:

```
p>mute @Toxic Dev you're being to toxic.
```

Mutes will show in #mod-logs channel.

---

### Bans

Admins and Moderators have the delegated authority to ban users.

From a policy standpoint, indefinite bans should only be issued if there is a repeated offense by a member or if user is causing some sort of issue (i.e. raiding).  As a moderator, you are trusted to perform these actions judiciously and without malace.

Do not be afraid to use this power but know that you are wielding it.

To ban a member, issue the following command:

```
p>ban @Someone <reason>
```

Some examples:

```
p>ban @Toxic Dev You're a bit thirsty.  Come back after you've rehydrated.
```

### Mute vs. Ban

On the surface, mute and bans accomplish the same action: preventing the offending member from interacting with the rest of the server.  So why do one over the other?

A mute may be more appropriate for someone who is new to the server or someone who has been on the server a long time and needs "a time out".  If they are being a bit of an ass, isolating them so that they have to interact with the mod so they understand what they did wrong, with the ultimate goal being mutual understanding.  If the member understands, feel free to lift the mute early.

Bans, on the other hand, should be employed for cases involving egregious rule breaks, such as spamming, repeated harassment, etc.  Temp bans should lead to a full ban if the admin agrees.

A short cut to deciding between the two: if you want to talk to the offending user, mute.  If you just want them out of here, ban.

Both are reversable so don't feel bad if you choose incorrectly.  At the end of the day, remember it's about protecting members and both actions do just that.

