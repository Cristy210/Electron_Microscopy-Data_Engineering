<h1 align="center">Nueroglancer – FlyEM Hemibrain </h1>

This folder documents the FlyEM Hemibrain connectome dataset, available in the Neuroglancer [precomputed format](https://github.com/google/neuroglancer/blob/master/src/datasource/precomputed/volume.md#unsharded-chunk-storage). The FlyEM Hemibrain dataset represents the largest synapse-resolution map of brain connectivity, capturing part of the adult Drosophila (fruit fly) brain. Data was downloaded and accessed using the [CloudVolume](https://github.com/seung-lab/cloud-volume) Python package.

## Dataset Overview

- **Source:** [FlyEM Hemibrain](https://tinyurl.com/hemibrain-ng)
- **Sample:** Drosophila melanogaster adult brain, hemibrain region (part of the central brain)
- **Dataset Location:** precomputed://gs://neuroglancer-janelia-flyem-hemibrain/v1.0/segmentation
- **Data Format:** Neuroglancer precomputed volume

### Metadata: Summary

| Field              | Value                          |
|:-------------------|:-------------------------------|
| @type              | neuroglancer_multiscale_volume |
| data_type          | uint64                         |
| num_channels       | 1                              |
| type               | segmentation                   |
| mesh               | mesh                           |
| segment_name_map   | names                          |
| segment_properties | segment_properties             |

### Metadata: Scales(Resolution Levels)

|   Scale | chunk_sizes    | compressed_segmentation_block_size   | encoding                | key                  | resolution         | size                  |
|--------:|:---------------|:-------------------------------------|:------------------------|:---------------------|:-------------------|:----------------------|
|       0 | [[64, 64, 64]] | [8, 8, 8]                            | compressed_segmentation | 8.0x8.0x8.0          | [8, 8, 8]          | [34432, 39552, 41408] |
|       1 | [[64, 64, 64]] | [8, 8, 8]                            | compressed_segmentation | 16.0x16.0x16.0       | [16, 16, 16]       | [17216, 19776, 20704] |
|       2 | [[64, 64, 64]] | [8, 8, 8]                            | compressed_segmentation | 32.0x32.0x32.0       | [32, 32, 32]       | [8608, 9888, 10352]   |
|       3 | [[64, 64, 64]] | [8, 8, 8]                            | compressed_segmentation | 64.0x64.0x64.0       | [64, 64, 64]       | [4304, 4944, 5176]    |
|       4 | [[64, 64, 64]] | [8, 8, 8]                            | compressed_segmentation | 128.0x128.0x128.0    | [128, 128, 128]    | [2152, 2472, 2588]    |
|       5 | [[64, 64, 64]] | [8, 8, 8]                            | compressed_segmentation | 256.0x256.0x256.0    | [256, 256, 256]    | [1076, 1236, 1294]    |
|       6 | [[64, 64, 64]] | [8, 8, 8]                            | compressed_segmentation | 512.0x512.0x512.0    | [512, 512, 512]    | [538, 618, 647]       |
|       7 | [[64, 64, 64]] | [8, 8, 8]                            | compressed_segmentation | 1024.0x1024.0x1024.0 | [1024, 1024, 1024] | [269, 309, 324]       |
|       8 | [[64, 64, 64]] | [8, 8, 8]                            | compressed_segmentation | 2048.0x2048.0x2048.0 | [2048, 2048, 2048] | [135, 155, 162]       |

### Metadata: Scales['Sharding']

|   Scale | @type                          | data_encoding   | hash     |   minishard_bits | minishard_index_encoding   |   preshift_bits |   shard_bits |
|--------:|:-------------------------------|:----------------|:---------|-----------------:|:---------------------------|----------------:|-------------:|
|       0 | neuroglancer_uint64_sharded_v1 | gzip            | identity |                6 | gzip                       |               9 |           15 |
|       1 | neuroglancer_uint64_sharded_v1 | gzip            | identity |                6 | gzip                       |               9 |           12 |
|       2 | neuroglancer_uint64_sharded_v1 | gzip            | identity |                6 | gzip                       |               9 |            9 |
|       3 | neuroglancer_uint64_sharded_v1 | gzip            | identity |                6 | gzip                       |               9 |            6 |
|       4 | neuroglancer_uint64_sharded_v1 | gzip            | identity |                6 | gzip                       |               9 |            3 |
|       5 | neuroglancer_uint64_sharded_v1 | gzip            | identity |                6 | gzip                       |               9 |            0 |
|       6 | neuroglancer_uint64_sharded_v1 | gzip            | identity |                3 | gzip                       |               9 |            0 |
|       7 | neuroglancer_uint64_sharded_v1 | gzip            | identity |                0 | gzip                       |               9 |            0 |
|       8 | neuroglancer_uint64_sharded_v1 | gzip            | identity |                0 | gzip                       |               6 |            0 |