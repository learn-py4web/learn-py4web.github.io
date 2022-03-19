# Code Changes

Since the lectures were recorded, some minor code changes were necessary to keep up with py4web evolution. 
We summarize here the main ones. 

## `action.uses` argument order

The template must now appear as the first (rather than last) argument of `action.uses`, so that what used to be written for isntance as 

```
action('index')
action.uses(db, auth.user, 'index.html')
def index():
    ...
```

is now written: 

```
action('index')
action.uses('index.html', db, auth.user)
def index():
    ...
```

## Tag import

`Tags` is now imported from `pydal.tools.tags` rather than `py4web.utils.tags` (this is usually in `common.py`).
