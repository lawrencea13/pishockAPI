# pishockAPI
a quick API for using the shock/vibrate/beep functions with the pishock site.

# Example
The best practice would be to create 1 instance of this and use it throughout the lifetime of the program. Otherwise, you will need to redefine the user information.

```
  // test information
  api = new APIAccess
  {
      username = "puppy73",
      apiKey = "5c678926-d19e-4f86-42ad-21f5a76126db",
      code = "17519CD8GAP",
      senderName = "Program name"
  };

  _ = Task.Run(async () => await api.Shock(50, 2));
```
