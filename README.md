# Work In Progress
### TODO
1. setup.py
2. Documentation
3. Add `exec_from` to load template string from file
4. Add `load_state` to json.loads from a local file

# Example
```
# jinja-shell> set name.first leigh
Using string value
Setting name.first to leigh
# jinja-shell> set name.last martell
Using string value
Setting name.last to martell
# jinja-shell> print_state
{'name': {'first': 'leigh', 'last': 'martell'}}
# jinja-shell> clear
Cleared state
# jinja-shell> print_state
{}
# jinja-shell> set name {"first":"leigh","last":"martell"}
Setting name to {u'last': u'martell', u'first': u'leigh'}
# jinja-shell> print_state
{'name': {u'first': u'leigh', u'last': u'martell'}}
# jinja-shell> exec "First Name {{ name.first }} Last Name {{ name.last
| upper }}"
OUTOUT: "First Name leigh Last Name MARTELL"
# jinja-shell>
```
