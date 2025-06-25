# Isomorphic-in-hashmap
package HashMap;
import java.util.*;
// iska mtlb h ki aab - xxy --- a a x x se replace hoga or b y se
public class isomorphic {
    public boolean isIsomorphic(String s,String t) {
        HashMap<Character, Character> mp = new HashMap<>();
        for (int i = 0; i < s.length(); i++) {
            Character sCh = s.charAt(i);
            Character tCh = t.charAt(i);
            if (mp.containsKey(sCh)) {
                if (mp.get(sCh) != tCh) {
                    return false;
            }

            } else {
                if (mp.containsValue(tCh)) {

                return false;
            }

        
        mp.put(sCh, tCh);
    }


        }

        return true;
    }
    }
