# Deposito (Warehouse) - Department Knowledge

## Overview

The Deposito (Warehouse) is the central material hub for all Lakeshore Development construction projects. Managed by Klauser Silva ("Seu Clauser"), it handles receiving, quality control, stock management, and distribution of construction materials to job sites. The warehouse operates as the physical bridge between purchasing (Compras) and field construction (Supervisao/Scheduling), ensuring the right materials reach the right house at the right time.

## Receiving & Quality Control

### Material Receiving Process
1. **Delivery arrives** -- verify delivery truck and supplier against expected schedule
2. **Check against PO** -- compare delivered items (type, quantity, condition) against the Purchase Order from Compras
3. **Inspect quality** -- visual inspection for damage, correct specifications, material condition
4. **Sign delivery receipt** -- acknowledge receipt on supplier's delivery document
5. **Register in Zorro** -- enter received materials into the Zorro warehouse management system
6. **Notify Compras** -- confirm receipt with PO reference and any discrepancies

### QC Checks
- **Quantity match**: Count delivered units against PO quantity
- **Material condition**: Check for damage during transport (broken blocks, bent lumber, water-damaged drywall)
- **Specification compliance**: Verify material grade, size, color matches PO specifications
- **Packaging integrity**: Ensure packaging is intact (important for flooring, fixtures, hardware)

### Rejection Workflow
When material arrives damaged, wrong, or does not match the PO:
1. **Photograph** the issue (damage, wrong item, shortage)
2. **Do not sign** full acceptance on delivery receipt -- note discrepancy
3. **Notify Compras** (Brenda) immediately with photos and PO reference
4. **Compras arranges** return/replacement with supplier
5. **Log rejection** in Zorro with reason code

### Validation Limitation
Clauser receives materials and distributes them to job sites, but cannot autonomously validate incoming shipments against PO details or takeoff quantities. When discrepancies are noticed (wrong quantities, wrong materials, damaged goods), he flags them to Compras for resolution. This creates a bottleneck when Brenda is unavailable and materials need to go out urgently.

## Destination Allocation by Project

- Each delivery is tagged with the project/house number it is destined for
- Material staging areas in the warehouse are organized by active project
- **Allocation priority**: active construction phase > upcoming phase (pre-staging) > general stock
- Distribution is tracked in both Zorro (Sales Orders) and Compras spreadsheets for cost accounting

### Per-House Tracking
- Every material exit from the warehouse creates a Zorro Sales Order tied to a specific house number
- This enables cost-per-house tracking for financial closing
- Materials not yet assigned to a house remain in general stock until Compras allocates them

## Zorro Sales Orders

- **Zorro** is the warehouse management software for tracking stock movements
- **Sales Orders (SO)** are created when material leaves the warehouse for a project
- **Draft SOs**: Clauser uses drafts to separate/reserve materials before formal dispatch -- drafts are not yet confirmed
- **Reconciliation**: daily check that SO quantities match physical dispatch records
- **Known issue**: Zorro does not reference which original purchase lot the material came from, making cost traceability per house difficult
- **Known issue**: Confirmed houses sometimes show missing exit records in Zorro -- flagged during closing

## Reorder Notifications

- **Automated reorder point monitoring** for high-usage materials via the `set_reorder_point` tool
- **Notification chain**: stock falls below threshold -> alert Compras agent -> Compras generates PO or adds to monthly bulk order
- **Safety stock calculation**: 2-week buffer for critical materials:
  - Concrete/cement: 2-week supply based on active pour schedule
  - Lumber: 2-week supply based on framing schedule
  - Rebar: 2-week supply based on foundation schedule
  - Blocks (8x8x16): 2-week supply based on masonry schedule
- **Seasonal adjustment**: During peak construction season (March-June), safety stock increases to 3-week buffer

## Scheduling Material Request Integration

- **48-hour advance notice**: Scheduling agent sends material needs at least 48 hours before phase start
- **Pick list preparation**: Warehouse prepares materials based on Scheduling's request and takeoff quantities
- **Staging**: Materials are staged in the dispatch area by house number and delivery date
- **Delivery coordination**: 
  - Internal truck schedule for warehouse-to-site delivery
  - Supplier direct-to-site for large items (concrete, lumber packages, trusses)
  - Core Craft handles appliance and specialty deliveries

## Daily Operations

### Morning Routine
- Review incoming deliveries scheduled for today (from Compras delivery calendar)
- Check overnight stock alerts (items that fell below reorder point)
- Prepare outgoing pick lists for scheduled dispatches

