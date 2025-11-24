% ---- EXERCÍCIO 3 ----

% A e B têm os mesmos dois progenitores (pai e mãe)
irmaos_germanos(A, B) :-
    progenitor(P1, A), progenitor(P1, B),
    progenitor(P2, A), progenitor(P2, B),
    P1 \= P2,
    A  \= B.
