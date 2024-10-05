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

