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
`>>> ./benchmark-launcher-cli benchmark --blender-version 2.81a --device-type CPU --json --submit bmw27`
