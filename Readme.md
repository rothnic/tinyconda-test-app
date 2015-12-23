### Quickstart with Example App
Assuming you have docker installed. The example uses pandas and click to demonstrate
that we can use pre-combiled libraries and pip-installed libraries. The example
modifies the example click app to build up a DataFrame of greetings.

1. Clone this repository
3. `make build`
4. `make run`

**Output**

```

# uses default CMD in Dockerfile
→ docker run --rm -it test_app /app/app.py
Your name: Nick
  greeting  name
0    Hello  Nick

# overrides CMD in Dockerfile
→ docker run --rm -it test_app /app/app.py --count=3
Your name: Nick
  greeting  name
0    Hello  Nick
1    Hello  Nick
2    Hello  Nick

→ docker run --rm -it test_app /app/app.py --count=3 --greeting=Yo
Your name: Nick
  greeting  name
0       Yo  Nick
1       Yo  Nick
2       Yo  Nick
```