### Midday Operations
- Process receipts for morning deliveries -- update Zorro stock levels
- Execute material dispatches to job sites per Scheduling requests
- Handle walk-in requests from field supervisors (urgent material needs)

### End of Day
- Reconcile Zorro Sales Orders against physical dispatch log
- Flag any discrepancies (missing exits, unconfirmed drafts, quantity mismatches)
- Update reorder status -- notify Compras of items approaching threshold
- Secure warehouse and update next-day delivery schedule

## Daily Assignment-to-Takeoff Reconciliation

Clauser performs a daily reconciliation: check what materials were assigned to specific houses against what the takeoff specifies for those houses. When discrepancies are found -- for example, more material sent than the takeoff calls for, or material sent to a house not in the current schedule -- Clauser flags the discrepancy to Compras (Brenda) for resolution.

## Key Systems and Tools

| System | Purpose | Used For |
|--------|---------|----------|
| Zorro | Warehouse management | Stock levels, Sales Orders, receiving, dispatch tracking |
| Excel spreadsheets | Backup tracking | Distribution records, cost allocation per house |
| Builder Trend | Project management | PO reference, house schedules, cost codes |

## Dependencies

- **Receives from**: Compras (PO details, delivery schedules, supplier info), Scheduling (material requests 48h ahead), Supervisao (urgent field requests)
- **Delivers to**: Supervisao/Field (construction materials), Scheduling (availability confirmations), Compras (receipt confirmations, discrepancy alerts, reorder triggers), Financeiro (distribution data for cost closing)

## Key Personnel

- **Klauser Silva ("Seu Clauser")** -- Warehouse manager, responsible for physical stock control, receiving, and distribution

## Navigation

- [Indice Geral](INDICE.md)
- [Mapa de Dependencias](04_MAPA_DEPENDENCIAS.md)
- **Departamentos relacionados:**
  - [Compras](dept_compras.md) -- purchasing, PO management, supplier coordination
  - [Scheduling](dept_scheduling.md) -- material request scheduling, phase coordination
  - [Supervisao](dept_supervisao.md) -- field material needs, delivery verification
  - [Financeiro](dept_financeiro.md) -- cost allocation per house, closing reconciliation
  - [Core Craft](dept_core_craft.md) -- appliance deliveries, specialty materials

---

## BuilderTrend Job 455 -- Real Data

### Material Flow Through Warehouse for Job 455
Job 455 required 122 Purchase Orders ($150,850.83 total). Materials flowed through the warehouse in these categories:

**Stocked Materials (from warehouse)**:
| Material | Vendor | Cost | Warehouse Handling |
|----------|--------|------|-------------------|
| Foundation Material (rebar, poly, bar chair, tape) | Cast Crete | Various | Receive, QC, distribute to site |
| Blocks | Cemex | $5,713 | Large delivery, staged on slab |
| Lumber | 84 Lumber | $6,177 | Deliver to back of property (theft prevention) |
| Shingles | Various | Included in roofing | Stocked material |
| Interior Doors + Trim Set | Home Depot | $1,030 (bifolds) + $914 (front doors) | Receive, store, distribute per house |
| Door Knobs, Door Stops | Lowes/Amazon | $292 | Small items, stocked |
| Shelves, Brackets | Home Depot/Lowes | $194 | Stocked items |
| Bathroom Kits | Amazon | $58 | Stocked items |
| Light Fixtures | Amazon | $3.79-$76.37 per unit | Receive, check specs, distribute |
| Electronic Lockers | Amazon/Costco | Various | Security items, stocked |
| Builders Paper, Blue Tape | Home Depot/Lowes | $36 | Consumable stocked items |
| Vinyl Material | AMERICAN STORE LLC | $2,808 | Stocked flooring material |
| Tile Material | Various | Included in finishing | Stocked material |
| Casings and Baseboards | Imeca Web POS | $970 | Linear measurement items |

**Direct-to-Site Materials (bypass warehouse)**:
| Material | Vendor | Cost | Reason |
|----------|--------|------|--------|
| Trusses | Truss Direct LLC | $6,500 | Oversized, delivered directly to site |
| Lintel Concrete | Del Zotto Concrete LLC | $1,693 | Wet pour, time-sensitive |
| Windows | Various | $22,368 | Direct from manufacturer |
| Cabinets/Countertop | ONYX GRANITE | $6,978 | Custom-fit, direct install |
| Garage Door | Strong Quality | $1,850 | Direct install by sub |
| Driveway Pavers | Red Twelve LLC | $5,053 | Direct to site |

