<!--
    Hey there, I'm Daria Stanilevici!
    Happy to see you here exploring my README code
    Feel free to inspire!
    
    But may I please ask you to follow me in return? Just a click!
    You may also want to connect with me on LinkedIn @daria-stanilevici :))
-->

<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=FF5F05&height=100&section=header" alt="header"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=40&duration=3000&pause=1000&color=FF5F05&center=true&vCenter=true&width=1000&height=100&lines=Hi!+My+name+is+Raghav+%F0%9F%91%8B;I'm+an+Engineering+Student+%40+UIUC;Check+Out+My+Projects+Below+%E2%AC%87%EF%B8%8F)](https://git.io/typing-svg)

## 🔥 Latest Project

### ⚡ HFT FPGA Trading Engine
I designed a **custom 4-layer Artix-7 PCB** and implemented a **10 Gbps market data parser** in SystemVerilog targeting sub-150ns tick-to-trade latency. The full signal chain runs from the SFP+ physical layer through a Xilinx PCS/PMA IP core and 10G Ethernet MAC down to a custom 8-state FSM that parses Ethernet/IPv4/UDP headers and extracts ITCH-inspired trading payload — entirely in silicon, no CPU involved.

**Highlights:**
- Custom PCB designed in Altium: BGA escape routing, 100Ω impedance-controlled SFP+ traces, eFuse protection, QSPI flash, 156.25 MHz LVDS oscillator
- Packet parser FSM in SystemVerilog: validates full Eth/IP/UDP header stack, fires `signal_trigger` with extracted price in deterministic clock cycles
- Clock Domain Crossing architecture: two-stage synchronizers with ASYNC_REG placement, async-assert synchronous-deassert reset pattern
- Self-checking testbench: 10 test cases covering happy path, all DROP conditions, sequence gap detection, and back-to-back packet parsing
- Full PCS/PMA/MAC stack: Xilinx GTX transceiver → XGMII → eth_mac_10g → AXI-Stream → parser

Check out the [repo](https://github.com/RaghavS06/hft-fpga-engine) for RTL, testbench, XDC constraints, and full documentation.

---

<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=FF5F05&height=100&section=footer" alt="footer"/>

<!--
**RaghavS06/RaghavS06** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
