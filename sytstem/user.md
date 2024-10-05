---
layout: default
title: system.user
parent: system
---

# system.user
User management module

## `user.getData(uid: number)`
Get data for a specific user.

### Parameters
1. uid: `number` ID of the user to retrieve.

### Returns
1. `table`: User data

or

1. `nil`: If the user does not exist

## `user.group.getData(gid: number)`
Get data for a specific group.

### Parameters
1. gid: `number` ID of the group to retrieve.

### Returns
1. `table`: Group Data

or

1. `nil`: If the group does not exist

## `user.create(name: string, password: string, [gid: number], [uid: number])`
Create a new user

### Parameters
1. name: `string` user name.
2. password: `string` user password.
3. gid: `number` Group to which the user belongs.
4. uid: `number` ID assigned to the user.

### Returns
1. `number`: Created user's id
   
## `user.delete(uid: number)`
delete user

### Parameters
1. uid: `number` ID of the user to be deleted.

### Returns
1. `table` or `nil` Returns the deleted user's data only if the deletion was successful.

## `user.group.create(name: string, [gid: number], [permission: string])`
Create a new group

### Parameters
1. name: `string` user name.
2. gid: `number` ID of the group to create
3. permission: `string` Permissions for the group to be created (in the format rwxrwxrwx)

### Returns
1. `number`: Created group's id
   
## `user.group.delete(gid: number)`
delete group

### Parameters
1. gid: `number` ID of the group to be deleted.

### Returns
1. `table` or `nil` Returns the deleted group's data only if the deletion was successful.
