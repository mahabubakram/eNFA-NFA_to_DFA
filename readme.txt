Name: Mahabub Akram
ID: 0910024040
Course: CSC 273

IDE: Netbeans
Compiler : JDK java compiler(ubuntu iced tea also included)

Algorithm : 
Just normal algorithm to convert E-NFA to DFA nothing else
and my most efficient block of code is the upper function and eclosure function which both efficiently
by recursion calculate the epsilon state of a input state.
First I just calculated the epsilon state for each state and save that , and then i check each state of its edges 
and defined it with their epsilon states.

and then i just merge the value with their edges and stored it in a HashMap.

after that DFA building is finishe/// seems easy !!!!!!!!!! but not was easy for me

then i changed the DFA to min_dfa
I just built 437589 combinations of string then check for the DFA minimum states

Sample Input :

nfa.put("0_a", "");
                nfa.put("0_b", "");
                nfa.put("0_e", "1_7");

                nfa.put("1_a", "");
                nfa.put("1_b", "");
                nfa.put("1_e", "4_2");

                nfa.put("2_a", "3");
                nfa.put("2_b", "");
                nfa.put("2_e", "");

                nfa.put("3_a", "");
                nfa.put("3_b", "");
                nfa.put("3_e", "6");

                nfa.put("4_a", "");
                nfa.put("4_b", "5");
                nfa.put("4_e", "");

                nfa.put("5_a", "");
                nfa.put("5_b", "");
                nfa.put("5_e", "6");

                nfa.put("6_a", "");
                nfa.put("6_b", "");
                nfa.put("6_e", "1_7");

                nfa.put("7_a", "8");
                nfa.put("7_b", "");
                nfa.put("7_e", "");

                nfa.put("8_a", "");
                nfa.put("8_b", "9");
                nfa.put("8_e", "");

                nfa.put("9_a", "");
                nfa.put("9_b", "10");
                nfa.put("9_e", "");

                nfa.put("10_a", "");
                nfa.put("10_b", "");
                nfa.put("10_e", "");

                System.out.println(in_symbol);
                System.out.println(first);
                System.out.println(last);
                System.out.print(nfa);
                in_symbol.add("a");
                in_symbol.add("b");
                result.add(10);


Sample Output:
Final symbolic dfa
{A_a=B, A_b=C, B_a=B, B_b=D, C_a=B, C_b=C, D_a=B, D_b=E, E_a=B, E_b=C}

aabba
Rejected

minimized dfa
This is the minimized dfa where the small letters are edges and block are merged states 
{_A_C_a=B, _A_C_b=_A_C, B_a=B, B_b=D, D_a=B, D_b=_E, _E_a=B, _E_b=_A_C}