# Reverse String

## Java

```Java
public class Solution {
    public String reverseString(String s) {
        // First solution, iterate through String
        char[] in = s.toCharArray(); // s.split() gives you a String[]  
        char[] out = new char[s.length()]; // when making a new primitive array, make sure to set its size!
        
        // Already reversed
        if (s.length() <= 1) {
            return s; 
        }
        
        // Otherwise
        for (int i=0; i<s.length(); i++) {
            out[s.length()-1-i] = in[i];
            out[i] = in[s.length()-1-i];         
        }
        
        return new String(out);
    }
}
```

### Things I learned

* s.split() gives you a String[] 
* s.toCharArray() is what gives you a char[]!
* if you init a new array, you have to set its size (for ex. `char[] out = new char[s.length()];`
