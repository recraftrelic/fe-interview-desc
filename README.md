# Frontend Javascript Developer Interview

The task is to write a React APP which let's user search a flatten array version of a tree structure

You have this structure

```
{
  "github": {
    "nodes": {
      "profile": {
        "type": "action"
      },
      "search": {
        "type": "action"
      },
      "repo": {
        "nodes": {
          "new": {
            "type": "action"
          },
          "pr": {
            "nodes": {
              "list": {
                "type": "action"
              }
            },
            "type": "folder"
          },
          "issues": {
            "nodes": {
              "list": {
                "type": "action"
              }
            },
            "type": "folder"
          }
        },
        "type": "folder"
      },
      "login": {
        "type": "action"
      },
      "logout": {
        "type": "action"
      }
    }
  }
}
```

The task is to write a function which takes the above tree and output this flat array

```
[
  "github profile",
  "github search",
  "github repo new",
  "github repo pr list",
  "github repo pr",
  "github repo issues list",
  "github repo issues",
  "github repo",
  "github login",
  "github logout",
  "github"
]
```

The next task it to build a search input in react and let user search through the list returned from the function
