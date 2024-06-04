1⁰)
let rec hanoi debut milieu arrivee n =
  if n > 0 then begin
    hanoi debut arrivee milieu (n - 1);
    deplacement debut arrivee;
    hanoi milieu debut arrivee (n - 1)
  end;;
hanoi "A" "B" "C" 5;;

2⁰)
let rec hanoi_aux debut milieu arrivee n =
  if n > 0 then begin
    hanoi_aux debut arrivee milieu (n - 1);
    deplacement debut arrivee;
    hanoi_aux milieu debut arrivee (n - 1)
  end
let hanoi n =
  hanoi_aux "A" "B" "C" n

3⁰)
let deplacement position1 position2 =
  print_string ("Déplacer le disque de " ^ position1 ^ " vers " ^ position2);
  print_newline ()
let rec hanoi_aux debut milieu arrivee n =
  if n > 0 then begin
    hanoi_aux debut arrivee milieu (n - 1);
    deplacement debut arrivee;
    hanoi_aux milieu debut arrivee (n - 1)
  end
let hanoi n =
  let start_time = Sys.time () in
  hanoi_aux "A" "B" "C" n;
  let end_time = Sys.time () in
  Printf.printf "Temps d'exécution pour n = %d : %f secondes\n" n (end_time -. start_time)
let () = hanoi 10
