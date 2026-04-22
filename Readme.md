# First Pilot Results
## Full Results will be aviliable in 2 days Of 100-500 dinosaurs

<img width="3826" height="1930" alt="image" src="https://github.com/user-attachments/assets/9d850ec3-6122-44b6-8eaa-2e3bfecd903f" />

```
➜  Axiom-Dinosaur python main.py --taxa Edmontosaurus --output-dir Edmontosaurus

[AXIOM INFO] ======================================================================
[AXIOM INFO] AXIOM-DINOSAUR v1.0  |  Truthimatics Full-Paint  |  Edmontosaurus
[AXIOM INFO] ======================================================================
[AXIOM INFO]   State cleared for new run: Edmontosaurus
[AXIOM INFO] Clade: ORNITHISCHIAN
[AXIOM INFO] PBDB query: Edmontosaurus
[AXIOM INFO]   [S1] /specs/list.json?show=meas,elements
[AXIOM INFO]       -> 16 records, 0 with measurements
[AXIOM INFO]   [S2] /specs/list.json (batch spec IDs)
[AXIOM INFO]       -> 16 spec records, 0 with spec_no
[AXIOM INFO]   [S3] /occs/list.json?show=meas
[AXIOM INFO]       -> 84 occurrence records
[AXIOM INFO]   Source=occs  Endpoint=occs/list.json?show=meas  Records=84
[AXIOM INFO]   Parsed=84  Measurable=0  Elements=[]
[AXIOM INFO] Measurable from PBDB: 0
[AXIOM WARNING] PBDB returned 0 measurable fragments (need ≥4) — supplementing with canonical literature data
[AXIOM INFO] Layer 1: 17 elements mapped
[AXIOM INFO] Layer 2: biomechanical coupling
[AXIOM INFO]   Mass: 4962.3 kg
[AXIOM INFO] Layer 3: deterministic collapse
[AXIOM INFO] Volumetric alpha-shape + voxelization synthesis
[AXIOM INFO]   Alpha-shape volume: 17.486 m³  |  Volumetric mass: 18535.0 kg  (vs regression: 4962.3 kg, delta=273.5%)
[AXIOM INFO]   Voxelizing 8936-point cloud...
[AXIOM INFO]   Voxels inside hull: 380,229/512,000 | Voxel volume: 17.654 m³ | Compute: 21.7s
[AXIOM INFO]   Consensus volume: 17.570 m³ (alpha-shape + voxel average)
[AXIOM WARNING]   Volumetric mass delta 275% > 200% threshold. Alpha-shape unreliable for 4962 kg taxon. Volume geometry retained for visualisation; regression mass used as authoritative value.
[AXIOM INFO]   Valid=True  Score=1.0000  Elements=25  Inferred=8
[AXIOM INFO]   CoG: [2.378, 1.235, 0.01]
[AXIOM INFO] Running Truthimatics engine
[AXIOM INFO]   Axiom I  (Entropy)       : 0.9495
[AXIOM INFO]   Axiom II (Spectral λ₂=0.229, Sym=100%): 0.4343
[AXIOM INFO]   Axiom III (R²)           : 0.9149
[AXIOM INFO]   Axiom IV (Lomb-Scargle)  : FAP=1.0000  peak=0.000 Hz
[AXIOM INFO]   Axiom V  (TCI)           : 0.7471  partial confidence
[AXIOM INFO] Computing physical properties
[AXIOM INFO]   Speed: 14.6 km/h (trot)  | Bite force: 20133.0 N  | Body length: 5.78 m
[AXIOM INFO] Generating outputs
[AXIOM INFO]   Stress chart -> Edmontosaurus/_tmp/stress.png
[AXIOM INFO]   Allometric chart -> Edmontosaurus/_tmp/allom.png
[AXIOM INFO]   TCI chart -> Edmontosaurus/_tmp/tci.png
[AXIOM INFO]   Skin tension -> Edmontosaurus/_tmp/heatmap.png
[AXIOM INFO] Generating full-paint soft tissue synthesis
[AXIOM INFO]   Full-paint PNG -> Edmontosaurus/full_paint.png
[AXIOM INFO]   3D skeleton  -> Edmontosaurus/skeleton_3d.html
[AXIOM INFO]   PDF report   -> Edmontosaurus/reconstruction_report.pdf
[AXIOM INFO]   Truth file   -> Edmontosaurus/truth_file.json
[AXIOM INFO]   Allometric CSV -> Edmontosaurus/allometric_data.csv
[AXIOM INFO] ======================================================================
[AXIOM INFO] Complete in 44987 ms  | TCI=0.7471  | partial
[AXIOM INFO] Output -> /mnt/c/Users/dell/Desktop/Axiom-Dinosaur/Edmontosaurus/
[AXIOM INFO] ======================================================================

=================================================================
  AXIOM-DINOSAUR v4.0   TRUTH FILE SUMMARY
=================================================================
  Specimen ID   : AXIOM_2E97D9C5EB
  Taxa          : Edmontosaurus
  Clade         : Ornithischian
  PBDB records  : 84
  Integrity     : 68.0% Measured / 32.0% Inferred
  Mass (regr.)  : 4962.3 kg
  Mass (vol.)   : 18624.2 kg  (delta 275.3%)
  Volume        : 17.57 m³
  Valid         : True  (score 1.0000)
  TCI           : 0.7471  (partial)
  Axiom I       : 0.9495  (entropy)
  Axiom II      : λ₂=0.229  sym=100%
  Axiom III     : R²=0.9149
  Axiom IV      : FAP=1.0000  peak=0.000 Hz
  CoG (m)       : [2.3781, 1.2352, 0.0101]
  Latency       : 44987.36 ms
-----------------------------------------------------------------
```

