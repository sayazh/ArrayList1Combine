# ArrayList1Combine

public static void main(String[] args) {
		String[] ar1= {"f","o","o"};
		String[] ar2= {"b","a","r"};
		String word=combineRs(ar1, ar2);
		System.out.println(word);
	}
	
	/*
	 * combine two String arrays into 
	 * one ArrayList and return it as a string.
	 */
	public static String combineRs(String[] r1, String[] r2) 
	  {
	 ArrayList<String> str = new ArrayList<>(r1.length+r2.length);
	 
	for(int z=0; z<r1.length; z++) {
	  str.add(r1[z]);
	  }
	 for (int j=0; j<r2.length; j++) {
	  str.add(r2[j]);
	 }
	  
	 String newStr ="";
	// for(int z=0; z<str.size(); z++) {
		//newStr+=str.get(z);
	// }
	 for(String s :str) {
		 newStr+=s;
	 }
	  return newStr;
	   
	  }
}
