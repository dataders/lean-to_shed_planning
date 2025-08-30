# Structural Calculations and Engineering Notes

## Project Parameters
- **Roof Span**: 16 feet long
- **Roof Pitch**: 2:12 (2" rise per 12" run)  
- **Run**: 6.5 feet horizontal projection
- **Rafter Spacing**: 24" on center
- **Live Load**: 20 psf minimum
- **Dead Load**: ~15 psf (estimated)

## Rafter Calculations

### Basic Geometry
```
Run = 6.5 feet = 78 inches
Rise = 78" × (2/12) = 13 inches
Pitch Angle = arctan(2/12) = 9.46°
```

### Rafter Length Calculation
```
Theoretical Length = √(run² + rise²)
= √(78² + 13²)
= √(6084 + 169)
= √6253
= 79.08 inches = 6.59 feet
```

### Actual Rafter Length (including overhangs)
```
Rafter Length = Theoretical + Overhangs
= 6.59' + 0.5' (eave overhang)
= 7.09 feet
Specify: 8' 2x6 rafters (allows for cutting/waste)
```

### Bird's Mouth Cut Dimensions
For 2x beam (actual 1.5" x 9.25"):
```
Horizontal Cut (seat) = 1.5" (beam width)  
Vertical Cut (plumb) = 3.5" (maximum for 2x6)
Remaining Rafter Depth = 5.5" - 3.5" = 2.0" (adequate)
```

## Beam Sizing Analysis

### Load Calculations
```
Tributary Width = 6.5 feet (roof run)
Dead Load = 15 psf × 6.5' = 97.5 plf
Live Load = 20 psf × 6.5' = 130 plf
Total Load = 227.5 plf
```

### Beam Span and Loading
```
Beam Span = 16 feet
Total Uniform Load = 227.5 plf
Maximum Moment = (wL²)/8 = (227.5 × 16²)/8 = 7,280 ft-lbs
```

### Section Modulus Requirements
```
Allowable Bending Stress (Douglas Fir) = 900 psi
Required Section Modulus = M/Fb = 7,280 × 12 / 900 = 97.1 in³
```

### Beam Options Analysis
| Beam Size | Section Modulus | Adequate? | Notes |
|-----------|----------------|-----------|--------|
| 2x10 | 49.9 in³ | **NO** | Undersized |
| 2x12 | 73.8 in³ | **NO** | Still undersized |
| (2) 2x10 | 99.8 in³ | **YES** | Recommended option |
| (2) 2x12 | 147.6 in³ | **YES** | Conservative option |
| 4x10 | 230.8 in³ | **YES** | Overkill but simple |

**Recommendation**: Use (2) 2x10s sistered together with 1/2" carriage bolts every 16".

## Post Sizing Verification

### Column Load Calculation
```
Tributary Area per Post = 16' × 6.5' ÷ 3 posts = 34.7 sq ft
Load per Post = 34.7 sq ft × 35 psf = 1,215 lbs
```

### 4x4 Post Capacity
```
Actual 4x4 dimensions = 3.5" × 3.5" = 12.25 in²
Unbraced Length = ~6.5 feet = 78"
Slenderness Ratio = 78/3.5 = 22.3
Allowable Load = ~2,500 lbs (Douglas Fir)
Safety Factor = 2,500/1,215 = 2.06 (adequate)
```

## Connection Details

### Ledger Board Connection
```
Ledger Load = 227.5 plf × 16' = 3,640 lbs total
Number of Lag Bolts = 12 (16" OC)
Load per Bolt = 3,640/12 = 303 lbs
1/2" Lag Bolt Capacity = ~400 lbs (adequate)
```

### Rafter Hanger Sizing
```
Reaction per Rafter = 227.5 plf × 2' = 455 lbs
2x6 Joist Hanger Capacity = ~565 lbs (adequate)
Use galvanized hangers with proper nails
```

## Deflection Analysis

### Beam Deflection Check
```
Moment of Inertia (2) 2x10 = 2 × 98.9 = 197.8 in⁴
E (modulus of elasticity) = 1,400,000 psi
Deflection = (5wL⁴)/(384EI)
= (5 × 227.5 × 16⁴ × 1728)/(384 × 1,400,000 × 197.8)
= 0.52 inches
```

### Deflection Limits
```
L/240 = 16' × 12/240 = 0.8" (allowable)
Actual deflection = 0.52" < 0.8" ✓ (acceptable)
```

## Wind Load Considerations

### Basic Wind Load (simplified)
```
Design Wind Speed = 90 mph (typical residential)
Wind Pressure = ~20 psf uplift on roof
Uplift per Rafter = 20 psf × 2' × 6.5' = 260 lbs
Rafter connections must resist uplift
```

### Recommendations
- Use hurricane ties at beam connections
- Ensure adequate fastener penetration
- Consider impact of roof slope on wind loads

## Snow Load (Regional Variation)

### Typical Snow Loads by Region
- **Light Snow**: 20 psf (southern regions)
- **Moderate Snow**: 30-40 psf (central regions)  
- **Heavy Snow**: 50+ psf (northern/mountain regions)

### Design Recommendation
Current design based on 20 psf live load. For higher snow loads:
- Increase to 2x12 beam or add center support
- Reduce rafter spacing to 16" OC
- Verify local building code requirements

## Code Compliance Notes

### International Building Code (IBC)
- Minimum live load: 20 psf (satisfied)
- Deflection limits: L/240 (satisfied)
- Connection requirements: Per manufacturer
- Ventilation: May require soffit/ridge vents

### Local Code Variations
- Snow loads vary by region
- Wind speeds vary by location
- Permit requirements vary by jurisdiction
- Professional engineer stamp may be required

## Design Margins

### Safety Factors Summary
- **Beam Bending**: Section modulus 97.1 req'd vs 99.8 provided = 2.8% margin
- **Post Compression**: 2.06 safety factor
- **Deflection**: 0.52" actual vs 0.8" limit = 35% margin
- **Fasteners**: All connections have adequate capacity

## Recommendations for Upgrades

### Enhanced Durability
1. Use pressure-treated lumber for posts
2. Galvanized/stainless hardware throughout
3. Proper flashing and drainage details

### Increased Capacity  
1. Upgrade to 2x12 beam for higher snow loads
2. Reduce rafter spacing to 16" OC
3. Add knee braces from posts to beam

### Professional Review
Consider structural engineer review if:
- Local snow loads exceed 30 psf
- Soil conditions are poor
- Existing shed structure is questionable
- Building department requires stamped plans