```json

{
  "specimen_id": "AXIOM_2E97D9C5EB",
  "taxa": "Edmontosaurus",
  "clade": "ornithischian",
  "physical_properties": {
    "locomotion": {
      "hip_height_m": 2.35,
      "stride_length_m": 4.875,
      "estimated_speed_ms": 4.06,
      "estimated_speed_kmh": 14.6,
      "froude_number": 0.715,
      "gait": "trot",
      "speed_method": "Alexander (1976) / Thulborn (1990)"
    },
    "jaw_feeding": {
      "skull_length_mm": 900.0,
      "skull_height_mm": 400.0,
      "bite_force_N": 20133.0,
      "bite_force_kgf": 2052.3,
      "method": "Christiansen & Wroe (2007)"
    },
    "limb_biomechanics": {
      "femoral_robusticity_index": 0.389,
      "limb_strength_index": 3.3e-05
    },
    "body_geometry": {
      "body_length_est_m": 5.78,
      "neck_length_est_m": 1.05,
      "tail_length_est_m": 2.62
    }
  },
  "pbdb_record_count": 84,
  "skeletal_integrity": "68.0% Measured / 32.0% Inferred",
  "total_bones_in_model": 25,
  "incalculable_bones": [],
  "biomechanical_validity": 1.0,
  "biomech_valid": true,
  "mass_prediction_kg": 4962.3,
  "mass_volumetric_kg": 18624.2,
  "body_volume_m3": 17.57,
  "bio_density_kg_m3": 1060.0,
  "center_of_gravity_m": [
    2.3781,
    1.2352,
    0.0101
  ],
  "truthimatics": {
    "axiom_I_entropy": 0.9495,
    "axiom_II_spectral_gap": 0.229,
    "axiom_II_symmetry_pct": 100.0,
    "axiom_III_r2": 0.9149,
    "axiom_IV_lomb_fap": 1.0,
    "axiom_IV_peak_hz": 0.0,
    "tci": 0.7471,
    "full_paint": false
  },
  "bone_manifest": {
    "coracoid": {
      "length_mm": 200.0,
      "diameter_mm": 140.0,
      "slenderness": 1.429,
      "volume_cm3": 1570.17,
      "estimated_mass_g": 2356.8,
      "centroid_m": [
        2.1,
        1.2075,
        0.2363
      ],
      "feature_int16": [
        1638,
        2293,
        1170,
        1028,
        386
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 15.0,
      "stress": {
        "sigma_axial_MPa": 1.55,
        "sigma_bending_MPa": 2.973,
        "sigma_total_MPa": 4.523,
        "safety_factor": 15.0,
        "status": "OK"
      }
    },
    "femur": {
      "length_mm": 1050.0,
      "diameter_mm": 130.0,
      "slenderness": 8.077,
      "volume_cm3": 7107.81,
      "estimated_mass_g": 10668.8,
      "centroid_m": [
        0.1313,
        0.735,
        0.3255
      ],
      "feature_int16": [
        8601,
        2129,
        6616,
        4658,
        1747
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 7.985,
      "stress": {
        "sigma_axial_MPa": 1.798,
        "sigma_bending_MPa": 19.491,
        "sigma_total_MPa": 21.289,
        "safety_factor": 7.985,
        "status": "OK"
      }
    },
    "femur_right": {
      "length_mm": 1050.0,
      "diameter_mm": 130.0,
      "slenderness": 8.077,
      "volume_cm3": 7107.81,
      "estimated_mass_g": 10668.8,
      "centroid_m": [
        0.1313,
        0.735,
        -0.3255
      ],
      "feature_int16": [
        8601,
        2129,
        6616,
        4658,
        1747
      ],
      "infer_method": "symmetry",
      "confidence": 0.836,
      "safety_factor": 7.985
    },
    "fibula": {
      "length_mm": 880.0,
      "diameter_mm": 40.0,
      "slenderness": 22.0,
      "volume_cm3": 563.98,
      "estimated_mass_g": 846.5,
      "centroid_m": [
        0.1313,
        -0.2625,
        0.3307
      ],
      "feature_int16": [
        7208,
        655,
        18021,
        369,
        138
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 0.293,
      "stress": {
        "sigma_axial_MPa": 18.99,
        "sigma_bending_MPa": 560.766,
        "sigma_total_MPa": 579.756,
        "safety_factor": 0.293,
        "status": "CRITICAL"
      }
    },
    "fibula_right": {
      "length_mm": 880.0,
      "diameter_mm": 40.0,
      "slenderness": 22.0,
      "volume_cm3": 563.98,
      "estimated_mass_g": 846.5,
      "centroid_m": [
        0.1313,
        -0.2625,
        -0.3307
      ],
      "feature_int16": [
        7208,
        655,
        18021,
        369,
        138
      ],
      "infer_method": "symmetry",
      "confidence": 0.836,
      "safety_factor": 0.293
    },
    "humerus": {
      "length_mm": 600.0,
      "diameter_mm": 85.0,
      "slenderness": 7.059,
      "volume_cm3": 1736.4,
      "estimated_mass_g": 2606.3,
      "centroid_m": [
        2.2575,
        1.0762,
        0.3412
      ],
      "feature_int16": [
        4915,
        1392,
        5782,
        1137,
        427
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 3.859,
      "stress": {
        "sigma_axial_MPa": 4.205,
        "sigma_bending_MPa": 39.845,
        "sigma_total_MPa": 44.05,
        "safety_factor": 3.859,
        "status": "WARNING"
      }
    },
    "humerus_right": {
      "length_mm": 600.0,
      "diameter_mm": 85.0,
      "slenderness": 7.059,
      "volume_cm3": 1736.4,
      "estimated_mass_g": 2606.3,
      "centroid_m": [
        2.2575,
        1.0762,
        -0.3412
      ],
      "feature_int16": [
        4915,
        1392,
        5782,
        1137,
        427
      ],
      "infer_method": "symmetry",
      "confidence": 0.836,
      "safety_factor": 3.859
    },
    "ilium": {
      "length_mm": 700.0,
      "diameter_mm": 140.0,
      "slenderness": 5.0,
      "volume_cm3": 5495.59,
      "estimated_mass_g": 8248.9,
      "centroid_m": [
        0.105,
        1.47,
        0.2625
      ],
      "feature_int16": [
        5734,
        2293,
        4095,
        3601,
        1351
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 14.221,
      "stress": {
        "sigma_axial_MPa": 1.55,
        "sigma_bending_MPa": 10.404,
        "sigma_total_MPa": 11.954,
        "safety_factor": 14.221,
        "status": "OK"
      }
    },
    "ilium_right": {
      "length_mm": 700.0,
      "diameter_mm": 140.0,
      "slenderness": 5.0,
      "volume_cm3": 5495.59,
      "estimated_mass_g": 8248.9,
      "centroid_m": [
        0.105,
        1.47,
        -0.2625
      ],
      "feature_int16": [
        5734,
        2293,
        4095,
        3601,
        1351
      ],
      "infer_method": "symmetry",
      "confidence": 0.836,
      "safety_factor": 14.221
    },
    "ischium": {
      "length_mm": 520.0,
      "diameter_mm": 90.0,
      "slenderness": 5.778,
      "volume_cm3": 1687.13,
      "estimated_mass_g": 2532.4,
      "centroid_m": [
        -0.0525,
        1.2075,
        0.231
      ],
      "feature_int16": [
        4259,
        1474,
        4733,
        1105,
        414
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 5.176,
      "stress": {
        "sigma_axial_MPa": 3.751,
        "sigma_bending_MPa": 29.091,
        "sigma_total_MPa": 32.842,
        "safety_factor": 5.176,
        "status": "OK"
      }
    },
    "metacarpal": {
      "length_mm": 150.0,
      "diameter_mm": 35.0,
      "slenderness": 4.286,
      "volume_cm3": 73.6,
      "estimated_mass_g": 110.5,
      "centroid_m": [
        2.3782,
        0.4883,
        0.4042
      ],
      "feature_int16": [
        1228,
        573,
        3510,
        48,
        18
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 1.015,
      "stress": {
        "sigma_axial_MPa": 24.803,
        "sigma_bending_MPa": 142.681,
        "sigma_total_MPa": 167.484,
        "safety_factor": 1.015,
        "status": "CRITICAL"
      }
    },
    "metatarsal": {
      "length_mm": 400.0,
      "diameter_mm": 55.0,
      "slenderness": 7.273,
      "volume_cm3": 484.67,
      "estimated_mass_g": 727.5,
      "centroid_m": [
        0.2363,
        -0.8925,
        0.2835
      ],
      "feature_int16": [
        3276,
        901,
        5957,
        317,
        119
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 1.573,
      "stress": {
        "sigma_axial_MPa": 10.044,
        "sigma_bending_MPa": 98.051,
        "sigma_total_MPa": 108.095,
        "safety_factor": 1.573,
        "status": "CRITICAL"
      }
    },
    "phalanx": {
      "length_mm": 90.0,
      "diameter_mm": 28.0,
      "slenderness": 3.214,
      "volume_cm3": 28.26,
      "estimated_mass_g": 42.4,
      "centroid_m": [
        2.4465,
        0.3465,
        0.4148
      ],
      "feature_int16": [
        737,
        458,
        2633,
        18,
        6
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 0.825,
      "stress": {
        "sigma_axial_MPa": 38.754,
        "sigma_bending_MPa": 167.204,
        "sigma_total_MPa": 205.959,
        "safety_factor": 0.825,
        "status": "CRITICAL"
      }
    },
    "pubis": {
      "length_mm": 480.0,
      "diameter_mm": 70.0,
      "slenderness": 6.857,
      "volume_cm3": 942.1,
      "estimated_mass_g": 1414.1,
      "centroid_m": [
        0.105,
        1.155,
        0.231
      ],
      "feature_int16": [
        3932,
        1146,
        5617,
        617,
        231
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 2.687,
      "stress": {
        "sigma_axial_MPa": 6.201,
        "sigma_bending_MPa": 57.072,
        "sigma_total_MPa": 63.273,
        "safety_factor": 2.687,
        "status": "WARNING"
      }
    },
    "radius": {
      "length_mm": 460.0,
      "diameter_mm": 50.0,
      "slenderness": 9.2,
      "volume_cm3": 460.64,
      "estimated_mass_g": 691.4,
      "centroid_m": [
        2.3363,
        0.735,
        0.3832
      ],
      "feature_int16": [
        3768,
        819,
        7536,
        301,
        113
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 1.048,
      "stress": {
        "sigma_axial_MPa": 12.153,
        "sigma_bending_MPa": 150.081,
        "sigma_total_MPa": 162.235,
        "safety_factor": 1.048,
        "status": "CRITICAL"
      }
    },
    "radius_right": {
      "length_mm": 460.0,
      "diameter_mm": 50.0,
      "slenderness": 9.2,
      "volume_cm3": 460.64,
      "estimated_mass_g": 691.4,
      "centroid_m": [
        2.3363,
        0.735,
        -0.3832
      ],
      "feature_int16": [
        3768,
        819,
        7536,
        301,
        113
      ],
      "infer_method": "symmetry",
      "confidence": 0.836,
      "safety_factor": 1.048
    },
    "rib": {
      "length_mm": 700.0,
      "diameter_mm": 35.0,
      "slenderness": 20.0,
      "volume_cm3": 343.47,
      "estimated_mass_g": 515.6,
      "centroid_m": [
        1.26,
        1.1288,
        0.2625
      ],
      "feature_int16": [
        5734,
        573,
        16383,
        225,
        84
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 0.246,
      "stress": {
        "sigma_axial_MPa": 24.803,
        "sigma_bending_MPa": 665.845,
        "sigma_total_MPa": 690.647,
        "safety_factor": 0.246,
        "status": "CRITICAL"
      }
    },
    "scapula": {
      "length_mm": 560.0,
      "diameter_mm": 220.0,
      "slenderness": 2.545,
      "volume_cm3": 10856.59,
      "estimated_mass_g": 16295.7,
      "centroid_m": [
        2.0475,
        1.4175,
        0.2625
      ],
      "feature_int16": [
        4587,
        3604,
        2085,
        7114,
        2669
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 15.0,
      "stress": {
        "sigma_axial_MPa": 0.628,
        "sigma_bending_MPa": 2.145,
        "sigma_total_MPa": 2.773,
        "safety_factor": 15.0,
        "status": "OK"
      }
    },
    "scapula_right": {
      "length_mm": 560.0,
      "diameter_mm": 220.0,
      "slenderness": 2.545,
      "volume_cm3": 10856.59,
      "estimated_mass_g": 16295.7,
      "centroid_m": [
        2.0475,
        1.4175,
        -0.2625
      ],
      "feature_int16": [
        4587,
        3604,
        2085,
        7114,
        2669
      ],
      "infer_method": "symmetry",
      "confidence": 0.836,
      "safety_factor": 15.0
    },
    "skull": {
      "length_mm": 900.0,
      "diameter_mm": 400.0,
      "slenderness": 2.25,
      "volume_cm3": 57679.64,
      "estimated_mass_g": 86577.1,
      "centroid_m": [
        3.9375,
        1.47,
        0.0
      ],
      "feature_int16": [
        7372,
        6553,
        1843,
        32767,
        14184
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 15.0,
      "stress": {
        "sigma_axial_MPa": 0.19,
        "sigma_bending_MPa": 0.574,
        "sigma_total_MPa": 0.763,
        "safety_factor": 15.0,
        "status": "OK"
      }
    },
    "tibia": {
      "length_mm": 900.0,
      "diameter_mm": 90.0,
      "slenderness": 10.0,
      "volume_cm3": 2920.03,
      "estimated_mass_g": 4383.0,
      "centroid_m": [
        0.105,
        -0.2625,
        0.315
      ],
      "feature_int16": [
        7372,
        1474,
        8191,
        1913,
        718
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 3.142,
      "stress": {
        "sigma_axial_MPa": 3.751,
        "sigma_bending_MPa": 50.349,
        "sigma_total_MPa": 54.1,
        "safety_factor": 3.142,
        "status": "WARNING"
      }
    },
    "tibia_right": {
      "length_mm": 900.0,
      "diameter_mm": 90.0,
      "slenderness": 10.0,
      "volume_cm3": 2920.03,
      "estimated_mass_g": 4383.0,
      "centroid_m": [
        0.105,
        -0.2625,
        -0.315
      ],
      "feature_int16": [
        7372,
        1474,
        8191,
        1913,
        718
      ],
      "infer_method": "symmetry",
      "confidence": 0.836,
      "safety_factor": 3.142
    },
    "ulna": {
      "length_mm": 480.0,
      "diameter_mm": 52.0,
      "slenderness": 9.231,
      "volume_cm3": 519.89,
      "estimated_mass_g": 780.3,
      "centroid_m": [
        2.3415,
        0.7298,
        0.3885
      ],
      "feature_int16": [
        3932,
        851,
        7561,
        340,
        127
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 1.13,
      "stress": {
        "sigma_axial_MPa": 11.236,
        "sigma_bending_MPa": 139.223,
        "sigma_total_MPa": 150.459,
        "safety_factor": 1.13,
        "status": "CRITICAL"
      }
    },
    "ulna_right": {
      "length_mm": 480.0,
      "diameter_mm": 52.0,
      "slenderness": 9.231,
      "volume_cm3": 519.89,
      "estimated_mass_g": 780.3,
      "centroid_m": [
        2.3415,
        0.7298,
        -0.3885
      ],
      "feature_int16": [
        3932,
        851,
        7561,
        340,
        127
      ],
      "infer_method": "symmetry",
      "confidence": 0.836,
      "safety_factor": 1.13
    },
    "vertebra": {
      "length_mm": 200.0,
      "diameter_mm": 130.0,
      "slenderness": 1.538,
      "volume_cm3": 1353.87,
      "estimated_mass_g": 2032.2,
      "centroid_m": [
        1.3125,
        1.47,
        0.0
      ],
      "feature_int16": [
        1638,
        2129,
        1260,
        887,
        332
      ],
      "infer_method": "measured",
      "confidence": 0.88,
      "safety_factor": 15.0,
      "stress": {
        "sigma_axial_MPa": 1.798,
        "sigma_bending_MPa": 3.713,
        "sigma_total_MPa": 5.51,
        "safety_factor": 15.0,
        "status": "OK"
      }
    }
  },
  "warnings": [],
  "reconstruction_latency_ms": 44987.36
}
```

