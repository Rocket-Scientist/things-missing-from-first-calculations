#include <stdio.h>
#include <math.h>

float mass payload number_of_boosters inert_mass i thrust centaur_engine_type

float calc_mass_of_payload(mass, payload) {
      printf ("Would you like to have:\n1. short pay load\n2. medium pay load\n3. long pay load\n");
      scanf("%f",&i);
      if (i = 1) payload = 3524;
      if (i = 2) payload = 4003; 
      if (i = 3) payload = 4379;
      return payload;
      }

float decide_number_of_boosters(number_of_boosters) {
      printf ("How many boosters would you like (you can have 0-5): ");
      scanf ("%f", &number_of_boosters);
      return number_of_boosters;
      }

float find_out_what_inert_masses_to_use(inert_mass) {
      printf ("What type of JOECOLEBROOK would you like to use:\n1. 5x1\n2. 5x2\n");
      scanf ("%f", &i);
      if (i = 1) inert_mass = 2247 + 2212; /*common centaur, interstage adapter*/
      if (i = 2) inert_mass = 2462 + 2227; /*common centaur, interstage adapter*/
      return inert_mass;
      }

float calc_mass(mass payload number_of_boosters inert_mass); {
      mass = payload + number_of_boosters * 46697 + inert_mass + 275 + 20830 + 285 + 284089 + 21351; /*payload, boosters, inert mass, common centaur(CFLR, Propellant), Atls booster cylindrical interstage adapter, atlas booster(propellant, inert mass*/
      return mass;
      }

float decide_centaur_engine_type(centaur_engine_type i) {
      printf ("What type of centaur engine would you like to use:\n1. Single engine centaur\n2. Duel engine centaur\n");
      scanf("%f", &i);
      if (i = 1) centaur_engine_type = 99200;
      if (i = 2) centaur_engine_type = 198400;
      return centaur_engine_type;
      }

float thrust_calc(thrust centaur_engine_type i) {
      thrust = centaur_enginer_type + number_of_boosters * 1688400 + 3827000;
      return thrust;
      }

/*for temperature, i have googled rocket launches from the uk. on of the sites i a place called south uist. I have found the average temperature there to be about 7 degrees C so we could use this as our default case and then on the start menu when it says what the programme is we could just say "this programme is designed to simulate an Atlas V launching from Soutch Uist" or something like that*/
