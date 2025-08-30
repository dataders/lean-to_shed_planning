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
                CROSS-SECTION VIEW
                
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
                        ═══════  Beam (sistered 2x10s)
                          ║      6.42' height
                          ║
                          ║
                      ═════════  Concrete Pier
                       4x4 Post
                       
    <--6' from shed--> <-6" overhang->
    <------- 6.5' Run ------->
    
    Pitch: 2:12 (2" rise per 12" run)
    Rise: 6.5' × (2/12) = 13 inches
```

## Rafter Detail with Bird's Mouth Cut

```
                RAFTER CUTTING DIAGRAM
                
    ←------ 8' 2x6 Rafter ----→
    
    Ledger End                                      Overhang End
         |                                               |
         |           Bird's Mouth Cut                    |
         |                 ↓                            |
    ═════════════════════════════════════════════════════════
                             ┌─────┐  
                             │ 1.5"│  ← Horizontal cut
                             │     │
                             │ 3.5"│  ← Vertical cut  
                             └─────┘
                               ↑
                          Beam Contact
                          
    Measurements:
    - Total rafter length: 8' (7.09' needed + waste)
    - Bird's mouth depth: 1.5" (beam width)
    - Bird's mouth height: 3.5" (sits on beam top)
    - Angle: 9.46° (2:12 pitch angle)
```

## Beam Connection Detail

```
                BEAM-TO-POST CONNECTION
                
    ════════════════════════════════  Sistered 2x10 Beam
    ║ 2x10 #1    ║    2x10 #2      ║  (joined with carriage bolts)
    ║            ║                 ║
    ║    ○       ║        ○        ║  ← 1/2" Carriage bolts, 16" OC
    ║            ║                 ║
    ════════════════════════════════
                 ║
                 ║  4x4 Post
                 ║
                 ○  ← 1/2" x 8" Carriage bolt
                 ║    through beam and post
                 ║
                 ║
            ═══════════  Concrete Pier
            Simpson Strong-Tie Bracket
            (already installed)
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