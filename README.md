# Blender-Render-Bench

# Getting Started
`>>> ./benchmark-launcher-cli authenticate`

# Next you need to determine which Blender version and which scenes you want to
# benchmark:
`>>> ./benchmark-launcher-cli blender list`

# Next we need to download the Blender versions and the required scenes:
`>>> ./benchmark-launcher-cli blender download 2.81a`
`>>> ./benchmark-launcher-cli scenes download --blender-version 2.81a bmw27`

# We also need to decide on which device to run the benchmark:
`>>> ./benchmark-launcher-cli devices --blender-version 2.81a`
### The first column is the device name.
### The second column is the device type.

# Run the benchmark:
`>>> ./benchmark-launcher-cli benchmark --blender-version 2.81a --device-type CPU --json --submit bmw27
[
  {
    "timestamp": "2020-01-15T14:07:44.254378+00:00",
    "blender_version": {
      "version": "2.81 (sub 16)",
      "build_date": "2019-12-04",
      "build_time": "13:48:07",
      "build_commit_date": "2019-12-04",
      "build_commit_time": "11:32",
      "build_hash": "f1aa4d18d49d",
      "label": "2.81a",
      "checksum": "08d718505d1eb1d261efba96b0787220a76d357ce5b94aca108fc9e0c339d6c6"
    },
    "benchmark_launcher": {
      "label": "2.0.4",
      "checksum": "37c9687e041fa0a94a89914618f80d5213a556bba3822c58c09086e9c8d48944"
    },
    "benchmark_script": {
      "label": "2.0.0",
      "checksum": "e38921ff7a2959d5e47a83501a2dde3f7f166a4f46b65fac272eec38ae9e5f27"
    },
    "scene": {
      "label": "bmw27",
      "checksum": "bc4fd79cbd85a1cc47926e848ec8f322872f5c170ef33c21e0d0ce303c0ec9ea"
    },
    "system_info": {
      "bitness": "64bit",
      "machine": "x86_64",
      "system": "Linux",
      "dist_name": "Pop!_OS",
      "dist_version": "19.10",
      "devices": [
        {
          "type": "CPU",
          "name": "AMD Ryzen 7 1800X Eight-Core Processor"
        }
      ],
      "num_cpu_sockets": 1,
      "num_cpu_cores": 8,
      "num_cpu_threads": 16
    },
    "device_info": {
      "device_type": "CPU",
      "compute_devices": [
        {
          "type": "CPU",
          "name": "AMD Ryzen 7 1800X Eight-Core Processor"
        }
      ],
      "num_cpu_threads": 16
    },
    "stats": {
      "device_peak_memory": 140.85,
      "total_render_time": 229.737,
      "render_time_no_sync": 228.057
    }
  }
]`
