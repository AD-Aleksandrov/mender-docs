---
title: Debian partition layout
taxonomy:
    category: docs
---

Original layout of partition should be modified to fulfill Mender needs. [Mender conversion scripts](https://github.com/mendersoftware/mender-conversion-tools) provides a tool for modification of partition layout. Restructuring of partition layout should be done as the first step. It can be done by executing the following command:

```bash
        ./mender-conversion-tool.sh make_sdimg --image <output_image_file_name>
                --embedded <file_path_to_original_debian_image>
                --size-data <size_of_partition_data_in_MB> --device-type <beaglebone/raspberrypi3>
```


