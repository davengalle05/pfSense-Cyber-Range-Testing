# pfSense – Cyber Range Testing (Kali, Metasploitable, Chronos)

This phase focuses on **testing and validating the network security controls** implemented in previous phases by deploying a cyber range. Offensive and defensive systems are used to confirm firewall rules, VLAN segmentation, and access controls function as intended.

---

## Environments and Technologies Used

- pfSense Firewall
- VirtualBox
- Kali Linux
- Metasploitable
- Chronos
- VLAN Segmentation
- Firewall Rules & Aliases

---

## Operating Systems Used

- Kali Linux
- Metasploitable
- Chronos
- pfSense

---

## OVERVIEW

1. Deploy attacker and vulnerable target machines.
2. Assign systems to appropriate VLANs.
3. Validate DHCP and IP addressing.
4. Test firewall rules and segmentation.
5. Confirm allowed and blocked traffic paths.
6. Simulate basic attack scenarios.

---

## 1. Cyber Range VM Deployment

Deploy the following systems into the lab environment:

- **Kali Linux** – Attacker machine
- **Metasploitable** – Vulnerable target
- **Chronos** – Additional test target

Configure each VM to use the appropriate **Internal Network / VLAN** defined in Phase 2.

---

## 2. Network Assignment and Validation

- Verify each VM receives an IP address from the correct VLAN.
- Confirm default gateway assignment via pfSense.
- Validate DNS resolution where applicable.

---

## 3. Connectivity Testing

Perform connectivity tests to validate firewall behavior.

- Ping tests within the same VLAN.
- Attempt inter-VLAN communication:
  - Confirm blocked traffic where expected.
  - Confirm explicitly allowed traffic functions correctly.
- Test WAN access restrictions.

---

## 4. Attack Simulation and Observation

From **Kali Linux**, perform basic reconnaissance:

- Network discovery scans.
- Service enumeration against Metasploitable and Chronos.
- Observe firewall behavior and logging in pfSense.

No exploitation is performed beyond validation and observation.

---

## 5. Firewall Rule Validation

- Confirm firewall logs reflect blocked traffic.
- Verify alias-based rules function as intended.
- Adjust rules if necessary and re-test.

---

## 6. Final Validation

Confirm the following:

- VLAN segmentation is enforced.
- Firewall rules operate as designed.
- Attacker traffic is restricted appropriately.
- Logging and visibility are maintained.

---

## Conclusion

This phase validates the effectiveness of the **pfSense firewall configuration and network segmentation** by testing real-world attack and traffic scenarios within a controlled cyber range. The completed lab demonstrates practical network security design, implementation, and validation skills applicable to IT Support, Network Administration, and Cybersecurity roles.
