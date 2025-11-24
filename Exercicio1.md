% ---- EXERCÍCIO 1 ----

% 1) Hades como filho de Cronos e Reia
progenitor(cronos, hades).
progenitor(reia,   hades).

% 2) Regra: deus filho de Cronos e com domínio céu/mar/submundo
divindade_olimpica(Deus) :-
    progenitor(cronos, Deus),
    dominio(Deus, Dominio),
    ( Dominio = ceu
    ; Dominio = mar
    ; Dominio = submundo
    ).
