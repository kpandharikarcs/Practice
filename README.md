class Solution {
    public int[] plusOne(int[] digits) {
        
        int lastdigit = digits.length-1;
        for(int i=lastdigit;i>=0;i--){
             if(digits[i]==9){
                digits[i] =0;
                System.out.println(i);
        }
        else{
            digits[i]++;
            return digits;
        }
        
        }
        digits = new int[digits.length+1];
        digits[0]=1;
        return digits;
    }
}
