# Lean-To Roof Structural Diagrams

## Overview Diagram

```
                    SIDE VIEW (16' Length)
                    
    EXISTING SHED WALL                          
    |                                           
    |  Ledger Board (2x8, 7.5' height)        
    |  ═══════════════════════════════════════  
    |  ║ Rafter 1    Rafter 5    Rafter 9    ║  
    |  ║    \          \           \         ║  
    |  ║     \          \           \        ║  
    |  ║      \          \           \       ║  
    |  ║       \          \           \      ║  
    |  ║        \          \           \     ║  
    |  ║         \          \           \    ║  
    ────────────────────────────────────────────  Ground Level
         \         \          \           \
          \         \          \           \
           \         \          \           \ 
            \         \          \           \
         ════════════════════════════════════════  Beam (2x10x12 sistered)
         ║    ║              ║              ║    ║  6.42' height  
         ║    ║              ║              ║    ║
         ║    ║              ║              ║    ║
    ═════════════════════════════════════════════  Concrete Piers
       Post 1            Post 2            Post 3
      (4x4)             (4x4)             (4x4)
      
    <-- 8' --><------ 8' ------>
    <-------- 16' Total Length -------->
```

## Cross-Section Detail (Looking Along 16' Length)

```
                CROSS-SECTION VIEW - SIDE-SISTERED BEAM
                
        EXISTING SHED
        |
        |  Ledger Board
        |  ═══════════════
        |      Rafter (2x6)
        |         \
        |          \  13" Rise
        |           \
        |            \
        |             \  Rafter Length = 6.59'
        |              \
        |               \
        |                \
    ────────────────────────────────  Ground (7.5')
                         \
                          \
                    ╔════■════╗  Side-Sistered 2x12 Beam
                    ║ 2x12║2x12 ║  (Rafter sandwiched between)
                    ║    ║     ║  6.42' height
                    ╚════■════╝
                         ║
                      ═════════  Concrete Pier
                       4x4 Post
                       
    <--6' from shed--> <-6" overhang->
    <------- 6.5' Run ------->
    
    Pitch: 2:12 (2" rise per 12" run)
    Rise: 6.5' × (2/12) = 13 inches
    Beam Width: 3" total (1.5" + gap + 1.5")
```

## Rafter Detail - Side-Sistered Beam Connection

```
                RAFTER CONNECTION DIAGRAM - NO BIRD'S MOUTH REQUIRED
                
    ←------ 8' 2x6 Rafter ----→
    
    Ledger End                                      Overhang End
         |                                               |
         |         Side-Sistered Connection              |
         |                 ↓                            |
    ═════════════════════════════════════════════════════════
                       ╔═══════════╗  
                       ║  2x12 #1  ║  ← 1.5" thick
                       ║═══════════║  ← Rafter fits here (1.5" gap)
                       ║  2x12 #2  ║  ← 1.5" thick
                       ╚═══════════╝
                           ↑
                    Full Strength Rafter
                    (No structural notching)
                          
    Connection Details:
    - No bird's mouth cut required
    - Rafter maintains full 5.5" depth
    - 6" Torx structural screws: 4 per rafter connection
    - 2 screws each side through beam faces
    - Total connection width: 4.5" (1.5" + 1.5" + 1.5")
    - Angle maintained by ledger connection: 9.46° (2:12 pitch)
```

## Side-Sistered Beam Assembly & Post Connection

```
                SIDE-SISTERED BEAM ASSEMBLY
                
    ╔════════════════════════════════╗  2x12 Beam #1
    ║                                ║  
    ║         ○           ○          ║  ← 1/2" Carriage bolts, 16" OC
    ║                                ║    (connecting beam halves)
    ╠════════════════════════════════╣  ← 1.5" Gap for rafters
    ║                                ║
    ║         ○           ○          ║  ← 1/2" Carriage bolts, 16" OC
    ║                                ║
    ╚════════════════════════════════╝  2x12 Beam #2
                     ║
                     ║  4x4 Post
                     ║
                     ○  ← 1/2" x 10" Carriage bolt
                     ║    through both beam halves and post
                     ║
                     ║
                ═══════════  Concrete Pier
                Simpson Strong-Tie Bracket
                (already installed)

    Assembly Notes:
    - Beam halves temporarily bolted at ends for positioning
    - Post connection bolt goes through all three members
    - Rafter installation gaps beam halves to final 1.5" spacing
    - Final beam bolts installed at 16" centers between rafters
```

## Ledger Board Attachment Detail

```
                LEDGER-TO-WALL CONNECTION
                
    EXISTING SHED WALL STUDS (16" OC)
    ║        ║        ║        ║        ║
    ║   ○    ║   ○    ║   ○    ║   ○    ║  ← 1/2" x 6" Lag bolts
    ║        ║        ║        ║        ║    into studs
    ════════════════════════════════════════  Ledger Board (2x8)
    ╔══════════════════════════════════════╗  
    ║  Joist Hanger    Joist Hanger       ║  ← 2x6 Joist hangers
    ║      □               □              ║    24" on center
    ║                                     ║
    ╚═════════════════════════════════════╝
             Rafter fits here
             
    Flashing Detail:
    ┌─────────────────────────────────────┐
    │     Step Flashing Above Ledger      │  ← Weather protection
    └─────────────────────────────────────┘
```

