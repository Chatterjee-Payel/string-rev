# string-rev

string reverseString(string s)
{
    //code here.
    string ans;
   unordered_set<char>m;
   unordered_set<char>ans2;
   for(int i=s.size()-1;i>=0;i--){
       if(s[i]==' '){
           continue;
       }
       if(ans2.find(s[i])==m.end()){
           ans+=s[i];
          ans2.insert(s[i]);
       }
   }
   return ans;
};
