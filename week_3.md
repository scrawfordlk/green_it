(Definitely rewatch this)
# Week 3 - 
## Side Channel
  - = obtaining metadata
  j
## Attack via Cache
  - through shared memory you also share cache
  - the attacker can flush the memory to empty the cache. Now the attacker can verify if the victim has accessed some data if the attacker's access is fast (cache hit), because the victim got a cache miss.
## other attack
  - if memory location of important kernel atvtivies are known, then you can monitor them (?)
## Hammering
  - through accesses of rows, other rows may be affected (bitflips)
    + bitflips can lead to a different opcode, e.g. changing a beq to bne
## Alternatives to security (dont know how serious)
  + No security -> Just pay the damages for every issue

- Runtime Overhead largely correlates with energy overhead, but not always. Sometimes
  there is a high runtime overhead with the unchangin energy costs or high energy costs for
  the same runtime overhead

## Is it possible to increase efficiency by adding security?
  + counterintuitive at first, but
    - SMTCache is more energy-efficient, performant and secure
  + does undervolting increase or decrease performance?
    - turns out undervolting increases performance actuallysame 
