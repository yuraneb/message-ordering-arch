# Message ordering Architecture design proposals

This repo showcases some possible solutions I have for enforcing message ordering. These are mostly fairly standard approaches, adapted to the simple scenario where we care about events (carrying an ID and an arbitrary payload) being updated/inserted strictly in the order that they arrive into a distributed system (e.g. any instance of a microservice). These are mostly high-level designs with minimal required detail. If I have time, I will include minimal implementations for some of them.

## Errata

In solution ASYNC1, I'm referring to the "STATUS" table, which I actually labeled "EVENTS" in the diagram. Please be aware these refer to the same table.
In the diagram for solution ASYNC2, Partition2 of the Kafka topic has been lableled "Partition1". 
I will leave these errata notes in the readme until I have a chance to correct the writeups/diagrams.
