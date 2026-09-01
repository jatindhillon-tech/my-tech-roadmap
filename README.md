# my-tech-roadmap
Day 1 — Phase 0 started. Learned: disk → RAM → CPU.
Day 2 — Layer 0: voltage=1/0, binary chosen for noise immunity, silicon doping (N/P type), MOSFET switching (gate field summons electron channel).         corrected: phosphorus→N/boron→P, gate attracts electrons to form channel
Day 3 — Layer 1 expert: gates = MOSFETs pulling wires, propagation delay & critical path set clock speed, NAND/NOR cheaper than AND/OR, built a half-adder (XOR=sum, AND=carry)    corrected: critical path = longest gate-chain sets max clock; sequential logic remembers via feedback
## Layer 1 Practical — Half-Adder  Built a half-adder in CircuitVerse.  SUM = A XOR B  CARRY = A AND B  0 + 0 = 00  0 + 1 = 01  1 + 0 = 01  1 + 1 = 10  The XOR gate calculates the current sum bit.  The AND gate detects whether a carry must be sent to the next binary position.
Day 4 — Layer 2: feedback creates memory. SR latch (set/reset/hold + forbidden state), D latch (enable=freeze), D flip-flop (snapshot on clock edge). 1 FF=1 bit → register → RAM. RAM volatile b/c loop needs power.
## Layer 2 Practical — SR Latch  Built an SR latch from two cross-coupled NOR gates.  S=1, R=0  → Q = 1 (Set)  S=0, R=0  → Q holds (memory!)  S=0, R=1  → Q = 0 (Reset)  S=1, R=1  → forbidden (Q and Qbar both 0)  The cross-coupled feedback is what lets dead gates remember a bit.  This is the atom of all memory: 1 latch = 1 bit.
