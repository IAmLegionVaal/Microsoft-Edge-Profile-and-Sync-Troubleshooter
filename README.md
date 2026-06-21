# Microsoft Edge Profile and Sync Troubleshooter

Created by **Dewald Pretorius**.

The repository includes the original profile, sync, favorite, password, extension, policy, and sign-in diagnostics plus a guarded `Repair.ps1` helper.

Supported actions are `Diagnose`, `ResetSyncCaches`, and `FlushDns`.

```powershell
.\Repair.ps1 -Action Diagnose
.\Repair.ps1 -Action ResetSyncCaches -WhatIf
.\Repair.ps1 -Action ResetSyncCaches -Confirm
```

Close Edge before cache repair. Existing cache data is preserved in timestamped backups, and profile data is not changed. Source-reviewed for PowerShell 5.1; not runtime-tested against every Edge profile or management configuration.
