# wireshark
Here’s a **README.md** file you can use for that Wireshark task:

---

# Wireshark Packet Capture & Protocol Analysis

## Steps to Perform

1. **Install Wireshark**
   Download and install from: [https://www.wireshark.org/download.html](https://www.wireshark.org/download.html)

2. **Start Packet Capture**

   * Open Wireshark.
   * Select your **active network interface** (usually Ethernet or Wi-Fi).
   * Click **Start Capturing Packets**.

3. **Generate Network Traffic**

   * Open a browser and visit a website **OR** run:

     ```bash
     ping google.com
     ```
   * This will generate traffic for capture.

4. **Stop Capture**

   * After 1 minute, click the **red stop button** in Wireshark.

5. **Filter by Protocol**

   * In the Wireshark filter bar, enter:

     * `http` → to view HTTP packets
     * `dns` → to view DNS packets
     * `tcp` → to view TCP packets

6. **Identify Protocols**

   * Note at least 3 different protocols from the capture (e.g., HTTP, DNS, ARP, TCP, ICMP).

7. **Export Capture**

   * Go to **File → Save As**.
   * Save the file in `.pcap` format.
   * Example filename: `network_capture.pcap`.

8. **Summarize Findings**

   * Example summary:

     * **HTTP** – 50 packets (browser website requests).
     * **DNS** – 10 packets (domain resolution).
     * **TCP** – 100 packets (underlying transport).
   * Include packet details like source IP, destination IP, ports, and packet length.

---

## Example Output

**Protocols Found:**

1. HTTP – Source: 192.168.1.5 → Destination: 142.250.183.238 (google.com)
2. DNS – Source: 192.168.1.5 → Destination: 8.8.8.8
3. TCP – Multiple connections with SYN, ACK flags

---
