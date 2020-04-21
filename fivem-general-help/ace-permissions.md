# ACE Permissions

**Principals**

A _principal_ is identifiers that hold permissions \(permissions will be referred to as aces\). These identifiers can either be player identifiers \(identification that represents a player's account such as their discord ID or steam ID for example\). They can also be made up identifiers. Made up identifiers can be thought of as _groups_. You can make groups simply when you add a principal.

**Example of adding a principal to a player and a group**

```text
add_principal identifier.discord:394446211341615104 group.admin 

# The above line in a server.cfg or permission.cfg will add the player
# who has the discord identifier 394446211341615104 to the group.admin group.
# It should also be noted that lines denoted with a # are commented and will be
# skipped by the .cfg parser.

add_principal group.admin group.moderator

# The above line will make moderator aces inherited by the admin group.
# So group.admin will get all of the same permissions that group.moderator gets. 
```

**ACE Permissions**

Now clearly you want to give yourself permissions to use certain commands in scripts using the ACE permissions system of FiveM. To do this, you can either add the ACE permission directly to one of your identifiers or to a group, then add yourself to the group. In most cases, you will probably utilize a group since then they can be set to multiple players without having to add a permission node for each player's identifiers.

```text
add_ace group.admin "BadgerTools.Spectate" allow

# The above line would give the group.admin permission to use /spectate 
# in the BadgerTools script.

add_principal identifier.discord:394446211341615104 group.admin

# The above line now sets the player to inherit all the permissions set up with
# group.admin.

add_ace identifier.discord:394446211341615104 "BadgerTools.Spectate" allow 

# The above line will add permission to use /spectate for only the player
# that matches having a discord identifier.

remove_ace group.admin "BadgerTools.Spectate" allow

# The above line will remove the allow status of a permission from the 
# group.admin. 

remove_ace identifier.discord:394446211341615104 "BadgerTools.Spectate" allow

# The above line will do the same as mentioned above, but will remove
# the allow status of the permission from the player that matches having
# the specified discord identifier ID.
```

