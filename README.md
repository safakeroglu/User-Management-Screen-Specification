# User Management Screen Specification

## Overview
This document explains the specifications for User Management screen. It gives details about UI parts, how it works, and what developers need to do when making this screen.

## UI Parts

### 1. Header Actions
- **New User Button**: A button with "New User" text to add new user.
- **Hide Disabled User Checkbox**: A checkbox to show or hide users that are not active.
- **Save User Button**: A button with "Save User" text to keep changes.

### 2. User List Table
- Columns:
  - ID (can be ordered)
  - User Name (can be ordered)
  - Email (can be ordered)
  - Enabled status (can be ordered)
- Rows show user infos
- Different colors for every other row to see better

### 3. New User Form
- Places to write:
  - Username
  - Display Name
  - Phone
  - Email
  - User Roles (choose from list)
  - Enabled (tick box)

## How It Works

### When Page Opens
- Show the user list table with users already there
- Keep the "New User" form closed or hidden

### Adding New User
1. Click "New User" button
2. Show the New User form
3. Fill needed places
4. Pick user role(s) from list
5. Turn on or off "Enabled" tick box
6. Click "Save User" to put new user in list

### Hiding Users Not Active
- When "Hide Disabled User" is ticked, don't show users that are not active

### Ordering
- When you click column names in user list table, it should order the list

### Changing User Info
- Make a way to change user info (maybe click on a row to change)
- Use same form as "New User" but fill with old info

## What Is Needed

1. Screen should look good on all sizes
2. Check if info put in form is correct
3. Show errors and tell user what's happening
4. Make it easy for everyone to use (WCAG 2.1 AA)
5. Keep user info safe
6. Make it work fast even with many users

## More Ideas

- Add pages or endless scroll for lots of users
- Add search to find users easier
- Ask "Are you sure?" before doing important things (like making user not active)
- Add little help texts for hard parts

## Working with API

Make API points for:
- Getting user list
- Making new users
- Changing user info
- Turning user on or off

Make sure to handle errors and show loading when talking to API.
