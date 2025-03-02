# Gum
//
//  main.cpp
//  Portfolio I
//
//  Created by GuM on 2/15/25.
//

#include <iostream>
#include <cstdlib>
#include <ctime>

int main() {
    using namespace std;
    
    srand(static_cast<unsigned int>(time(0)));
    
    string choice1, choice2, acceptOffer, spiritTalk;
    
    cout << "A spirit manifests before thee\n";
    
    cout << "⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n";
    cout << "⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣸⣿⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n";
    cout << "⠀⠀⠀⠀⠀⠀⠀⠀⠀⣰⣿⣿⣷⡆⠀⠀⠀⠀⠀⠀⠀⠀⠀\n";
    cout << "⠀⠀⠀⠀⠀⠀⠀⢀⣾⣿⣿⣯⣿⣃⡀⠀⠀⠀⠀⠀⠀⠀⠀\n";
    cout << "⠀⠀⠀⠀⠀⢰⡆⣿⣿⣿⣿⣿⣿⣿⠁⣴⡄⠀⠀⠀⠀⠀⠀\n";
    cout << "⠀⠀⠀⠀⣠⣿⣷⣿⣿⣯⣿⣿⡿⣿⢸⣿⣵⡀⠀⠀⠀⠀⠀\n";
    cout << "⠀⠀⢀⣴⣿⣿⣿⣿⣏⡿⣿⣿⣿⣿⣿⣿⣿⣦⣦⡀⠀⠀⠀\n";
    cout << "⠀⣰⣿⣿⣿⣟⣿⢾⠿⢛⣓⣉⢙⠻⢿⣽⣿⡿⣿⣿⡦⡀⠀\n";
    cout << "⣸⣿⢯⣿⣿⣻⠍⢀⣴⣿⢿⣿⣿⣿⡦⠙⣿⣿⣿⠏⢻⣷⠀\n";
    cout << "⣿⣿⠸⣿⣿⣿⢀⣬⣷⠶⠆⠈⢻⣿⣿⡇⢸⣿⣿⡆⠸⣿⠇\n";
    cout << "⠹⣿⣗⣙⢿⣷⢼⣿⣿⠁⠀⠀⣸⡟⠍⢠⣾⣿⣟⣠⣿⠟⠀\n";
    cout << "⠀⠈⠛⢿⣷⣯⣟⡿⢷⣵⣤⣠⣤⣤⣶⣿⣿⣿⢿⠿⠉⠀⠀\n";
    cout << "⠀⠀⠀⠀⠈⠘⠻⣷⣧⣦⣈⠉⣩⣵⡿⡿⠛⠉⠀⠀⠀⠀⠀\n";
    cout << "⠀⠀⠀⠀⠀⠀⠀⠀⠉⠻⣿⣿⠟⠟⠁⠀⠀⠀⠀⠀⠀⠀⠀\n";
    cout << "⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n";
    
    cout << "proclaims \"I have awaited thy arrival for countless moons. \nCome forth, and I shall guide thee to thy destiny.\"\n";
    cout << "Utter the sacred words: 'Aham' to embark upon thy fate: " << endl;
    getline(cin, acceptOffer);
    
    if (acceptOffer != "Aham") {
        cout << "I have made a mistake, you are not the chosen one, but we shall meet again, human...\n";
        return 0;
    }
    
    if (acceptOffer == "Aham") {
        cout << "I have sent you to the realm where your destiny was waited long enough.\n";
        cout << "Thousand of years ago, the Great Buddha had set a path for you.\n";
        cout << "Your hand will be the slayer of the evil one and take the justice for your kinds.\n";
        cout << "From now, follow your path on your own. But, afraid not... I will be with you through the end..."<< endl;
        
        cout << "You start walking out of the portal and you saw the light.\n";
        cout << "You are standing at a fork in the road near Indawgyi Lake.\n" << endl;
        cout << "There are two paths leading to the dragon: the Valley Path and the Canal Path.\n";
        cout << "Which path will you choose?\n" << "1)Valley\n" << "2)Canal)\n" << endl;
        cin >> choice1;
        
        while (choice1 != "1" && choice1 != "2" && choice1 != "Valley" && choice1 != "Canal") {
            cout << "There is no such place, please seek the right path.\n";
            cin >> choice1;
        }
        
        if (choice1 == "1") {
            choice1 = "Valley";
        } else if (choice1 == "2") {
            choice1 = "Canal";
        }
        
        int randomEvent = rand() % 2;
        if (randomEvent == 0) {
            cout << "\nAs you walk towards the dragon's lair, the spirit speaks again.\n";
            cout << "'Young one, before you reach your destiny, a decision must be made...'";
            cout << " The spirit pauses and then adds: 'The dragon will ask for mercy if your fate is ture...\n";
            cout << "I am the spirit, I do not know much about the dragon.\n";
            cout << "I am just a guide to you and help you through the journey.'\n" << endl;
        } else if (randomEvent == 1) {
            cout << "\"When a man is a traveler, the world is his home, and the sky is his roof. Where he hangs his hat is his home, and all people are his family.\"\n" << endl;
        } else {
            cout << "\"I may not have gone where I intended to go, but I think I have ended up where I needed to be.\"\n" << endl;
        }
        
        int spiritChoice = rand() % 2;
        if (spiritChoice == 0) {
            cout << "Sometimes, a choice is not as clear as it seems. Consider what lies beyond the consequences...\n";
            cout << "Some beautiful paths can’t be discovered without getting lost.\n" << endl;
        } else if (spiritChoice == 1) {
            cout << "The dragon is both a creature of wrath and wisdom. Approach with care, for its mind is older than time itself.\n" << endl;
        } else {
            cout << "Beware, young one. If you choose to wake the dragon, its fury will know no end. If you let it rest, peace may be yours... for now.\n" << endl;
        }
        
        if (choice1 == "Valley") {
            cout << "\nYou have chosen the Valley Path. You walk through the valley and finally reach the dragon.\n";
            cout << "You see the great petrified dragon. A monk sits nearby.\n";
            
            cout << "⠀⠀⠀⠀⠀⠀⠀⠀⢠⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀" << endl;
            cout << "⠀⠀⠀⠀⠀⠀⠀⠀⠀⢧⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀" << endl;
            cout << "⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠻⣦⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠤⠤⣤⣀⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀" << endl;
            cout << "⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠻⣦⣄⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠙⠻⣶⣤⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀" << endl;
            cout << "⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠛⢿⣶⣤⣄⡀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢻⣿⣷⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀" << endl;
            cout << "⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠙⠻⢿⣿⣶⣤⣤⣀⣀⣀⣀⣠⣾⣿⣿⣿⣷⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀" << endl;
            cout << "⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣈⣹⣿⣿⣿⣿⣿⣿⣿⣿⡿⠿⣿⣿⣿⣷⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀" << endl;
            cout << "⠀⠀⠀⠀⠀⠀⠀⣀⣠⣤⣤⣤⣤⣤⣄⣀⣤⣶⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣦⣀⠉⢿⣿⣿⣷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀" << endl;
            cout << "⠀⠀⠀⠀⡠⠶⠛⠋⠉⠉⠙⢻⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣄⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀" << endl;
            cout << "⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⣴⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⣦⣤⣀⠀⠀⠀⠀⠀⠀" << endl;
            cout << "⠀⠀⠀⠀⠀⠀⠀⣀⣾⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡍⠛⠿⣿⡛⢿⣿⣿⣿⣿⣿⣿⣿⣍⡳⣦⡀⠀" << endl;
            cout << "⠀⠀⠀⣠⣴⣶⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡿⠋⠁⠀⠙⣿⣿⣇⠙⢿⣦⡀⠘⠇⠀⠙⢿⡏⠉⠻⣿⡝⠻⣿⣿⣿⣷⠀⠀" << endl;
            cout << "⠀⢠⠞⠉⠀⢨⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠟⠀⠀⠀⠀⠀⢹⣿⣿⣆⠀⠙⢿⣄⠈⠀⠀⠈⠃⠀⠀⠘⠇⠀⠘⣿⠙⣿⠀" << endl;
            cout << "⠠⠁⠀⠀⠀⣼⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡇⠀⠀⠀⠀⠀⠀⠀⢻⣿⣿⣷⣤⣀⠙⠷⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠇⠀" << endl;
            cout << "⠀⠀⠀⠀⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠻⣿⣿⣦⡀⠀⠀⠈⠛⢶⣤⣀⣀⣀⣀⡀⠀⠀⠀⠀⠀" << endl;
            cout << "⠀⠀⠀⢀⣾⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠻⢿⣿⣟⡉⠀⡀⠀⠀⠉⠛⠛⠻⢭⡉⠂⠀⠀⠀" << endl;
            cout << "⠀⠀⢠⡿⠋⢹⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠛⠿⠯⠤⠀⠀⠀⠀⠀⠀⠀⠈⠂⠀⠀⠀" << endl;
            cout << "⠀⠀⡜⠀⠀⠈⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⣦⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀" << endl;
            cout << "⠀⠀⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀" << endl;
            
            cout << "The monk says; Finally, you have arrived. Make your own choices, Do you want to wake the dragon or let him remain petrified?\n" << "1)Wake the dragon\n" << "2)Let it be\n" << endl;
            
        } else {
            cout << "\nYou have chosen the Canal Path. You walk through the temple and finally see the dragon.\n" << endl;
            
            cout << "               \\         O_._._._A_._._._O          /( " << endl;
            cout << "                \\`--.___,'===============`.___,--' /   " << endl;
            cout << "                 \\`--._._                  _._,--'/    " << endl;
            cout << "                  \\  ,. l`~~~~~~~~~~~~~~~'l ,.  /      " << endl;
            cout << "                    \\||(_)!_!_!_.-._!_!_!(_)||/        " << endl;
            cout << "                      ||_|____!!_|;|_!!____|_||         " << endl;
            
            cout << "Spirit says, Do you want to wake the dragon or let him remain petrified?\n" << "1)Wake the dragon\n" << "2)Let it be\n" << endl;
        }
        
        cin >> choice2;
        while (choice2 != "Wake" && choice2 != "Let" && choice2 != "1" && choice2 != "2") {
            cout << "Find the truth, choose wisely young one.\n";
            cin >> choice2;
        }
        
        if (choice2 == "1") {
            choice2 = "Wake";
        } else if (choice2 == "2") {
            choice2 = "Let";
        }
        
        if (choice1 == "Valley" && choice2 == "Wake") {
            cout << "Here, read this spell out loud. It was written by languages of your kinds.\n";
            cout << "You used an ancient spell cast to wake the dragon.\n";
            cout << "✧･ﾟ: *✧･ﾟ:* 　　 *:･ﾟ✧*:･ﾟ✧\n";
            cout << "        ✧･ﾟ: *✧･ﾟ:* 　　 *:･ﾟ✧*:･ﾟ✧";
            
            cout << "The great dragon wakes up. Grouhhhh..........\n";
            cout << "Behold,... The dragon said: 'You must be the destined one, my child,\n"
            << "I have been waiting for this moment. I know young child, I have made a mistake by broking the promises of god.I accepted my punishment to suffer for ten thousand years. But now, the curse is broken. I believe Buddha forgives me because he sent you... I realized... Let it be,Thank you...young man..'\n";
            cout << "Spirti makes a protal and set the dragon free. The dragon flew up to the highest sky and enter the portal with the highest speed. At last, the dragon and spirit combines together and reincernates to afterlife together.\n" << endl;
            cout << "The monk show you the way to home.\n" << endl;
        
        } else if (choice1 == "Valley" && choice2 == "Let") {
            cout << "The monk tells you the story of the dragon.\n";
            cout << "This dragon was petrified by Buddha because he broke his promises to heaven.\n";
            cout << "There was a village near the great lake named Indawgyi. The people of Indawgyi were blessed by the heavenly gods for their faithful heart and strong belief in Dhamma.\n";
            cout << "And a great serpent lived inside the lake, the serpent was trying to turn to a dragon.\n";
            cout << "Initially, the serpent practice accodring to the way of Buddha to achieve the dragon form.\n";
            cout << "One day, when the serpent came closer to the shore and haunts the fish for lunch, a little child falls into the lake.\n";
            cout << "The serpent accidently swallow the little kid, the serpent feels something very strange feeling as it felt the power inside rises.\n";
            cout << "From that day it devour the Dhamma, it greed never stop as it never comsume the power but the power blind its eyes of justice. It started to hunt good people of Indawgyi day after day. The serpent finally turned into dragon after thitry fullmoon days.\n";
            cout << "For what he has comitted, the heavenly gods punished him for a thousand years to be stoned and on the last day, he will be died in the hand of a descendant of the Dhamma.'\n";
            cout << "The spirit said: now both of us discover the truth, young.\n" << endl;
            cout << "I will sent you to your realm again, child.\n" << endl;
            
        } else if (choice1 == "Canal" && choice2 == "Wake") {
            cout << "You used an ancient spell to wake the dragon.\n";
            cout << "✧･ﾟ: *✧･ﾟ:* 　　 *:･ﾟ✧*:･ﾟ✧\n";
            cout << "      ✧･ﾟ: *✧･ﾟ:* 　　 *:･ﾟ✧*:･ﾟ✧\n";
            cout << endl;
            cout << "The dragon wakes up and attacks you because it is finally free.\n";
            cout << "As the fate had set a path for you, you must end it life' said the spirit.\n";
            cout << "The great dragon attacks you with the flames from its lungs.\n";
            cout << "Spirit blessed you with the all almighty sword and sacred shield.\n";
            cout << "As the fate comes,you strikes its heart with all strength.\n";
            cout << "The Evil shall fall. He has to suffered from his acts.\n";
            cout << "The long history of the tale has come to an end.\n" << endl;
            cout << "Be the fate and destiny in your hands!\n" << endl;
            
        } else if (choice1 == "Canal" && choice2 == "Let") {
            cout << "You must made a decision, young one. I know you are being merciful to the dragon. But remember young man, giving a mercy to the wrong can only lead to an unimagineable disaster.\n";
            cout << "The heaven knows what they had done, and you should know what is yours.\n";
            cout << "You have chose not to wake the dragon. This is your chance...\n";
            cout << "Now, you have a chance to slay the dragon in its petrified form, the chosen one.\n";
            cout << "The spirit said; End its life, this is the time to take the creature's life.\n";
            cout << "Your destiny is to end the dragon, no matter what....\n";
            cout << "You cannot turn back....\n";
            cout << "The monk gives you the mighty sword to take the life of the dragon.\n";
            
            cout << "       ./~\n";
            cout << "(=#####{>==================- \n";
            cout << "       `\\_\n";
            
            cout << "You slay the dragon and fulfill the purpose of mission, your destiny to end the dragon's life.\n" << endl;
            cout << "I will sent you to your realm again, child.\n" << endl;
        }
       
        return 0;
    }
}
