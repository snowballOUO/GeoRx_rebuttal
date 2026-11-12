# GeoRx rebuttal data
The data cover 9 encoders, 10 workloads, and 3 evaluation seeds. Encoder and workload identifiers follow the paper.
- diagnosis_z_recall.csv (270 rows): One row per encoder × workload × seed, containing the five direction-aligned, standardized deviations from the spherical reference (z_H1 through z_H5) and baseline R@1, R@5, and R@10 for full-corpus cosine retrieval.
- diagnosed_mapped_repairs.csv (816 rows): Each row records a positive diagnosis for a given seed and the result of applying its mapped repair method independently. If multiple channels are positive for the same evaluation unit, each appears in a separate row. H3 has no positive diagnoses.
- all_five_repairs.csv (1350 rows): Each evaluation unit includes results for all five repair methods, each evaluated independently against the same cosine baseline. Records shared with the preceding table have identical values.
The diagnosis-to-repair mappings are H1→CSLS, H2→α-QE, H3→Diffusion, H4→Listwise CE, and H5→Pointwise CE.
