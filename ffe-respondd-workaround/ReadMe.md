ffe-respondd-workaround
==============================

Checks whether respondd is still running and restarts it if necessary.

site.conf
---------

**respondd_workaround.step_size**
- execute the cronjob each x minutes

### example
```lua
{
  respondd_workaround = {
    step_size = 10,
  },
  ...
},
```
