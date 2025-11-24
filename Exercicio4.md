% ---- EXERCÍCIO 4 ----

% Caso base: A é progenitor direto de D
ancestral(A, D) :-
    progenitor(A, D).

% Passo recursivo: A é progenitor de um intermediário Z,
% e Z é ancestral de D
ancestral(A, D) :-
    progenitor(A, Z),
    ancestral(Z, D).
