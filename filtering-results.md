
# Filtering and searching

[Cloud-GPUs.com](https://cloud-gpus.com) has flexible filters, as well as full-text search. 

## Filters

Filters are shown on the left-hand-side of the page. On mobile, click "Show Filters" first. 
These allow for selecting specific GPU models, instance specs (total VRAM, CUDA version compatibility),
or individual cloud providers.

For more detailed information about each filter, hover over the info icon next to the filter name. 
### Hardware filters

It's possible to filter the results down to only instances which have:
- A specific GPU model attached (e.g. NVIDIA B200, NVIDIA H100, or AMD MI355X)
- A specific brand of GPU attached (NVIDIA/AMD/Intel/Qualcomm)
- Total GPU memory (VRAM) in a certain range
- Per-GPU memory (VRAM) in a certain range
- An exact number of a certain GPU attached
- GPUs attached which are compatible with a particular CUDA version

For example: 
- [Instances with NVIDIA GPUs across all cloud providers](https://cloud-gpus.com/?brand=NVIDIA)
- [Instances with AMD GPUs across all cloud providers](https://cloud-gpus.com/?brand=AMD)

### Cloud provider filters

It's possible to filter by:
- Cloud providers who have certain compliance certifications (e.g. ISO 27001, SOC 2 Type II, or BSI C5)
- Cloud providers who are NVIDIA Preferred Partners
- Individual cloud providers (e.g. Google Cloud, or Runpod)

### Other filters

Other filters allow for selecting:
- Certain commitment periods, all the way from 1 second to 3 years
- Provisioning models, including on-demand, reserved (i.e. pre-commit to a set period in advance), and spot
- Min/max overall hourly price
- Bare metal vs virtual machines

## Search

In addition to filters, instant search is also available. Just start typing in the search bar at the top, and
matching results will be shown. If any filters are selected, only results which match both the filter and search
criteria will be shown.

## Shareable URLs
 
The page's URL is automatically updated when filters and search terms change, making it easy to bookmark or share
specific views of the data to come back to. 

For example, these are shareable URLs for the following results:
- [On-demand instances with NVIDIA Blackwell GPUs at EU-based providers](https://cloud-gpus.com/?brand=NVIDIA&provisioning=On-demand&reg=EU&arch=Blackwell)
- [Spot instances with GPUs that are compatible with CUDA 12.8/12.9](https://cloud-gpus.com/?provisioning=Spot%2FInterruptible&cuda=12.8-12.9)
- [On-demand or spot instances with at least 128GB VRAM, including P2P marketplaces](https://cloud-gpus.com/?provisioning=On-demand%2CSpot%2FInterruptible&vram__lower=128&p2p=No)

## Defaults

Some filters are applied by default, to exclude the following:
- Peer-to-peer marketplace instances
- Older GPU architectures (Turing, Volta, CDNA2)
- Spot instances
 
To include these in the results:
- Select "Yes" in the "Include P2P" filter
- Select "Older" under "Architecture generation"
- Select "Spot/Interruptible" under "Provisioning"

To go back to the default filters, click "Reset Filters" at the bottom. 
