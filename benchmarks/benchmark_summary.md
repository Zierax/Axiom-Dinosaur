# AXIOM-DINOSAUR v4.0 — Benchmark Report
> Generated: 2026-05-01T00:04:46.428386+00:00  |  Taxa attempted: 58  |  Successful: 58

## Overall Performance

| Metric | Value |
|--------|-------|
| Taxa reconstructed | 58 / 58 |
| Mean TCI | 0.6719 |
| Median mass log-error | 0.2108 |
| Mean speed error % | 34.7% |
| Diet accuracy | 65.5% |
| Mean latency | 27.27 s |
| Full-Paint achieved (TCI≥0.85) | 0 / 58 |

## Accuracy by Clade

| Clade | N | Mean TCI | Median Mass LogErr | Diet Acc% |
|-------|---|----------|-------------------|-----------|
| Theropod | 23 | 0.674 | 0.274 | 43% |
| Sauropod | 11 | 0.691 | 0.178 | 100% |
| Ornithischian | 18 | 0.674 | 0.113 | 67% |
| Pterosaur | 6 | 0.622 | 1.368 | 83% |

## Per-Taxon Results

| Taxon | Clade | Mass Pred (kg) | Mass Lit (kg) | LogErr | TCI | Diet | Speed (km/h) | Latency (s) |
|-------|-------|----------------|---------------|--------|-----|------|--------------|-------------|
| Triceratops | Ornithischian | 8248 | 12000 | 0.163 | 0.641 | hypercarnivo ✗ | 17.1 | 34.1 |
| Styracosaurus | Ornithischian | 2932 | 2700 | 0.036 | 0.679 | hypercarnivo ✗ | 13.4 | 33.7 |
| Centrosaurus | Ornithischian | 2932 | 2200 | 0.125 | 0.679 | hypercarnivo ✗ | 13.4 | 42.8 |
| Pachyrhinosaurus | Ornithischian | 2932 | 3000 | 0.010 | 0.679 | hypercarnivo ✗ | 13.4 | 45.2 |
| Ankylosaurus | Ornithischian | 5778 | 6000 | 0.016 | 0.697 | herbivore ✓ | 11.6 | 36.3 |
| Euoplocephalus | Ornithischian | 5778 | 2000 | 0.461 | 0.697 | herbivore ✓ | 11.6 | 35.7 |
| Edmontonia | Ornithischian | 5778 | 3000 | 0.285 | 0.697 | herbivore ✓ | 11.6 | 34.9 |
| Stegosaurus | Ornithischian | 3577 | 3000 | 0.076 | 0.661 | herbivore ✓ | 13.8 | 32.3 |
| Kentrosaurus | Ornithischian | 3577 | 750 | 0.678 | 0.661 | herbivore ✓ | 13.8 | 34.8 |
| Edmontosaurus | Ornithischian | 3791 | 4000 | 0.023 | 0.670 | herbivore ✓ | 14.3 | 35.8 |
| Parasaurolophus | Ornithischian | 3791 | 3000 | 0.102 | 0.670 | herbivore ✓ | 14.3 | 44.2 |
| Corythosaurus | Ornithischian | 3791 | 4000 | 0.023 | 0.670 | herbivore ✓ | 14.3 | 42.1 |
| Iguanodon | Ornithischian | 3641 | 3000 | 0.084 | 0.692 | herbivore ✓ | 14.2 | 32.6 |
| Maiasaura | Ornithischian | 3791 | 3000 | 0.102 | 0.670 | herbivore ✓ | 14.3 | 34.1 |
| Pachycephalosaurus | Ornithischian | 807 | 450 | 0.254 | 0.685 | hypercarnivo ✗ | 10.3 | 26.8 |
| Stygimoloch | Ornithischian | 807 | 200 | 0.606 | 0.685 | hypercarnivo ✗ | 10.3 | 38.9 |
| Psittacosaurus | Ornithischian | 3819 | 20 | 2.281 | 0.646 | herbivore ✓ | 14.6 | 31.2 |
| Protoceratops | Ornithischian | 3819 | 180 | 1.327 | 0.646 | herbivore ✓ | 14.6 | 37.9 |
| Quetzalcoatlus | Pterosaur | 219 | 225 | 0.012 | 0.633 | piscivore ✓ | 5.5 | 45.3 |
| Pteranodon | Pterosaur | 30 | 35 | 0.061 | 0.623 | piscivore ✓ | 4.1 | 39.1 |
| Rhamphorhynchus | Pterosaur | 233 | 0 | 2.669 | 0.619 | piscivore ✓ | 5.5 | 32.6 |
| Pterodactylus | Pterosaur | 233 | 1 | 2.368 | 0.619 | piscivore ✓ | 5.5 | 29.5 |
| Anhanguera | Pterosaur | 233 | 20 | 1.067 | 0.619 | piscivore ✓ | 5.5 | 33.9 |
| Tapejara | Pterosaur | 233 | 5 | 1.669 | 0.619 | piscivore ✗ | 5.5 | 33.2 |
| Diplodocus | Sauropod | 7965 | 12000 | 0.178 | 0.700 | herbivore ✓ | 11.9 | 17.1 |
| Brachiosaurus | Sauropod | 48781 | 35000 | 0.144 | 0.619 | herbivore ✓ | 15.5 | 17.3 |
| Giraffatitan | Sauropod | 48781 | 34000 | 0.157 | 0.619 | herbivore ✓ | 15.5 | 17.2 |
| Argentinosaurus | Sauropod | 10214 | 80000 | 0.894 | 0.709 | herbivore ✓ | 12.8 | 21.3 |
| Apatosaurus | Sauropod | 7965 | 22000 | 0.441 | 0.700 | herbivore ✓ | 11.9 | 22.8 |
| Camarasaurus | Sauropod | 10214 | 20000 | 0.292 | 0.709 | herbivore ✓ | 12.8 | 42.0 |
| Saltasaurus | Sauropod | 10214 | 7000 | 0.164 | 0.709 | herbivore ✓ | 12.8 | 42.8 |
| Rapetosaurus | Sauropod | 10214 | 8000 | 0.106 | 0.709 | herbivore ✓ | 12.8 | 38.5 |
| Aegyptosaurus | Sauropod | 10214 | 10000 | 0.009 | 0.709 | herbivore ✓ | 12.8 | 36.1 |
| Mamenchisaurus | Sauropod | 10214 | 22000 | 0.333 | 0.709 | herbivore ✓ | 12.8 | 35.0 |
| Nigersaurus | Sauropod | 10214 | 4000 | 0.407 | 0.709 | herbivore ✓ | 12.8 | 32.2 |
| Tyrannosaurus | Theropod | 5729 | 7000 | 0.087 | 0.629 | hypercarnivo ✓ | 20.0 | 13.6 |
| Tarbosaurus | Theropod | 3603 | 5000 | 0.142 | 0.643 | hypercarnivo ✓ | 16.8 | 13.6 |
| Gorgosaurus | Theropod | 3603 | 2500 | 0.159 | 0.643 | hypercarnivo ✓ | 16.8 | 12.8 |
| Allosaurus | Theropod | 2160 | 2000 | 0.033 | 0.695 | hypercarnivo ✓ | 16.5 | 12.8 |
| Giganotosaurus | Theropod | 6829 | 7000 | 0.011 | 0.686 | hypercarnivo ✓ | 21.0 | 13.9 |
| Spinosaurus | Theropod | 2979 | 7000 | 0.371 | 0.684 | hypercarnivo ✗ | 15.2 | 15.4 |
| Baryonyx | Theropod | 2979 | 1700 | 0.244 | 0.684 | hypercarnivo ✗ | 15.2 | 18.6 |
| Carnotaurus | Theropod | 2289 | 2000 | 0.059 | 0.685 | herbivore ✗ | 17.1 | 20.2 |
| Dilophosaurus | Theropod | 3603 | 400 | 0.955 | 0.643 | hypercarnivo ✗ | 16.8 | 19.3 |
| Ceratosaurus | Theropod | 2289 | 700 | 0.514 | 0.685 | herbivore ✗ | 17.1 | 25.3 |
| Velociraptor | Theropod | 40 | 15 | 0.425 | 0.738 | hypercarnivo ✗ | 9.0 | 17.9 |
| Deinonychus | Theropod | 40 | 75 | 0.274 | 0.738 | hypercarnivo ✗ | 9.0 | 16.8 |
| Microraptor | Theropod | 40 | 1 | 1.601 | 0.738 | hypercarnivo ✗ | 9.0 | 18.2 |
| Utahraptor | Theropod | 3603 | 500 | 0.858 | 0.643 | hypercarnivo ✗ | 16.8 | 20.6 |
| Gallimimus | Theropod | 343 | 440 | 0.108 | 0.659 | herbivore ✓ | 12.9 | 16.3 |
| Ornithomimus | Theropod | 343 | 170 | 0.305 | 0.659 | herbivore ✓ | 12.9 | 16.2 |
| Oviraptor | Theropod | 139 | 35 | 0.598 | 0.766 | hypercarnivo ✗ | 9.6 | 18.4 |
| Struthiomimus | Theropod | 343 | 150 | 0.359 | 0.659 | herbivore ✓ | 12.9 | 21.8 |
| Therizinosaurus | Theropod | 4836 | 4500 | 0.031 | 0.630 | herbivore ✓ | 17.1 | 16.0 |
| Deinocheirus | Theropod | 6382 | 6350 | 0.002 | 0.647 | hypercarnivo ✗ | 16.3 | 16.2 |
| Compsognathus | Theropod | 2 | 1 | 0.380 | 0.658 | hypercarnivo ✗ | 4.6 | 15.3 |
| Archaeopteryx | Theropod | 0 | 0 | 0.000 | 0.658 | insectivore ✓ | 3.6 | 17.0 |
| Troodon | Theropod | 3603 | 50 | 1.858 | 0.643 | hypercarnivo ✗ | 16.8 | 16.2 |

## Invariant Violations (Axiom IX)

_No Axiom IX mass violations detected._

## Failed Taxa

_All taxa reconstructed successfully._

---

*AXIOM-DINOSAUR v4.0 — Deterministic Palaeontological Reconstruction Engine*