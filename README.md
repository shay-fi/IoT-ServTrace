# IoT-ServTrace Datasets

This repository contains the service trace data used for our paper published at IFIP Networking 2026 (see 'Cite Our Data' section below). The repository contains two subdirectories corresponding to the **IoT-ServTrace-2019** and **IoT-ServTrace-2022** datasets.

## Directory Structure
```
.
├── IoT-ServTrace-2019/
│   ├── <device_1>.json
│   ├── <device_2>.json
│   └── ...
└── IoT-ServTrace-2022/
    ├── <device_1>.json
    ├── <device_2>.json
    └── ...
```

Each **JSON** file contains traffic data of a single IoT device type.

---

## File Format

Each line in a `.json` file is a JSON object with the following structure:

```json
{
    "flowEndTimestamp": "<UTC timestamp of the flow export, e.g., '2019-06-01 00:01:01.000'>",
    "protocol": "<TCP or UDP>",
    "portNumber": <integer port number, e.g., 80>
}
```

### Field Descriptions
- **flowEndTimestamp**: The timestamp when the flow ended, in human-readable format.
- **protocol**: The transport protocol used by the flow (`TCP` or `UDP`).
- **portNumber**: The port number associated with the flow.

---

## Cite Our Data:
<pre>
@INPROCEEDINGS{26IFIPNetworking,
    author = {Azizi, Shayan and Okui, Norihiro and Nakahara, Masataka and Kubota, Ayumu and Habibi Gharakheili, Hassan},
    booktitle = {Proc. IFIP Networking},
    title = {{Backend-Service Fingerprints: Lightweight and Interpretable Identification of Household IoTs}},
    year = {2026},
    month = {May},
    address = {Lugano, Switzerland}
}

## Related Links:
https://iotanalytics.unsw.edu.au
