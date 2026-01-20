# Delivering Optimal Wireless in the Glass Manufacturing Plant

**A First-Principles Approach to Industrial Wireless Design**

Version 0.1 - January 2026

## Overview

This document provides a comprehensive framework for designing, deploying, and validating wireless networks in glass manufacturing facilities—one of the most hostile RF environments in industry. Rather than relying on generic factory models or vendor promises, this work establishes a first-principles methodology grounded in physics, standards, and empirical validation.

### Why Glass Manufacturing is Different

Glass plants present unique challenges:
- **Extreme thermal environments** (furnaces operating at 1,500°C+)
- **Highly reflective surfaces** (glass sheets, metal rollers, Low-E coatings)
- **Dynamic RF conditions** (moving inventory, conveyors, cranes)
- **Intense electromagnetic interference** (arc furnaces, induction heaters)

Traditional wireless deployment strategies—adding more access points, boosting transmit power, relying on automatic optimization—often fail or prove counterproductive in these environments.

## The Ten First Principles

This framework is built on ten foundational principles:

1. **Wireless Is a Shared, Finite Medium** - Capacity doesn't scale linearly with added devices
2. **The Environment Dominates the Channel** - Physical surroundings matter more than protocol features
3. **Multipath Is the Default State** - Signals arrive via reflected paths, not direct paths
4. **Reliability ≠ Throughput** - High data rates don't guarantee reliable delivery
5. **Mobility Creates Continuous Channel Instability** - Movement transforms static problems into dynamic ones
6. **Much Interference Is Self-Inflicted** - Internal network behavior often dominates interference
7. **Determinism Requires Constraint and Control** - Predictable performance requires limiting variability
8. **Not All Wireless Traffic Is Equal** - Different applications have fundamentally different requirements
9. **Failure Is Inevitable - Resilience Is a Design Choice** - Design for graceful degradation
10. **If It Isn't Measured, It Isn't True** - Continuous measurement validates assumptions

## Key Topics Covered

### Architecture and Design
- **Hybrid wireless architectures** combining Wi-Fi 6/6E/7, private 5G (CBRS), WirelessHART, LoRaWAN, and UWB
- **Segmentation strategies** by use case, mobility, and criticality
- **Constrained RF design** using directional antennas, deliberate low-power operation, and fixed channels
- **Spectrum discipline** with static channel planning and traffic prioritization

### Technologies
- **Private 5G/URLLC** for high-mobility automation and mission-critical control
- **Wi-Fi 6E/7** for high-throughput human interfaces and best-effort traffic
- **Deterministic protocols** (IEEE 802.15.4e TSCH, IETF DetNet/RAW)
- **Time-Sensitive Networking (TSN)** integration

### Security
- **Zero-trust identity** for all devices
- **Network slicing** as security boundaries
- **Encryption requirements** (link-layer and application-layer)
- **Management plane isolation**
- **Continuous security monitoring** correlated with RF performance

### Validation and Metrics
- **IEEE 3388-2025** testing protocols
- **Performance metrics** (PDR, latency, jitter, recovery behavior)
- **Alignment with operational KPIs** (OEE, downtime costs, scrap rates)

## Standards Foundation

This work is grounded in established standards and research:

- **IEEE 3388-2025** - Performance Assessment of Industrial Wireless Systems
- **NIST Technical Note 1951** - Industrial Wireless Systems: Radio Propagation Measurements
- **IETF DetNet/RAW** - Deterministic and Reliable Wireless Networking
- **IEEE 802.11ax/be** - Wi-Fi 6/6E/7 specifications
- **3GPP 5G NR** - Private cellular network standards
- **IEC 62443** - Industrial cybersecurity framework
- **NIST SP 800-82r3** - Guide to Operational Technology Security

## Case Studies

Real-world deployments demonstrating these principles:
- **John Deere** - Private 5G supporting 100+ AGVs across multiple facilities
- **Airbus/Ericsson** - 5G in reflective aerospace assembly environments
- **Celanese Chemical** - CBRS deployment in EMI-heavy process automation
- **US Steel Manufacturer** - Celona 5G LAN in highly reflective metal environments

## Document Structure

1. **Problem Statement** - Why glass manufacturing demands specialized approach
2. **Design Requirements** - Derived from first principles
3. **Architectural Implications** - Hybrid, physics-driven frameworks
4. **Technologies and Architectures** - Specific implementation guidance
5. **Implementation Guidelines** - Phased, risk-mitigated deployment
6. **Performance Validation** - Metrics that matter and success criteria
7. **Conclusion** - Summary and path forward

### Appendices
- **A:** Failure Modes and Anti-Patterns
- **B:** Glossary of Terms
- **C:** References and Research
- **D:** IEEE 3388-2025 Overview
- **E:** Security and Integrity Framework
- **F:** Global 5G Implementation Practices
- **G:** Wi-Fi Spectrum Guide (2.4/5/6 GHz)
- **H:** RF Site Survey Methodology

## Target Audience

- **Industrial wireless architects and engineers**
- **Plant operations and facilities managers**
- **IT/OT convergence teams**
- **Network security professionals**
- **Systems integrators and consultants**
- **Vendor solution architects**

## Key Takeaways

**Wireless reliability in glass manufacturing is not a mystery.** The challenges are well-understood consequences of physics in a hostile environment. By returning to first principles—recognizing wireless as a shared, finite medium shaped by its environment—we can move beyond reactive fixes to intentional designs built on:

- Segmentation
- Constrained RF planning
- Traffic discipline
- Continuous empirical validation

When designed from first principles, wireless becomes a **predictable, scalable enabler** even under extreme conditions.

## About

**Author:** Casey Fahey (Casey.Fahey@NetGoalie.com)

**Affiliation:** In association with the Toledo Tech Loft

**Version:** 0.1 (Initial Draft)

**Date:** January 2026

## Important Notes

### Standards Are Not Solutions

This document relies heavily on standards from IEEE, IETF, NIST, 3GPP, and IEC because they represent the best available foundation for industrial wireless design. However, **standards are tools, not solutions**.

The performance figures, design parameters, and validation methodologies presented represent:
- **Design targets** derived from standards and research, not guaranteed outcomes
- **Engineering principles** that must be validated through site-specific testing
- **Framework approaches** that require adaptation to each facility's unique conditions

### Validation Is Non-Negotiable

When this document states "target latency <10ms" or "PDR >99.99%," these are specifications from IETF DetNet and NIST factory testbeds—they are what deterministic systems *should* achieve, not what all systems *will* achieve without proper design and validation.

Organizations implementing these designs must validate all performance claims through:
- Site-specific RF surveys
- IEEE 3388-2025 testing protocols
- Empirical measurement during pilot deployment
- Continuous monitoring and correlation analysis

## License

This document is provided for educational and professional use. Please cite appropriately when referencing this work.

## Contributing

Feedback, corrections, and contributions are welcome. This is a living document that will evolve as standards mature and deployment experience grows.

## Citation

**Full Citation:**
Fahey, C. (2025). *Delivering Optimal Wireless in the Glass Manufacturing Plant: A First-Principles Approach*. Toledo Tech Loft. NetGoalie.

---

*"When designed from first principles, wireless becomes a predictable, scalable enabler even under extreme conditions."*
