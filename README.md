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
