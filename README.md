# federated_learning_attack

Privacy attack from the point of view of a malicious server during the usual federated averaging algorithm with secure aggregation.

Basically the server gives a poisoned model to everyone except one targeted participant. The poisoned models leverage dead relus to be in a frozen state, so that the trained models given back by the clients are left unchanged. This allows the malicious server to extract the gradient of the targeted participant.

It might seem obvious but it shows that even under secure aggregation protocol, there is a form of trust that we need to place in the server.
