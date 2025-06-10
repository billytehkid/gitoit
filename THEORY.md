# A todo list manager with a git backend

Let's see how this pans out...

## Concepts
Binder -> Git repository
Lists  -> Git branches
List   -> list.json

## Implementation
### Clients
clients/*
These are the various clients written in different languages.  
They should all behave more or less the same.

### Client operations
  1. Create new Binder          -> `git init`
  1. Connect to existing Binder -> `git clone`
  1. Create/delete list         -> `git branch`
  1. Switch list                -> `git switch`
  1. Add/delete/update task     -> *edit list.json*
  1. Synchronize                -> `git push/pull`
