# Lenovo.DE SDT Inventory (v1)

Tag taxonomy baseline:
`LNV.<TechId>.<Domain>[<Key>].<BlockType>`

TechId:
- `Lenovo.DE`

## System scope
Key (`<Key>`):
- system id or name (prefer stable id when available)

### Summary
- `LNV.Lenovo.DE.System[<SystemId>].Summary`

### Tables (core)
- `LNV.Lenovo.DE.System[<SystemId>].Tables.Systems` (systems inventory / identity)
- `LNV.Lenovo.DE.System[<SystemId>].Tables.Controllers` (controllers if collected)
- `LNV.Lenovo.DE.System[<SystemId>].Tables.Drives`
- `LNV.Lenovo.DE.System[<SystemId>].Tables.StorageContainers` (VG + DDP)
- `LNV.Lenovo.DE.System[<SystemId>].Tables.Volumes`

### Findings (optional v1 placeholder)
- `LNV.Lenovo.DE.System[<SystemId>].Findings`

### Evidence placeholder
- `LNV.Lenovo.DE.System[<SystemId>].Evidence.Placeholder`

## Notes
- Volume Groups and Disk Pools (DDP) are presented together as StorageContainers in v1.
- Future datasets (events/alerts) may add:
  - `LNV.Lenovo.DE.System[<SystemId>].Tables.Events`
  - `LNV.Lenovo.DE.System[<SystemId>].Tables.Alerts`
