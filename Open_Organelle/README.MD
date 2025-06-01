<h1 align="center">Open Organelle – Mouse Nucleus accumbens</h1>

This folder documents the Mouse nucleus accumbens dataset hosted at Janelia's Open Organelle data portal. This is a large-scale 3D electron microscopy (EM) dataset of the nucleus accumbens region in an adult mouse brain acquired using an enhanced focused ion beam scanning electron microscopy (FIB-SEM) technology developed at Janelia.

## Dataset Overview

- **Source:** [OpenOrganelle – jrc_mus-nacc-2](https://openorganelle.janelia.org/datasets/jrc_mus-nacc-2)
- **Sample:** Nucleus accumbens from a wild-type, adult male mouse, strain: C57/BL6J from Charles River.
- **Dataset Location:** s3://janelia-cosem-datasets/jrc_mus-nacc-2/
- **Data Format:** Multi-resolution volumetric data (zarr format)

<details>
<summary>Click to view the data tree structure</summary>

```text
/
└── recon-2
    ├── em
    │   └── fibsem-int16
    │        ├── s0 (564, 2520, 2596) int16
    │        ├── s1 (282, 1260, 1298) int16
    │        ├── s2 (141, 630, 649) int16
    │        ├── s3 (70, 315, 324) int16
    │        ├── s4 (35, 157, 162) int16
    │        ├── s5 (17, 78, 81) int16
    │        ├── s6 (8, 39, 40) int16
    │        ├── s7 (4, 19, 20) int16
    │        └── s8 (2, 9, 10) int16
    └── labels
        └── inference
            └── segmentations
                └── nuc
                    ├── s0 (70, 315, 324) uint8
                    ├── s1 (35, 157, 162) uint8
                    └── s2 (17, 78, 81) uint8
```
</details> 


### Metadata: EM Image Data
| Resolution   | Voxel size (z, y, x)[nm]            | Translation (z, y, x)[nm]      |
|:-------------|:------------------------------------|:-------------------------------|
| s0           | [2.96, 4.0, 4.0]                    | [0.0, 0.0, 0.0]                |
| s1           | [5.92, 8.0, 8.0]                    | [1.48, 2.0, 2.0]               |
| s2           | [11.840000000000002, 16.0, 16.0]    | [4.4399999999999995, 6.0, 6.0] |
| s3           | [23.68, 32.0, 32.0]                 | [10.36, 14.0, 14.0]            |
| s4           | [47.36, 64.0, 64.0]                 | [22.2, 30.0, 30.0]             |
| s5           | [94.72, 128.0, 128.0]               | [45.88, 62.0, 62.0]            |
| s6           | [189.44, 256.0, 256.0]              | [93.24, 126.0, 126.0]          |
| s7           | [378.8799999999999, 512.0, 512.0]   | [187.96, 254.0, 254.0]         |
| s8           | [757.7599999999999, 1024.0, 1024.0] | [377.4, 510.0, 510.0]          |

### Metadata: Segmentation Labels
| Resolution   | Voxel size (z, y, x)[nm]   | Translation (z, y, x)[nm]        |
|:-------------|:---------------------------|:---------------------------------|
| s0           | [23.68, 32.0, 32.0]        | [10.36, 14.0, 14.0]              |
| s1           | [47.36, 64.0, 64.0]        | [22.2, 30.0, 30.0]               |
| s2           | [94.72, 128.0, 128.0]      | [45.879999999999995, 62.0, 62.0] |
