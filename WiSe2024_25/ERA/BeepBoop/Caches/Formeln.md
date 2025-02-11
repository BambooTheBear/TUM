$\text{CPU Time} =\text{InstructionCount}\cdot \text{avg. Time per Instruction}$
$\text{CPU Time} =\text{InstructionCount}\cdot (\text{avg. Cycle Time per Instruction}+\text{Memory Time})$
$\text{CPU Time} = \text{InstructionCount}\cdot(\frac{\text{avg. Cycles Per Instruction}}{\text{frequency}}+\text{avg. Memory Accesses per Instruction}\cdot\text{avg. Memory access time})$

$\text{avg. Memory access time}=\text{Hit Rate}\cdot\text{Hit Latency}+\text{Miss Rate}\cdot\text{Miss Latency}$
$\text{Miss Penalty}=\text{Hit Latency - Miss Latency}$

# Misses
- Cold Miss ⇒ Daten zum ersten mal im Cache
- Conflict Miss ⇒ Daten waren schon mal im Cache, wurden aber aus einer _Cachezeile_ verdrängt obwohl noch Platz gewesen wäre (in einem _anderen Cacheset_ z.B.)
- Capacity Miss ⇒ Daten waren schon mal im Cache wurden aber aus dem Cache verdrängt, was auch bei einem voll-assoziativen Cache passiert wäre
![[Pasted image 20250211163406.png]]
# Ersetzungsstrategien
Welche Cachezeile tatsächlcih verdrängt wird kann anhand von verschiedenen Startegien entscheiden werden
- Least Recently Used
- Least Frequently Used
- First in first out (primitiver ansatz)
- 