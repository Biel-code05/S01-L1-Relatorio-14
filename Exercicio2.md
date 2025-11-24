% ---- EXERCÍCIO 2 ----

% Deus maior: tem pelo menos dois domínios diferentes
% e tem local_principal no olimpo.
deus_maior(Deus) :-
    dominio(Deus, D1),
    dominio(Deus, D2),
    D1 \= D2,
    local_principal(Deus, olimpo).