## Purline Layout Diagram

```
                PURLINE SPACING (24" OC)
                Looking up from below
                
    Shed End ←                                    → Eave End
              
    ╔═══════════════════════════════════════════════════════════╗
    ║  Rafter 1   Rafter 2   Rafter 3   Rafter 4   Rafter 5   ║
    ║     │         │         │         │         │           ║
    ║═════│═══════════════════│═════════════════════│═══════════║ Purline 1
    ║     │         │         │         │         │           ║
    ║     │    24"  │    24"  │    24"  │    24"  │           ║
    ║═════│═══════════════════│═════════════════════│═══════════║ Purline 2
    ║     │         │         │         │         │           ║
    ║     │         │         │         │         │           ║
    ║═════│═══════════════════│═════════════════════│═══════════║ Purline 3
    ║     │         │         │         │         │           ║
    ║════╤╤═════════════════════════════════════════════════════║ Purline 4
    ║    ╘╤════════════════════════════════════════════════════║ Beam
    ╚═══════════════════════════════════════════════════════════╝
    
    Notes: 
    - 8 total purlines (4 per side of 16' span)
    - 2x4 lumber, 8' lengths joined at rafter intersections
    - Attached with 2.5" Torx exterior screws
```

## Foundation Layout Plan

```
                    PIER LAYOUT (Top View)
                    
              EXISTING SHED (16' long)
    ╔════════════════════════════════════════════════╗
    ║                    SHED                        ║
    ║                                                ║
    ╚════════════════════════════════════════════════╝
                                                      
    ←------- 6' from shed wall -------→
                                                      
         ●                    ●                    ●
      Pier 1               Pier 2               Pier 3
      (4x4)                (4x4)                (4x4)
       │                     │                     │
    ═══■═══               ═══■═══               ═══■═══
    Concrete              Concrete              Concrete
    
    <-- 8' spacing --><-- 8' spacing -->
    
    ⚠️  POTENTIAL ISSUE: Piers may not be perfectly aligned
        Solution: Use shims and string lines to correct
    
    ✅ COMPLETED: All piers poured with Simpson brackets installed
```

## Roofing Panel Layout

```
                METAL PANEL INSTALLATION
                (View from above)
                
    Shed Wall
    ├─────────────────────────────────────────────────────────┐
    │ L-Style     Panel 1    Panel 2    Panel 3    Panel 4   │
    │ Drip Edge      │         │         │         │        │
    │              16'│       16'│       16'│       16'│      │
    │                │         │         │         │        │
    │                │    Overlap      Overlap      │        │
    │                │    2-3 ribs    2-3 ribs      │        │
    │                │         │         │         │        │
    ├─────────────────────────────────────────────────────────┤
    │              D-Style Drip Edge                          │
    │              (6" overhang past beam)                    │
    └─────────────────────────────────────────────────────────┘
    
    Total Coverage: ~250 sq ft
    Panel width: typically 36" (3')
    Number of panels: 4-5 depending on coverage width
```

## Tool Setup and Work Area Layout

```
                RECOMMENDED WORK AREA SETUP
                
    EXISTING SHED
    ╔════════════════════════════════════════╗
    ║                SHED                    ║
    ║                                        ║
    ╚════════════════════════════════════════╝
                      │
         Material Storage & Cutting Area      │
    ┌─────────────────────────────────────────┼────┐
    │  ⚡ Miter Saw Station                  │    │
    │     (upgraded recommended)              │    │
    │                                        │    │
    │  📦 Lumber Stack                      │    │
    │     (8' & 12' pieces)                  │    │
    │                                        │    │
    │  🔧 Tool Staging:                     │    │
    │     • DeWalt Impact Driver             │    │
    │     • Level (4')                       │    │
    │     • Drill & Bits                     │    │
    └────────────────────────────────────────┼────┘
                                           │
         Clear Work Zone (no obstacles)     │
         for beam positioning              │
                                           │
      ●         ●         ●               │
   Pier 1    Pier 2    Pier 3            │
   
   Safety Zone: Keep 10' minimum clear space
   Helper Position: Near pier 2 for beam lifting
```

## Critical Measurements Reference

```
    QUICK REFERENCE MEASUREMENTS
    
    Overall Dimensions:
    • Total length: 16 feet
    • Run (horizontal): 6.5 feet  
    • Rise: 13 inches (2:12 pitch)
    • Ledger height: 7.5 feet
    • Beam height: 6.42 feet
    
    Component Sizes:
    • Rafters: 2x6 x 8' (9 pieces)
    • Beam: 2x10 x 12' (2 pieces, sistered)
    • Ledger: 2x8 x 8' (2 pieces, spliced)
    • Posts: 4x4 x 8' (3 pieces)
    • Purlines: 2x4 x 8' (16 pieces)
    
    Critical Cuts:
    • Bird's mouth: 1.5" x 3.5"
    • Rafter angle: 9.46° (2:12 pitch)
    • Overhang: 6 inches past beam
    
    Hardware Spacing:
    • Rafters: 24" on center
    • Purlines: 24" on center  
    • Lag bolts: 16" on center
    • Post spacing: 8 feet
```