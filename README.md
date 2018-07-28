# Ch.8-Notes-L9-
**SORTING**

    counts.put(word, count == null ? 1: count + 1);
    
    //essentually counts.put(Key, value(aka count +1)
    //        "does count equal null? if TRUE return a 1, if FALSE return count + 1"
    //if count != null, it equals an integer (integer + 1)
    //a turnury operator (3 way operator) 
    
    Main.java
    (line 18)
    //what the HashMap entries are copied into:
    final ArrayList<Map.Entry<String, Integer>> arr = new ArrayList<>(counts.size());
    //ArrayList of TYPE Map.Entry<each entry is a STRING INTEGER>>calling it "arr" = its a new ArrayList(this ArrayList is however big the map is
    
    (line 19)
    arr.addAll(counts.entrySet());
    //entrySet() converts HashMap entrySet takes the entire entry as a key, value pair considers it a Map enntry (Map.Entry)
    considers it as one unit each, then add all to array list b/c a HashList is NOT iteratble/sortable 
    
    
    One I have (line 22-25), its the same for ALL implememtations of Map
    
    Lab9 vid (24 min in)
    Elements in ArrayList is a LinkedList (NOT in, NOT string) LL!
        key=word->hashCode of word = %size of hash table ==gives=>index into the ArrayList
        then, for every new word, I create a new node
        if word is already found, CALCULATE its hashCode, TAKE key (aka the word), hashCode of that word (aka floor.%)size of
   
        table (which give sthe index), use that to see if there is a word there or a LL
        if no LL, create one and put value(1) in
        if there is a LL, start searching through LL to say:
        are you the key? is this the count where myWord is located?
        if YES, ++ (increment by 1)


The java.lang.Math.floor(double a) returns the largest (closest to positive infinity) double value that is less than or equal to the argument and is equal to a mathematical integer. Special cases: If the argument value is already equal to a mathematical integer, then the result is the same as the argument.

MyHashMap.java
        
        private static final int DEFAULT_TABLE_SIZE = 11; //default is ALWAYS 11
  
  //size of hashTable = HOW MANY buckets we have, different from hashMap
  //size of myHashMap = go through every bucket and see evey node, every LL, and every bucket in this ArrayList
    //**HASHMAP > HASHTABLE
