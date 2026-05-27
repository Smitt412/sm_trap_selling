# sm_trap_selling

Trap selling resource using `sm_bridge` for ESX, QBCore, Qbox, inventory, progress, notification, target, and dispatch adapters.

## Commands
- `/trap`
- `/stop-trap`
- `/traprank`

## Requirements
- `sm_bridge`
- `oxmysql`
- One supported framework or standalone identifiers
- One supported inventory configured in `sm_bridge/config.lua`

## Install
1. `ensure sm_bridge`
2. `ensure sm_trap_selling`
3. Edit `config.lua` and replace the `example_*` item placeholders with your inventory item names and pricing.

## Notes
- Dispatch is configured through `Config.policeAlert.dispatch` and resolved by `sm_bridge`.
- Notifications, progress bars, inventories, and payouts are routed through `sm_bridge`.
- Leave webhook logging disabled until you add your own webhook URL.
