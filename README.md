# JavaQuestions

1. We can't change the string as it is imutable but using stringBuilder we can do so?
   
  import java.util.*;
  class HelloWorld {
      public static void main(String[] args) {
          StringBuilder sb = new StringBuilder("raghav");
          int low = 0;
          int high = sb.length()-1;
          while(low <= high){
              char temp = sb.charAt(low);
              sb.setCharAt(low,sb.charAt(high));
              sb.setCharAt(high,temp);
              low++;
              high--;
          }
          System.out.println(sb);
      }
  }
