# Aether for Windows (Scoop)

Use a normal PowerShell window (not "Run as administrator" - Scoop refuses that).

**1. Install Scoop** (skip if `scoop --version` already works)

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

**2. Install git** (Scoop needs it to add Aether's bucket)

```powershell
scoop install git
```

**3. Install Aether**

```powershell
scoop bucket add aether https://github.com/vansh7266/scoop-aether
scoop install aether
```

**4. Set up and start**

```powershell
aether setup
aether start
```

Then press **Ctrl+Shift+Space**.

Update: `scoop update; scoop update aether` - Uninstall: `aether uninstall`, then `scoop uninstall aether`.
Downloads come from [aether-releases](https://github.com/vansh7266/aether-releases).
