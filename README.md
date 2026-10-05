<div align="center">
  <img src="https://framerusercontent.com/images/zX3lmokKbWs01tG0gns0ruBgLo.png" alt="Rodrigo Andrade Logo" width="96"/>
</div>

<h1 align="center">LIONv3-Mini Module</h1>

<p align="center">
    <a href="https://github.com/RodrigoCAndrade/LIONv3-Mini"><img alt="Status" src="https://img.shields.io/badge/Status-In Development-050505?style=for-the-badge"></a>
    <a href="https://github.com/RodrigoCAndrade/LIONv3-Mini/releases"><img alt="GitHub Release" src="https://img.shields.io/github/v/release/RodrigoCAndrade/LIONv3-Mini?style=for-the-badge&color=050505&logo=github&logoColor=white"></a>
    <a href="https://github.com/RodrigoCAndrade/LIONv3-Mini/issues"><img alt="GitHub Issues" src="https://img.shields.io/github/issues/RodrigoCAndrade/LIONv3-Mini?style=for-the-badge&color=050505&logo=github&logoColor=white"></a>
    <a href="https://github.com/RodrigoCAndrade/LIONv3-Mini/pulls"><img alt="GitHub Pull Requests" src="https://img.shields.io/github/issues-pr/RodrigoCAndrade/LIONv3-Mini?style=for-the-badge&color=050505&logo=github&logoColor=white"></a>
    <a href="https://github.com/RodrigoCAndrade/LIONv3-Mini/graphs/contributors"><img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/RodrigoCAndrade/LIONv3-Mini?style=for-the-badge&color=050505&logo=github&logoColor=white"></a>
</p>

<br>

<p align="center">
    <img src="mechanics/3d_exports/PCB-Front.png" width="350"><img src="mechanics/3d_exports/PCB-Back.png" width="350">
</p>

## Overview

The LIONv3-Mini is a miniaturized version of the [LIONv3-R](https://github.com/RodrigoCAndrade/LIONv3-Mini), without an onboard LoRa PCB antenna. Built around the ESP32-C6 with 16 MB of external flash, it offers local connectivity over Wi-Fi, Zigbee and Thread, plus LoRa and LR-FHSS for reliable Direct-to-Satellite (DtS) or terrestrial uplinks from remote sites at higher device densities than conventional LoRa. It is a scalable platform for telemetry, global asset tracking and remote sensing.

## Repository Organization

* `docs`: Systems engineering documentation, including schematics, datasheets, requirements (SRD), interface control (ICD) and diagrams.
* `hardware`: Native KiCad project and manufacturing files.
* `mechanics`: 3D models, technical drawings, and physical integration constraints.
* `software`: Embedded firmware and support testing scripts.

## Releases

<table>
  <thead>
    <tr>
      <th>Render</th>
      <th>Hardware Revision</th>
      <th>Status</th>
      <th>Latest Release</th>
      <th>Date</th>
      <th>Datasheet</th>
      <th>BOM</th>
      <th>Manufacturing Info</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><img src="mechanics/3d_exports/PCB-Front.png" alt="board render" width="156"/></td>
      <td>LIONv3-Mini</td>
      <td>🚧 Development</td>
      <td><a href="#">-</a></td>
      <td>05-10-2026</td>
      <td><a href="#">PDF</a></td>
      <td><a href="hardware/Fabrication/BOM-LIONv3.csv">Available</a></td>
      <td><a href="hardware/Fabrication/GERBER-LIONv3.zip">Gerber</a></td>
    </tr>
  </tbody>
</table>

## Fabrication

This board is intended to be fabricated at [JLCPCB](https://jlcpcb.com/). The Gerber files, position files and BOM are available. For complete instructions, see the [Fabrication Guide](hardware/Fabrication/LIONv3-Mini%20Fabrication%20Guide.pdf). Please note that we do not guarantee the board will work, and any manufacturing issues are the user's responsibility. If you find an error or have suggestions for improvement, please do not hesitate to contribute.

## Contributing

We welcome contributions to this project! To ensure a smooth collaboration and maintain our engineering standards, please review our [Contribution Guidelines](CONTRIBUTING.md) before opening any issues, modifying the hardware design, or submitting pull requests.


## References

This board was developed from scratch, but draws on the earlier LIONv1 and LIONv2 designed by [Diego Anestor Coutinho](https://github.com/DIEGOVZK) and [Arielli Ajudarte](https://github.com/ari-aju). The v3 introduces several improvements:

- Dedicated low-power MCU on board
- LR-FHSS support and a more capable LoRa transceiver, covering both sub-GHz and S-band
- External flash for store-and-forward applications
- More compact form factor

<p align="center">
    <img src="docs/LIONv3-Mini-Diagram.png">
</p>

## License

This project utilizes a dual-licensing approach to maximize flexibility and adoption:

* **Hardware:** The hardware designs and schematics are licensed under the permissive **[CERN-OHL-P-2.0](hardware/LICENSE)** open-hardware license. You are entirely free to use, modify, distribute, and commercialize the design without any copyleft obligations to share your derived works under the same terms.
* **Software:** All embedded firmware and utility scripts are licensed under the **[MIT License](software/LICENSE)**. You are free to use, modify, and distribute the code without restriction, provided the original copyright notice and permission notice are included.

## Acknowledgments

This work was carried out at the National Institute of Telecommunications (Inatel) with the support of three research laboratories. The EMBRAPII Inatel Competence Center for 5G and 6G Networks [(xGMobile)](https://inatel.br/xgmobile/) supported this project through its Talent Development Program (PFT xGMobile), alongside the Radio & Communication Laboratory [(RadioCom Lab)](https://inatel.br/radiocomlab/) and the Wireless and Artificial Intelligence Laboratory [(WAI Lab)](https://inatel.br/wailab/). Many thanks to the researchers and staff of all three laboratories for their help and for the infrastructure that made the LIONv3-Mini possible.

<p align="center">
  <img src="https://i.imgur.com/tXnDPkG.png" alt="Funding" width="600"/>
</p>

<p align="center">
  <sub>Built with ❤️ by <a href="https://rodrigoandrade.com">Rodrigo de Carvalho Andrade</a></sub>
</p>
