# Getting Started

This page checks standard Markdown migration.

![Overview diagram](../assets/images/overview.png)

See [Authentication](./guides/authentication.md) for auth setup and [User model](../models/user.json) for model linking.

| Feature | Expected result |
| --- | --- |
| Table rendering | Preserved |
| Relative doc link | Resolved |
| Relative image | Imported and rendered |

```bash
curl https://api.example.com/users
```

<details>
  <summary>Raw HTML compatibility check</summary>
  HTML blocks may render differently and should be visually reviewed.
</details>