### Material Suppliers for Warehouse Stock
| Supplier | Material Categories | Est. PO Count |
|----------|-------------------|---------------|
| Home Depot | Doors, hardware, shutters, shelves, tiles, builders paper | 8+ |
| Amazon | Bathroom kits, brackets, mirrors, lockers, light fixtures, plumbing trim | 7+ |
| Lowes | Door knobs, garden set, shelves, vinyl, builders paper | 4+ |
| AMERICAN STORE LLC | Vinyl material | 1 |
| Imeca Web POS | Casings and baseboards | 1 |
| Costco | Electronic lockers, garden set | 2 |

## CPM Construction Sequence -- Warehouse Touchpoints

### Material Delivery Timing from CPM
1. **Foundation Material**: Order after UP Inspection scheduled; must arrive AFTER UP Inspection approval. If UP fails, verify warehouse has not received materials (theft risk if sitting on site)
2. **Blocks**: Must arrive 2 days AFTER slab pouring (stored on slab -- needs cure time)
3. **Precast Delivery Request**: Request to arrive after Masonry Assembly
4. **Lumber**: Deliver to BACK of property to reduce theft risk
5. **Trusses**: ETA = Foundation Material ETA + 2 weeks; never request Monday delivery
6. **Trim Set Material**: Must arrive during final Cabinets/Granite phase, BEFORE Trim Set starts. House must have Garage Door + Electronic Locker (theft protection)
7. **Windows/Doors Material**: Manufacturing request after Stake House; delivery before framing

### Warehouse Role in CPM Sub-Systems
- **Property Area Development**: Loads delivery tracking (amount_delivered >= amount_requested check)
- **Windows and Doors**: Receive manufactured windows, store if needed, distribute when installation scheduled
- **Exceeding Costs**: Purchase Upgrade path involves warehouse receiving upgraded materials

## Const App Integration

### Stock Module in Const App
- **Stock Levels** (/stock/stock_levels): View cumulative stock requirements from active projects; columns track COMPONENT NAME, CATEGORY, SUPPLY TYPE, SUPPLIER, REQUIRED QUANTITY, CURRENT STOCK, PROJECTED STOCK
- **Material Purchases** (/stock/stock_material_purchases): Register and track material purchase orders with delivery status
- **Material Pickups** (/stock/material_pickups): Coordinate material pickup from suppliers; confirm warehouse separation
- **Extraordinary Orders** (/stock/extraordinary_orders): Request materials outside normal stock replenishment; requires justification and approval

### Supply Type Classification (Const App)
| Type | Description | Warehouse Role |
|------|-------------|---------------|
| Stocked | Material in warehouse available for distribution | Full receive/QC/store/distribute cycle |
| Quoted | Requires vendor quotation | Track PO, receive when ordered |
| By Sub | Provided by subcontractor | Does not pass through warehouse |

### Service Catalog Material Codes
| Code | Service | Nature | Procurement |
|------|---------|--------|-------------|
| FND-001 | Foundation Material | Material | Stocked |
| MAS-001 | Blocks | Material | Stocked |
| ROF-002 | Lumber | Material | Stocked |
| ROF-003 | Hardware | Material | Stocked |
| ROF-007 | Shingles | Material | Stocked |
| WIN-002 | Windows Material | Material | Stocked |
| WIN-004 | Front Door Material | Material | Stocked |
| DOR-001 | Interior Doors and Trim Set | Material | Stocked |
| DOR-003 | Interior Doors | Material | Stocked |
| DOR-004 | Trim Set | Material | Stocked |
| DOR-006 | Door Knob and Door Stop | Material | Stocked |
| PLM-002 | Plumbing Fixtures | Material | Stocked |
| PLM-006 | Plumbing Materials | Material | Stocked |
| ELC-002 | Electrical Fixtures | Material | Stocked |
| FIN-004 | Insulation | Material | Stocked |
| FIN-007 | Flooring | Material | Stocked |
| FIN-008 | Tile Material | Material | Stocked |
| FIN-009 | Vinyl Material | Material | Stocked |
| FIN-012 | Cabinets and Countertop | Material | Stocked |
| FIN-013 | Appliances | Material | Stocked |
| SPC-001 | Shelves, Mirrors, Bath Kit | Material | Stocked |
| SPC-002 | Electronic Lock | Material | Stocked |
| SPC-003 | House Numbers | Material | Stocked |
| LND-008 | Wooden Fence Material | Material | Stocked |
| EXT-006 | Irrigation Hose | Material | Stocked |
| EXT-007 | Irrigation Timer | Material | Stocked |
| EXT-008 | Plants | Material | Stocked |
| EXT-009 | Sprinklers | Material | Stocked |
