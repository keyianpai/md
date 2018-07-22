# Yao’s garbled circuits

- Represent function as Boolean circuit
- Garbler encrypts circuit’s truth tables with random tokens and sends them to evaluator
- Evaluator can obliviously evaluate circuit using input tokens
# Construction of a Garbled Gate
- Alice picks two random keys for each wire thus she has 6 keys in total
- She encrypts each row of the table, creating the GCT
- She permutes it (rearranges it), so that the key’s position reveals nothing about the value that it is associated with
- She sends it over to Bob, along with her input key $k_x^{b'}$, with $b'$ her input value
- Bob still needs his own key to decrypt the GCT so Alice must send it to him
- If Alice sends both $k_y^0,k_y^1$to Bob, then Bob can decrypt more and if Bob asks for Alice the key that corresponds to his input, then Alice learns Bob’s input
  -  Bob receive his key by using Oblivious Transfer
# Outline of the Protocol

- P1 constructs a garbled circuit
- P1 sends to P2 the keys associated with its inputs
- P1 and P2 use oblivious transfer so that:
  - P2 obtains the key associated with its input on all of its wires
  - P1 learns nothing about P2 inputs  

  P2 computes the circuit and sends the output back to P1