```csv
element,length_mm,length_predicted_mm,diameter_mm,diameter_predicted_mm,length_residual_pct,body_mass_kg,infer_method,confidence
coracoid,200.0,270.76,140.0,189.53,-26.13,4962.34,measured,0.88
femur,1050.0,1421.48,130.0,175.99,-26.13,4962.34,measured,0.88
femur_right,1050.0,1421.48,130.0,175.99,-26.13,4962.34,symmetry,0.836
fibula,880.0,1191.34,40.0,54.15,-26.13,4962.34,measured,0.88
fibula_right,880.0,1191.34,40.0,54.15,-26.13,4962.34,symmetry,0.836
humerus,600.0,812.28,85.0,115.07,-26.13,4962.34,measured,0.88
humerus_right,600.0,812.28,85.0,115.07,-26.13,4962.34,symmetry,0.836
ilium,700.0,947.65,140.0,189.53,-26.13,4962.34,measured,0.88
ilium_right,700.0,947.65,140.0,189.53,-26.13,4962.34,symmetry,0.836
ischium,520.0,703.97,90.0,121.84,-26.13,4962.34,measured,0.88
metacarpal,150.0,203.07,35.0,47.38,-26.13,4962.34,measured,0.88
metatarsal,400.0,541.52,55.0,74.46,-26.13,4962.34,measured,0.88
phalanx,90.0,121.84,28.0,37.91,-26.13,4962.34,measured,0.88
pubis,480.0,649.82,70.0,94.77,-26.13,4962.34,measured,0.88
radius,460.0,622.74,50.0,67.69,-26.13,4962.34,measured,0.88
radius_right,460.0,622.74,50.0,67.69,-26.13,4962.34,symmetry,0.836
rib,700.0,947.65,35.0,47.38,-26.13,4962.34,measured,0.88
scapula,560.0,758.12,220.0,297.83,-26.13,4962.34,measured,0.88
scapula_right,560.0,758.12,220.0,297.83,-26.13,4962.34,symmetry,0.836
skull,900.0,1218.41,400.0,541.52,-26.13,4962.34,measured,0.88
tibia,900.0,1218.41,90.0,121.84,-26.13,4962.34,measured,0.88
tibia_right,900.0,1218.41,90.0,121.84,-26.13,4962.34,symmetry,0.836
ulna,480.0,649.82,52.0,70.4,-26.13,4962.34,measured,0.88
ulna_right,480.0,649.82,52.0,70.4,-26.13,4962.34,symmetry,0.836
vertebra,200.0,270.76,130.0,175.99,-26.13,4962.34,measured,0.88
```
